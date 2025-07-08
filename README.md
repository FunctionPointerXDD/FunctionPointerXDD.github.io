# 👨‍💻 Portfolio – 정찬수

> Economic‑minded problem solver turned systems programmer

---

## 👋 About Me

이것저것 세상 모든 것에 호기심이 많은 사람입니다. 남들이 다 아는 사실이더라도 다른 관점으로 보거나 본질을 찾으려고 노력합니다. 경제학을 전공했지만 IT에도 관심이 많아 독학을 하다가 42Seoul이라는 교육기관을 통해서 개발자가 되기로 마음 먹었습니다. 끝없이 공부해야 한다는 점이 매력적인 직업이라고 생각합니다. 

* **Current goal** : 저지연(ultra‑low‑latency) 시스템 및 네트워크 보안 솔루션 개발자
* **Interests** : lock‑free , HPC, Golang, Compiler, Assembly 

---

## 🔧 Tech Stack

|  Category              |  Tools                                                          |
| ---------------------- | --------------------------------------------------------------- |
| **Languages**          |  C / C++ / Python / Java                                        |
| **Systems**            |  POSIX API, pthread, epoll/poll, TCP/UDP sockets                |
| **Frameworks & Infra** |  Django, Nginx, Docker, GitHub, PostgreSQL                      |
| **Tooling**            |  GCC/GDB, Valgrind, Makefile, Git Flow                          |

---

## 📂 Projects

### 🐚 Minishell *(2‑person team, C)*  `2024‑02 → 03`

Bash‑like 셸 구현 – `fork/execve`, 파이프 & 리디렉션, 시그널 처리, heredoc, 환경변수 파싱. **리눅스 시스템 콜** 흐름을 심층 학습하고 메모리·FD 누수를 **Valgrind** 및 자체 leak checker로 검증.

▶ [Source Code](https://github.com/FunctionPointerXDD/minishell)

---

### 🌐 Webserv *(3‑person team, C++)*  `2024‑11 → 2025‑01`

HTTP/1.1 웹 서버. Poll 기반 논블로킹 I/O, CGI (Python), 쿠키 기반 세션. Keep‑Alive & Chunked Transfer 구현 → **1500 req/s**@local VM. 

▶ [Source Code](https://github.com/FunctionPointerXDD/webserv)

---

### 🍴 Philosophers *(solo, C)*  `2024‑03 → 04`

Dining Philosophers 문제를 **스레드(mutex)** / **프로세스(semaphore)** 두 버전으로 구현. 비대칭 포크 획득 + 모니터 스레드로 **데드락·굶주림(starvation) 방지** 보장. 동기화 성능·정확도 비교.

▶ [Source Code](https://github.com/FunctionPointerXDD/philo)

---

### 🏓 Real‑time Ping‑Pong Game *(5‑person, Django & WebSocket)*  `2025‑01 → 02`

8인 동시 경기, WebSocket 실시간 동기화, JWT + 2FA인증, 유저 프로필, 통계 대시 보드, Docker Compose 배포.

▶ [Source Code](https://github.com/FunctionPointerXDD/42-ascension)

---

### 🗄️ PhoneBook Database *(solo, C/C++)*  `2024-07`

1만개 이상의 사용자 이름, 주소, 연락처를 저장할 수 있는 주소록 구현. 벡터와 이진탐색으로 인덱싱 구현. 테스트를 통해 기본 쿼리와 인덱싱 적용 쿼리의 속도 차이 비교. 

▶ [Source Code](https://github.com/FunctionPointerXDD/network_assignment)

---

## 운영체제 스터디 `2024-04 -> 08`

Operting System Concepts 10th 원문을 학습 및 노션에 정리(1,2장과 부록만 제외하고 모든 장 학습). 5개월간 8명의 팀원들과 함께 매주 목요일 마다 모여서 각자 맡은 분량을 발표 및 토의함. 컴퓨터 구조와 운영체제 전반에 대한 이론적 지식 습득.
▶ [Notion](https://lean-taurus-898.notion.site/Operating-System-Concepts-10th-da775c8c55ec41e692534e5db02760a6?pvs=74)

---

## 🏆 Highlights

* 42Seoul **Common Core** complete – 중급 시스템 프로그래밍 역량 공인
* Git Flow & PR Review 문화에서 25+ merge 경험
* Valgrind, tcpflow, siege 활용으로 **성능·안정성 문제** 해결 

---

## 📫 Contact

* **Email**   [kapustin4613@gmail.com](mailto:kapustin4613@gmail.com)
* **GitHub**  [FunctionPointerXDD](https://github.com/FunctionPointerXDD)
* **LinkedIn** [chansoo‑jung](https://www.linkedin.com/in/chansoo-jung-a73617331/)

---
