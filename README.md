# 👨‍💻 Portfolio – 정찬수

> Economic‑minded problem solver turned systems programmer

---

## 👋 About Me

 42Seoul에서 총 24개의 프로젝트를 수행하며 시스템 프로그래밍의 기초부터 실제 서버 구현까지 경험하였고, 문제 해결 능력과 협업 역량을 키웠습니다. 네트워크와 DevOps분야에 흥미가 많은 편입니다.

---

## 🔧 Tech Stack

| Category | Tools |
| :--- | :--- |
| **Languages** | C / C++ / Python / Java / Go |
| **Systems** | POSIX API, pthread, epoll/poll, TCP/UDP sockets |
| **Frameworks & Infra** | Django, FastAPI, React, Nginx, PostgreSQL, Redis, Docker, AWS, GitHub |
| **Tooling** | GCC/GDB, Valgrind, Makefile, Git Flow |
| **Protocols** | HTTP/1.1, WebSocket, REST API |
| **AI API** | Vertex AI (Gemini Vision API, Imagen3) |

---

## 📂 Projects

### 🐚 Minishell *(2‑person team, C)*  `2024‑02 → 03`

Bash와 유사한 셸을 구현했습니다. `fork/execve`, 파이프 & 리디렉션, 시그널 처리, heredoc, 환경변수 파싱을 모두 직접 적용하고 구현했습니다.  **리눅스 시스템 콜** 흐름을 심층 학습하고 메모리·FD 누수를 **Valgrind** 및 자체 leak checker로 검증했습니다. 크게 사용자 입력 파싱과 파싱된 명령어를 실행하는 부분으로 나누어서 프로젝트 진행하였는데 저는 실행부를 담당하였고 엣지 케이스까지 최대한 고려하여 완성하였습니다. 

