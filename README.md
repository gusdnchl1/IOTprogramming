# IoT Programming with Python 📡🐍

이 레포지토리는 **IoT 프로그래밍 수업에서 학습한 파이썬 코드와 과제, 실습 예제**를 정리·관리하기 위한 공간입니다.  
수업 진도에 맞추어 주차별로 디렉터리를 나누고, 각 주차별로 실습 코드와 정리 노트를 저장합니다.

---

## 🎯 목표 (Goals)

- 파이썬 기본 문법을 이해하고 IoT 프로젝트에 활용하기
- 센서/액추에이터와 연동 가능한 **파이썬 기반 IoT 코드 패턴** 익히기
- 주차별 실습을 체계적으로 기록하여 **개인 레퍼런스(cheat sheet)** 구축
- 최종적으로 간단한 **IoT 미니 프로젝트**를 완성할 수 있는 기반 만들기

---

## 🧰 개발 환경 (Environment)

- **Language**: Python 3.x
- **OS**: Windows / Linux / Raspberry Pi OS (수업 환경에 따라 수정)
- **추천 도구**
  - IDE / Editor: VS Code, PyCharm, Thonny 등
  - 버전 관리: Git + GitHub (또는 GitLab)

> ⚙️ 실제 사용 중인 파이썬 버전, 라이브러리, 보드(Raspberry Pi, Arduino + Python 등)가 정해지면 여기에 구체적으로 적어 주세요.

---

## 📁 레포지토리 구조 (Repository Structure)

> 예시이며, 수업 주차/내용에 맞게 변경하시면 됩니다.

```bash
.
├── week01_basic_python/
│   ├── variables.py          # 변수, 자료형 실습
│   ├── control_flow.py       # if, for, while 연습
│   └── README.md             # 1주차 정리 노트
├── week02_function_module/
│   ├── functions.py
│   ├── modules_import.py
│   └── README.md
├── week03_file_io/
│   ├── file_read_write.py
│   └── README.md
├── week04_iot_intro/
│   ├── gpio_example.py       # 예: 라즈베리파이 GPIO 제어
│   └── README.md
├── project/
│   ├── main.py               # 최종 미니 프로젝트 진입 파일
│   └── docs/                 # 설계 문서, 아이디어 정리
└── README.md                 # (이 파일)
