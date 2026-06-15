## 1. 프로젝트 개요 / 项目概述
**한국어**
본 파일은 Flutter 여행 앱 전용 **항저우시(杭州市)** 관광 데이터를 정의한 코드입니다. 서호, 차 문화, 전통 거리, 항방 요리, 3일 여행 코스, 바로가기 메뉴 및 AI 여행 문답 기능을 통합하고 있으며, 앱 내 지역 여행 페이지에 연동하여 사용합니다.

**中文**
本文件是为 Flutter 旅行应用编写的**杭州市**旅游数据代码。整合了西湖风光、茶文化、传统街巷、杭帮菜、三日游玩路线、快捷功能入口与智能问答模块，用于应用内对应城市专题页面展示。

---

## 2. 파일 정보 / 文件说明
**한국어**
- 대상 파일 경로: `lib/models/city_data.dart`
- 참조 모델 파일: `travel_models.dart`
- 데이터 변수명: `hangzhouCity`
- 데이터 형식: `CityTravelData` 상수 객체

**中文**
- 目标文件路径：`lib/models/city_data.dart`
- 依赖模型文件：`travel_models.dart`
- 数据变量名：`hangzhouCity`
- 数据类型：`CityTravelData` 常量对象

---

## 3. 사용 방법 / 使用方式
**한국어**
1. 제공된 전체 코드를 `lib/models/city_data.dart` 파일에 추가합니다.
2. 앱 내 `cities` 도시 목록에 `hangzhouCity`를 등록합니다.
3. 프로젝트를 재실행한 후 항저우 관련 페이지가 정상 로드되는지 확인합니다.

**中文**
1. 将完整代码添加至 `lib/models/city_data.dart` 文件中。
2. 在项目的 `cities` 城市列表里注册 `hangzhouCity` 变量。
3. 重启项目，验证杭州专题页面所有内容可正常加载展示。

---

## 4. 데이터 구성 / 数据结构说明
**한국어**
`hangzhouCity` 객체는 총 6개 영역으로 나뉩니다.
1. **기본 도시 정보**: ID, 행정 구역, 명칭, 메인 타이틀, 홍보 문구, 대표 이미지, 지리·기후·도시 특징 소개
2. **주요 관광지**: 서호, 룽징 차밭, 허팡제 (이미지, 설명, 핵심 볼거리, 주소, 운영 안내 포함)
3. **특색 음식**: 서호초어, 동파육, 룽징새우 (요리 설명과 맛 특징 수록)
4. **3일 여행 일정**: 시간별 동선, 소요 시간, 현지 팁이 포함된 완전 여행 코스
5. **퀵 엔트리**: 도시소개, 관광지, 음식, AI 문답 4가지 기능 입구 (아이콘 및 테마 색상 설정)
6. **AI 자동 문답**: 인사말, 키워드별 응답 로직, 기본 답변 내용

**中文**
`hangzhouCity` 对象共分为六大板块：
1. **城市基础信息**：包含ID、省市名称、展示标题、宣传文案、轮播图、地理位置、气候与城市特色介绍
2. **热门景点**：西湖、龙井茶园、河坊街，附带配图、景点简介、游玩亮点、地址及开放说明
3. **特色美食**：西湖醋鱼、东坡肉、龙井虾仁，标注菜品介绍与口味特点
4. **三日行程**：分天规划旅行路线，明确游玩时段、停留时长与出行小贴士
5. **快捷入口**：城市介绍、景点、杭帮美食、智能问答四大功能入口，配置图标与主题配色
6. **智能问答**：包含欢迎语、关键词匹配回复、默认回复规则

---

## 5. 주의사항 / 注意事项
**한국어**
1. 이미지 소스는 외부 Unsplash 링크이므로 앱 실행 시 네트워크 연결이 필요합니다.
2. 차밭과 거리 내 개별 상점의 영업 시간이 각기 다르므로 현장에서 확인하는 것을 권장합니다。
3. 파일 내 기존 도시 데이터는 삭제하지 말고, `cities` 리스트에 본 데이터만 추가하세요.
4. 아이콘과 색상은 Flutter 기본 컴포넌트를 사용하며 앱 전체 테마에 맞춰 적용됩니다.

**中文**
1. 图片均引用 Unsplash 外部链接，运行应用需保持设备网络通畅。
2. 茶园、街区内各家商铺营业时间不统一，建议到达现场后再确认。
3. 请勿删除文件内原有其他城市数据，仅在城市列表中追加本条数据即可。
4. 页面图标与配色采用 Flutter 原生组件，适配应用整体视觉风格。

---

## 6. 운영 환경 / 运行环境
**한국어**
- 개발 프레임워크: Flutter
- 의존 클래스: `travel_models.dart` 내 `CityTravelData`、`Attraction`、`Food` 등
- 언어 지원: 한중 양문 동시 표시

**中文**
- 开发框架：Flutter
- 依赖类：`travel_models.dart` 中 `CityTravelData`、`Attraction`、`Food` 等实体类
- 语言适配：支持中韩双语对照展示

<img width="778" height="1304" alt="_cgi-bin_mmwebwx-bin_webwxgetmsgimg__ MsgID=1886265259099451165 skey=@crypt_16604cd7_86ded57eb51b28cfbcebb1afe8011cc9 mmweb_appid=wx_webfilehelper" src="https://github.com/user-attachments/assets/6a044e0c-07ad-4ab6-a14c-c846ac8a482a" />
<img width="778" height="1304" alt="_cgi-bin_mmwebwx-bin_webwxgetmsgimg__ MsgID=6314663987760623691 skey=@crypt_16604cd7_86ded57eb51b28cfbcebb1afe8011cc9 mmweb_appid=wx_webfilehelper" src="https://github.com/user-attachments/assets/4e13b81c-feee-4fcf-8105-c9958956e2bb" />

<img width="778" height="1304" alt="_cgi-bin_mmwebwx-bin_webwxgetmsgimg__ MsgID=9121605512950097654 skey=@crypt_16604cd7_86ded57eb51b28cfbcebb1afe8011cc9 mmweb_appid=wx_webfilehelper" src="https://github.com/user-attachments/assets/32845495-bcbc-41ff-b25a-f37bb1dbf63a" />
<img width="778" height="1304" alt="_cgi-bin_mmwebwx-bin_webwxgetmsgimg__ MsgID=6451736737989779213 skey=@crypt_16604cd7_86ded57eb51b28cfbcebb1afe8011cc9 mmweb_appid=wx_webfilehelper" src="https://github.com/user-attachments/assets/89ebe629-d442-44ae-aed2-ad004530d099" />









