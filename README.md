# 👀🔉 See Your Sound
<그림>
### 🔧 개발 배경
청각 장애인과 길에서 이어폰을 끼고 다니는 즉, 외부 소리가 차단된 사람들이 도로 환경에서 발생하는 소리들을 인식하도록 하는 장치가 필요하다고 생각했다. 추가적으로 최근 이슈가 되었던 칼부림 등의 흉기 난동 사건에도 대비할 수 있을 것 같아 고안하였다.
### 🔦 개발 목적
인공지능 기술을 활용하여 앱에서 소리를 실시간으로 인식 후, 디스플레이 알림과 진동을 소리의 종류나 미리 등록된 키워드 여부, 소리의 방향을 알려 주는 서비스를 만드는 것이 목적이다. 결과적으로 청각 장애인과 도로 사용자의 각종 사고 발생 가능성을 줄이는 것이 목적이다.
### 📂 레포지토리별 개요 및 링크
`📌 레포지토리 이름을 누르면 각 레포지토리별 실행 방법을 확인할 수 있다.`

🔎 [SeeYourSound FrontEnd](https://github.com/KOBOT-BOARD12/seeyoursound-frontend.git): Android Studio에서 JAVA 언어를 통하여 실제로 사용자들이 사용할 수 있는 앱을 개발했다.

🔎 [SeeYourSound BackEnd](https://github.com/KOBOT-BOARD12/seeyoursound-backend.git): Python 언어를 통하여 주로 DB와의 연결, API 개발, websocket을 통해 앱과 서버를 연결했다.

🔎 [SeeYourSound Model Serving](https://github.com/KOBOT-BOARD12/seeyoursound-model-serving.git): 학습시킨 모델을 서빙했다.

### 🎉  See Your Sound App 실행 순서
0. 레포지토리 다운로드 - 중앙 제어 서버
```shell
git clone https://github.com/KOBOT-BOARD12/seeyoursound-backend.git
```
1. 레포지토리 다운로드 - 모델 서버 `(※ gpu가 탑재돼 있는 환경에서 실행시키는 것이 효율적이다.)`
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