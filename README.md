# Capstone-2022-1-30


### 1. 프로젝트 소개
주제: 오픈 소스 (Open Source)를 활용한 교내 (PNU) LoRaWAN 네트워크 망 구축 및 운용\
LoRaWAN을 사용한 부산대 옥외 주차장 모니터링 시스템을 구축했다.
### 2. 팀소개
박윤형, the4456@pusan.ac.kr, 서버 구축 및 개발 총괄\
오세영, seiyoung0@gmail.com, 임베디드 시스템 및 어플리케이션 개발
### 3. 시스템 구성도
본 프로젝트는 크게 세 부분으로 나누어 진다.\
초음파 센서를 사용하고 LoRa통신을 하기 위한 임베디드 디바이스, 도커를 통해 구축한 서버, 안드로이드 어플리케이션
전체적인 구성은 아래의 그림과 같다.
![Untitled Diagram drawio](https://user-images.githubusercontent.com/62279820/195645524-118db5f7-8c19-4c05-a1ec-c6dd0bf61f2f.png)

#### 3.1. 임베디드 디바이스
![parkinglot drawio (1)](https://user-images.githubusercontent.com/62279820/195645197-9030cc7d-653b-4774-b808-c67b95f1df67.png)
디바이스에는 초음파센서를 연결해 사용하고 있으며, 임베디드 보드는 LoRa통신을 위해 만들어진 것을 사용한다.
#### 3.2. 서버
![docker container drawio](https://user-images.githubusercontent.com/62279820/195646292-6afd2c37-055e-4f37-bc82-06a9a4b2470a.png)
위의 그림에서 네모칸들은 네트워크를 구성하는 엔티티이다.\
Docker 내부에 있는 네모는 모두 Docker 컨테이너이며 네모 안의 숫자는 사용하는 포트로서 "(외부포트) -> (내부포트)"의 형태로 나타냈다.
#### 3.3. 어플리케이션
![캡처](https://user-images.githubusercontent.com/62279820/195648177-6697feda-55ec-4341-ba8e-2ef27edc5fdf.PNG)
![캡처2](https://user-images.githubusercontent.com/62279820/195648184-9e4bb3f9-c53a-4834-a021-cc1a176e2435.PNG)
어플리케이션의 동작 화면은 위와 같다.\
왼쪽 화면의 동그란 아이콘을 터치하면 오른쪽의 화면이 나오도록 구현했다.
### 4. 소개 및 시연 영상

### 5. 설치 및 사용법
프로젝트를 설치하기 위해 먼저 git과 Docker를 사용할 수 있는 환경이어야 한다.\
git과 Docker를 설치했으면 원하는 디렉토리에서 아래의 명령어로 github의 repository를 복사한다.
```
$ git clone https://github.com/ParkYoonHyeong/Capstone-2022-1-30.git
```