▶ [Source Code](https://github.com/FunctionPointerXDD/minishell)

---

###  MiniRT *(2‑person team, C)*  `2024‑05 → 07`

레이 트레이싱(Ray-Tracing)을 구현해서 3D 도형(구, 원기둥, 평면, 원뿔, 질감)을 구현했습니다. 저는 필요한 파일을 파싱, 그리고 스레드를 CPU코어 수를 고려해서 생성하고 이미지를 분할하여 렌더링하였습니다. 그 덕분에 다수의 도형이 들어간 이미지의 기존 렌더링 시간이 1분이상 소요가 되었는데 7초 이내로 단축하는 경험을 했습니다.

▶ [Source Code](https://github.com/FunctionPointerXDD/miniRT)

---

### 🌐 Webserv *(2‑person team, C++)*  `2024‑11 → 2025‑01`

HTTP/1.1 웹 서버. Poll 기반 논블로킹 I/O, CGI (Python), 쿠키 기반 세션. Keep‑Alive & Chunked Transfer 구현했습니다. 그리고 Siege로 서버 부하 테스트를 하면서 성능 검증을 하였고 추가적인 최적화 작업을 통해 1MB이상의 파일을 읽는 요청에서 느려지는 부분을 개선하는 경험을 했습니다.

▶ [Source Code](https://github.com/FunctionPointerXDD/webserv)

---

### 🍴 Philosophers *(solo, C)*  `2024‑03 → 04`

Dining Philosophers 문제를 **스레드(mutex)** / **프로세스(semaphore)** 두 버전으로 구현했습니다. 교착상태(Deadlock)을 방지하기 위해 홀수번째와 짝수번째 철학자를 번갈아 가면서 진행시켰고(스레드 시그널 함수는 사용하지 않았습니다.) 굶주림(starvation)을 방지하기 위해 모니터링 스레드를 구현해서 철학자의 상태를 계속 체크했습니다. 스레드 방식의 시뮬레이션에서 200명의 철학자를 테스트 하면서 30분 동안 5ms 이내로 지연(delay)되지 않는 점도 확인했습니다.     

▶ [Source Code](https://github.com/FunctionPointerXDD/philo)

---

### 🏓 Real‑time Ping‑Pong Game *(5‑person, Django & WebSocket)*  `2025‑01 → 02`

탁구 게임 웹서비스를 구현했습니다. 최대 8인 토너먼트 방식으로 플레이가 가능하게 구현했으며 적용된 기능들은 다음과 같습니다.  -> WebSocket 실시간 동기화, JWT + 2FA인증, RESTful api, Docker Compose 배포.

▶ [Source Code](https://github.com/FunctionPointerXDD/42-ascension)

---

### 🗄️ PhoneBook Database *(solo, C/C++)*  `2024-07`

1만개 이상의 사용자 이름, 주소, 연락처를 저장할 수 있는 주소록을 구현했습니다.  벡터와 이진탐색으로 인덱싱 기능을 추가했고,  테스트를 통해 기본 쿼리와 인덱싱 적용 쿼리의 속도 차이 비교하여 최대 10배 차이가 발생하는 것을 확인했습니다.  

▶ [Source Code](https://github.com/FunctionPointerXDD/network_assignment)

---

### 🕵️‍♀️ Hidden Catch *(3‑person team, React & FastAPI)*  `2025-11 -> 12`

Google Gemini와 Imagen API를 활용해 사용자가 업로드한 이미지로 **틀린그림찾기 퀴즈를 자동 생성**하는 웹 게임입니다. **FastAPI**와 **Celery(Redis)**를 사용해 AI 이미지 생성 작업을 비동기로 처리함으로써 사용자 대기 시간을 효율적으로 관리했습니다. **React** 기반의 인터랙티브한 UI를 구현하고 **Docker Compose**와 **AWS(EC2, RDS, S3)**를 활용해 배포 자동화 및 서비스 운영 환경을 구축했습니다.

▶ [Source Code](https://github.com/FunctionPointerXDD/hidden-catch1)

---

### 🔐 MCP Gateway *(solo, Go & React)*  `2026‑04`

금융 도메인을 위한 **MCP(Model Context Protocol) 게이트웨이** PoC입니다. 다수의I에이전트가 은행 백엔드 서비스를 안전하게 호출할 수 있도록 중앙화된 라우팅·감사·권한 관리 인프라를 구현했습니다. 부서별 독립 VMCP 인스턴스로 접근 권한을 격리하고, 모든 툴 호출을 PostgreSQL에 기록합니다. 12개 이상의 목 MCP 서버(계좌·대출·외환·투자·컴플라이언스 등)를 구성하고, SSE 기반 실시간 대시보드와 긴급 툴 차단/허용 기능을 통해 운영 중 동적 도구 관리가 가능하도록 구현했습니다.

▶ [Source Code](https://github.com/FunctionPointerXDD/mcp-gateway)

---

## 스터디 활동

### 운영체제 스터디 `2024-04 -> 08`

Operting System Concepts 10th 원문을 학습 및 노션에 정리했습니다.(1,2장과 부록만 제외하고 모든 장 학습). 5개월간 8명의 팀원들과 함께 매주 목요일 마다 모여서 각자 맡은 분량을 발표 및 토의하였습니다. 이를 통해 컴퓨터 구조와 운영체제 전반에 대한 이론적 지식 습득할 수 있었습니다.

▶ [Notion](https://lean-taurus-898.notion.site/Operating-System-Concepts-10th-da775c8c55ec41e692534e5db02760a6?pvs=74)
piano Jung이라는 아이디로 활동

---

## 🏆 Highlights

* **이노베이션 아카데미 코디세이 텀 프로젝트 우수상** (2025.12) - *Hidden Catch 프로젝트*
* 42Seoul **Common Core** complete – 중급 시스템 프로그래밍 역량 공인
* Git Flow & PR Review 문화에서 25+ merge 경험
* Valgrind, tcpflow, siege 활용으로 **성능·안정성 문제** 해결 

---

## 📫 Contact

* **Email**   [kapustin4613@gmail.com](mailto:kapustin4613@gmail.com)
* **GitHub**  [FunctionPointerXDD](https://github.com/FunctionPointerXDD)
* **LinkedIn** [chansoo‑jung](https://www.linkedin.com/in/chansoo-jung-a73617331/)

---
