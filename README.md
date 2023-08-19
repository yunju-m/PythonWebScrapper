# PythonWebScrapper
**Python으로 웹 스크래퍼 만들기 :sparkles:** </br>
**개발기간 : 2023.03.21 ~ 2023.03.26**

## 프로젝트 소개
☑️ Replit 사이트를 이용한 파이썬 코드 작성 </br>
☑️ 웹 사이트의 작동여부 확인 프로그램을 만들어본다. </br>
☑️ 검색어를 입력했을 때 indeed.com 사이트 결과 데이터를 추출한다. </br>
☑️ 추출한 결과 데이터를 결과 페이지에 출력한다.

## Stacks ⭐
### Environment
![Replit](https://img.shields.io/badge/Replit-F26207?style=for-the-badge&logo=Replit&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/VisualStudioCode-007ACC?style=for-the-badge&logo=VisualStudioCode&logoColor=white)

### Development
![Html](https://img.shields.io/badge/Html-E34F26?style=for-the-badge&logo=Html5&logoColor=white)
![Css](https://img.shields.io/badge/Css-1572B6?style=for-the-badge&logo=Css3&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=Flask&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white)

### git connection

```bash
$ git clone https://github.com/yunju-m/PythonWebScrapper
$ cd .
```

## 환경설정
### venv 가상환경
#### 가상환경 생성 및 pip 업데이트
```bash
$ python -m venv venv
$ venv\Scripts\activate.bat
$ pip install --upgrade pip
```

#### 가상환경 종료
```bash
$ deactivate
```

### 설치 목록 확인 명령어
```bash
$ pip list
```

### request 설치
request란 구글 웹 사이트에 접속하는 경우, 내 브라우저는 Google 서버에 request를 보내고 Google 서버는 나한테 웹 사이트를 보내준다. 
```bash
$ pip install requests
```

### Beautifulsoup4 설치
```bash
$ pip install beautifulsoup4
```

### Selenium 설치
```bash
$ pip install selenium
```

### flask(플라스크) 설치
```bash
$ pip install flask
```

### flask 애플리케이션 설정
#### pythonwebscrapper.cmd 생성
- myproject.cmd 파일에 이 명령어를 미리 추가해 놓으면 매번 환경 변수를 입력할 필요없다. 
- venv 가상환경에 PythonWebScrapper.cmd생성한다.
- 환경 변수 FLASK_APP에 main라는 값을 설정한다.
- main은 앞에서 작성한 main.py 파일을 의미한다.
- 디버깅이 가능하도록 설정해준다.

```bash
@echo off
cd c:/GitHub/PythonWebScrapper
set FLASK_APP=main
set FLASK_DEBUG=true
c:/venv/scripts/activate
```

#### WARNING: This is a development server. 경고문구 발생
- <span style="color:red">플라스크 서버가 개발 모드로 실행되었기 때문이다.</span>
- 운영 환경에서는 flask run으로 실행하는 개발서버가 아닌 WSGI 서버로 실행해야 한다. 

## 실행 명령어
```bash
$ flask run
```

## 프로젝트 진행 상황
| 날짜 |     내용      |
| ---- | ------------- |
|2023.03.21 | Replit 사이트 로그인, 배경 설정 |
|2023.03.21 | Replit을 이용한 파이썬 코드 작성 연습 |
|2023.03.22 | 파이썬 자료구조 |
|2023.03.22 | 웹사이트 작동 여부 확인 프로그램 구현 |
|2023.03.22~25 | 웹 스크래퍼 구현 |
|2023.03.25 | 데이터 추출 결과 csv 저장 |
|2023.03.26 | Flask를 이용한 검색어 웹사이트 구현 |

## 화면 구성 📺
| 메인 페이지 | 결과 페이지 |
| :----------------: | :---------------: |
| <img src="/img/메인페이지.png"> | <img src="/img/결과페이지.png">              |