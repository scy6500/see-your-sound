# 👀🔉 See Your Sound
![Image_20230907_175057_063](https://github.com/KOBOT-BOARD12/.github/assets/110521260/fc088ce2-1452-4961-b275-eba0093d0b20)

### 🔧 개발 배경 및 목적
청각 장애인은 일반인보다 도로에서 사고에 노출될 위험이 더 높다고 한다. 또, 최근 사회에 대한 불만을 가지고 심리적 불안 증세를 나타내는 이들의 묻지마 범죄가 대폭적으로 증가되고 있는데, 청각 장애인은 이러한 상황을 인식하고 대피하기가 더 어려울 것이다. 이 앱은 청각 장애인이 주변 상황에서 발생하는 소리와 방향을 인식하는 데에 도움을 주기 위한 목적으로 설계되었다. 인공지능 기술을 활용하여 앱에서 소리를 실시간으로 인식 후, 앱 화면을 통해 소리의 종류나 미리 등록된 예약어인지의 여부, 소리의 방향을 알려 주는 서비스를 제공하는 것이 목적이다. 결과적으로 청각 장애인이 겪는 각종 사고 발생 가능성을 줄이는 효과를 기대하고 있다.

### 🎥 프로젝트 시연 동영상
[🎬 영상 보러 가기](https://youtu.be/5TegST750mc)


### 📂 레포지토리별 개요 및 링크
`📌 레포지토리 이름을 누르면 각 레포지토리별 실행 방법을 확인할 수 있다.`

🔎 [SeeYourSound FrontEnd](https://github.com/KOBOT-BOARD12/seeyoursound-frontend.git): Android Studio에서 JAVA 언어를 사용하여 주변 소리와 등록한 예약어를 탐지할 수 있는 앱을 개발하고 디자인하였다.

🔎 [SeeYourSound BackEnd](https://github.com/KOBOT-BOARD12/seeyoursound-backend.git): Python 언어를 사용하여 주로 DB와의 연결, 예약어 관련 API와 소리 클래스 선택 API 개발, 앱과 서버의 연결을 위해 websocket 프로토콜을 정의하였다.

🔎 [SeeYourSound Model Serving](https://github.com/KOBOT-BOARD12/seeyoursound-model-serving.git): 소리 분류 모델, 등록된 예약어와 탐지된 소리의 유사도를 비교하는 모델, 방향 탐지 모델을 서빙하였다.

### 🎉  See Your Sound App 실행 순서
0. repository clone - 중앙 제어 서버
```shell
git clone https://github.com/KOBOT-BOARD12/seeyoursound-backend.git
```
1. repository clone - 모델 서버 `(※ gpu가 탑재돼 있는 환경에서 실행시키는 것이 효율적이다.)`
```shell
git clone https://github.com/KOBOT-BOARD12/seeyoursound-model-serving.git
```
2. 중앙 서비스 서버와 모델 서버를 실행시킨다. 
```shell
uvicorn app:app --port={$port}
```
3. SeeYourSound App을 실행시킨다.

---
# 팀원 소개 및 역할
1. 💥 윤민상

- Position : 팀장
- Github: <https://github.com/minsang22>
- Email : nornen20@kookmin.ac.kr
- Role
  - 모델 개발 및 서빙

2. 🌖 성창엽

- Position : 팀원
- Github: <https://github.com/scy6500>
- Email : scy6500@kookmin.ac.kr
- Role
  - 서버 개발 및 모델 개발

3. 🖤 안수현

- Position : 팀원
- Github: <https://github.com/3uhyeon>
- Email : saker123456@kookmin.ac.kr
- Role
  - 모바일 앱 디자인 및 개발

4. 😫 김영석

- Position : 팀원
- Github: <https://github.com/youngseok0>
- Email : kys030908@kookmin.ac.kr
- Role
  - 모델 개발 및 서빙

5. 🫨 신수민

- Position : 팀원
- Github: <https://github.com/syngrxm>
- Email : 5luck21948@kookmin.ac.kr
- Role
  - 서버 개발