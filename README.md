# Controlling LED with Flask Web Server on Raspberry Pi

라즈베리파이와 Flask 웹서버를 연동하여 웹 브라우저에서 LED를 제어하는 IoT 기본 실습 프로젝트입니다.

## 📌 프로젝트 개요

- 라즈베리파이 GPIO 21번 핀에 연결된 LED를 웹페이지에서 제어
- Flask 웹서버를 통해 [ON] / [OFF] 버튼으로 LED 동작
- URL 라우팅 방식 및 HTML 폼 POST 방식 두 가지 구현

## 🎬 데모 영상

[![Demo Video](https://img.youtube.com/vi/6iWOoXbwbXU/0.jpg)](https://www.youtube.com/watch?v=6iWOoXbwbXU)

## 🛠️ 사용 부품

| 부품명 | 수량 |
|---|---|
| 라즈베리파이 | 1개 |
| 빨강 LED | 1개 |
| 330옴 저항 | 1개 |
| 암/수 점퍼케이블 | 2개 |

## ⚙️ 개발 환경

| 항목 | 내용 |
|---|---|
| Language | Python 3.x |
| Framework | Flask |
| Library | gpiozero |
| Hardware | Raspberry Pi |

## 📂 파일 구성

```
project_20/
├── main20.py        # URL 라우팅 방식 LED 제어
├── main20-1.py      # HTML 폼 POST 방식 LED 제어
└── templates/
    └── index.html   # 웹페이지 UI
```

## 🚀 실행 방법

```bash
# 기본 URL 라우팅 방식
sudo python3 main20.py

# HTML 폼 POST 방식
sudo python3 main20-1.py
```

브라우저에서 `http://라즈베리파이IP` 로 접속하면 됩니다.

## 📚 참고문헌

- [Flask 공식 문서](https://flask.palletsprojects.com/)
- [gpiozero 공식 문서](https://gpiozero.readthedocs.io/)
- [Raspberry Pi GPIO 문서](https://www.raspberrypi.com/documentation/computers/raspberry-pi.html)
- [Python 3 공식 문서](https://docs.python.org/3/)
- [MDN Web Docs - HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data)
