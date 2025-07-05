# 👨‍💻 Portfolio – 정찬수

> Economic‑minded problem solver turned systems programmer – specialising in C‑based low‑latency back‑end & security‑conscious network software.

---

## 👋 About Me

경제학에서 훈련한 분석적 사고와 데이터 기반 의사결정 능력을 바탕으로 **시스템 프로그래밍 · 네트워크 보안 · 프랍 트레이딩 인프라**를 만드는 데 집중하고 있습니다. 42Seoul 공통 과정을 수료하며 C 언어로 운영체제 레벨 문제를 해결했고, Docker·Kubernetes 환경에서 배포 자동화와 성능 최적화 경험을 쌓았습니다.

* **Current goal** : 저지연(ultra‑low‑latency) 시스템 및 네트워크 보안 솔루션 엔지니어
* **Interests** : lock‑free 구조, order‑book simulation, eBPF, QUIC/HTTP 3, kernel optimisations

---

## 🔧 Tech Stack

|  Category              |  Tools                                                          |
| ---------------------- | --------------------------------------------------------------- |
| **Languages**          |  C / C++ / Python / JavaScript                                  |
| **Systems**            |  POSIX API, pthread, epoll/poll, shared‑memory, TCP/UDP sockets |
| **Frameworks & Infra** |  Django, Nginx, Docker, GitHub Actions, PostgreSQL              |
| **Tooling**            |  GCC/GDB, Valgrind, Make, Clang‑Tidy, Git Flow                  |

---

## 📂 Projects

### 🐚 Minishell *(2‑person team, C)*  `2024‑02 → 03`

Bash‑like 셸 구현 – `fork/execve`, 파이프 & 리디렉션, 시그널 처리, heredoc, 환경변수 파싱. **리눅스 시스템 콜** 흐름을 심층 학습하고 메모리·FD 누수를 **Valgrind** 및 자체 leak checker로 검증.

▶ [Source Code](https://github.com/FunctionPointerXDD/minishell)

---

### 🌐 Webserv *(3‑person team, C++)*  `2024‑11 → 2025‑01`

HTTP/1.1 웹 서버. Poll 기반 논블로킹 I/O, 가상 호스트, CGI (Python), 쿠키 기반 세션. Keep‑Alive & Chunked Transfer 구현 → **1500 req/s**@local VM. 

▶ [Source Code](https://github.com/FunctionPointerXDD/webserv)

---

### 🍴 Philosophers *(solo, C)*  `2024‑03 → 04`

Dining Philosophers 문제를 **스레드(mutex)** / **프로세스(semaphore)** 두 버전으로 구현. 비대칭 포크 획득 + 모니터 스레드로 **데드락·굶주림(starvation) 방지** 보장. 동기화 primitive 성능·정확도 비교 리포트 포함.

▶ [Source Code](https://github.com/FunctionPointerXDD/philosophers)

---

### 🏓 Real‑time Ping‑Pong Game *(5‑person, Django & WebSocket)*  `2025‑01 → 02`

8인 동시 경기, WebSocket 실시간 동기화, JWT + OTP 인증, Docker Compose 배포. CI/CD ( GitHub Actions → AWS EC2 ) 파이프라인 구축.

▶ [Source Code](https://github.com/FunctionPointerXDD/pingpong)
▶ [Demo Video](https://youtu.be/your-demo)

---

## 🏆 Highlights

* 42Seoul **Common Core** complete – 중급 시스템 프로그래밍 역량 공인
* Git Flow & PR Review 문화에서 25+ merge 경험
* Valgrind, perf, tcpdump 활용으로 **성능·안정성 문제** 해결 

---

## 📫 Contact

* **Email**   [kapustin4613@gmail.com](mailto:kapustin4613@gmail.com)
* **GitHub**  [FunctionPointerXDD](https://github.com/FunctionPointerXDD)
* **LinkedIn** [chansoo‑jung](https://www.linkedin.com/in/chansoo-jung-a73617331/)

---
