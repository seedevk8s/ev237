# EV237!

**Simple Docker Example**

repository에는 다음과 같은 Dockerfile, html 디렉토리가 있으며,
해당 디렉토리에서 docker build명령을 실행하면 nginx 웹서비스를 통해 웹페이지를 확인할 수 있음.

#### 컨테이너 빌드 
$ git clone https://github.com/237summit/ev237.git <BR>
$ cd ev237 <BR>
$ docker build -t ev237 . <BR>
$ docker images ev237 <BR>

#### 컨테이너 실행
$ docker run -p 80:80 --name c1  -d ev237

#### 컨테이터 실행 확인
웹브라우저를 실행해 localhost 로 접속한다.


#### Files


```mermaid

ev237/
├── Dockerfile
├── html
│   ├── images
│   │   └── ev237.jpg
│   └── index.html
└── README.md
