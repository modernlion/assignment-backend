# assignment-backend
KONKRIT Backend 코딩 과제

# [Beckend 과제] ERC721 Contract 수집

## 배경
회사는 이더리움 네트워크에서 생성되고 거래되는 ERC721의 Contract들의 PFP이미지나 Rarity같은 메타 정보들을 데이터화하고 사용자에게 제공하고 싶어합니다. 관리자는 Raw 데이터를 `Google 스프레드시트`를 통해 보는 것에 익숙하고 (가상의) 사용자는 Syltare Contract의 Token ID `222`번의 정보를 보고 싶어합니다. (1) Syltare Contract에 민팅된 모든 아이템의 정보들을 Google 스프레드 시트에 옮기고,  (2) Syltare Contract의 Token ID 222번 아이템과 관련된 자료들을 프론트로 제공하는 API를 제공해주어야 합니다. 해당 API를 통해 사용자의 거래를 원활히 할 수 있게 도움을 주고자 합니다.

당신은 백엔드 엔지니어로서 위에서 언급된 (1) 과 (2) 의 작업을 하여 API 를 제공하는 웹 서버 어플리케이션을 제작해야 합니다.

## 목적
- 백엔드 개발 역량을 중점적으로 평가합니다.
- 평소 어떤 식으로 프로그래밍 하는지 그 스타일을 봅니다.
- 다른 프로그래머가 재활용 할 수 있게끔 자신의 코드를 구조화 할 수 있는지를 확인합니다.

## 요구 사항
### 데이터 수집
- Contract 주소는 관리자나 사용자 요청에 따라 변동될 가능성이 있으나 Syltare Contract를 기준으로 합니다.
- Syltare의 Contract주소는 `0xff80bd43e3f0e414afc70cb8ac1d3f0e6a303a2f` 입니다.
- Contract의 조회 및 수집하는 방법에는 제한이 없으나 [Alchemy](https://www.alchemy.com/)를 이용하여 Contract의 정보 조회가 할 수 있습니다.

### Google 스프레드시트 연동
- Google spreadsheet API를 직접 컨트롤 하거나 공개된 다른 라이브러리를 사용해도 무관합니다.
- 데이터를 기입할 시트는 임의로 만드셔도 무방하나, 평가 시 접근이 가능해야 합니다.
- 연동되는 정보들은 응답에 필요한 필수 정보들을 저장하고 부가적인 정보도 업데이트가 되어야 합니다.

### API 제공
- Contract 정보를 스프레드시트에 입력하는 API와 조회하는 API가 있어야 합니다.
- 가상의 Frontend Engineer가 해당 데이터를 전달 받아 화면을 구성할 예정이라는 가정을 두고, 이를 구현하여 주시기 바랍니다.

## 평가 요소
- 3rd Party API활용을 할 수 있는가
- 입/출력될 자료들을 상황에 맞게 데이터로 정형화 할 수 있는가
- 이더리움 블럭체인의 기본 지식이 있는가
- 문제의 부분 문제를 두고, 각 부분 문제의 우선 순위를 잘 설정할 수 있는가
- 주어진 시간 안에 달성할 수 있는가
- 다른 사람이 유지 보수할 수 있게 배려하는가 (문서화, 주석, 네이밍 등)
- 기초적인 알고리즘, 자료 구조 개념
- 문제를 추상화하기 위한 언어적 도구를 잘 활용하는가
- 버전 관리 시스템을 적절하게 사용할 줄 아는가
- 표준적인 코딩 관습을 잘 따르는가
- 코드가 충분히 방어적으로 짜여져 있는가

## 제출 방법
지정된 Git 저장소에 작업 내용을 푸시합니다. 평가는 저장소 내용만으로 진행합니다. 평가자가 참고해야 할 사항이 있다면 저장소의 README 등을 이용합니다.