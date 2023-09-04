# 👀🔉 See Your Sound
<그림>
### 🔧 개발 배경
청각 장애인과 길에서 이어폰을 끼고 다니는 즉, 외부 소리가 차단된 사람들이 도로 환경에서 발생하는 소리들을 인식하도록 하는 장치가 필요하다고 생각했다.
### 🔦 개발 목적
소리를 실시간으로 인식 후, 디스플레이 알림과 진동으로 소리의 종류나 미리 등록된 키워드 여부, 소리의 방향을 알려 주는 서비스를 만드는 것이 목적이다.
### 📂 레포지토리별 개요 및 링크
📌 레포지토리 이름을 누르면 각 레포지토리 별 실행 방법을 확인할 수 있습니다.

🔎 [SeeYourSound FrontEnd](https://github.com/KOBOT-BOARD12/seeyoursound-frontend.git): Android Studio에서 JAVA 언어를 통하여 실제로 사용자들이 사용할 수 있는 앱을 개발했다.

🔎 [SeeYourSound BackEnd](https://github.com/KOBOT-BOARD12/seeyoursound-backend.git): Python 언어를 통하여 주로 

🔎 [SeeYourSound Model Serving](https://github.com/KOBOT-BOARD12/seeyoursound-model-serving.git):

### 🎉  See Your Sound App 실행 순서
0. 레포지토리 다운로드 - 중앙 서비스 서버
```
git clone https://github.com/KOBOT-BOARD12/seeyoursound-backend.git
```
1. 레포지토리 다운로드 - 모델 서버 `(※ gpu가 탑재돼 있는 환경에서 실행시키는 것이 안정적입니다.)`
```
https://github.com/KOBOT-BOARD12/seeyoursound-model-serving.git
```
2. 중앙 서비스 서버와 모델 서버를 실행시킨다. 
```shell
uvicorn app:app --port={$port}
```
3. SeeYourSound App을 실행시켜 회원가입 후 알림을 받을 클래스를 선택하고, 필요한 키워드를 등록시킨다.
4. 주변 소리를 차단한 뒤 길을 걸으며 테스트한다. (...)

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
  - 모바일 앱

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
