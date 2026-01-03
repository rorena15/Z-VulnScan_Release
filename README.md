# Z-Vuln Scan Professional Edition (v3.0.0)
### 🛡️ Next-Gen Network Asset Discovery & Topology Visualization

![Version](https://img.shields.io/badge/Version-v3.0.0_Professional-blue?style=flat-square) ![Python](https://img.shields.io/badge/Python-3.13+-3776AB?style=flat-square&logo=python&logoColor=white) ![GUI](https://img.shields.io/badge/GUI-PySide6_Dark-41CD52?style=flat-square&logo=qt&logoColor=white) ![License](https://img.shields.io/badge/License-Proprietary-red?style=flat-square)

**Z-Vuln Scan Professional**은 인가된 네트워크 환경에서 **자산 가시화, 서비스 포트 정밀 진단, 취약점 사전 점검**을 수행하는 전문가용 보안 도구입니다.

최신 **v3.0.0**에서는 **Deep Dark UI, 인터랙티브 네트워크 토폴로지 맵, 내장형 DB 매니저**가 추가되었으며, **Cython + PyArmor** 기술을 적용하여 보안성과 실행 성능을 극대화했습니다.

> **📢 v3.0.0 Major Update:**
> * **Topology Map:** 네트워크 자산 관계를 시각화하는 인터랙티브 HTML 맵 제공 (PyVis 엔진)
> * **New UI/UX:** 전문가용 Deep Dark 테마 및 통합 설정 대시보드
> * **Security:** Cython 컴파일 엔진 탑재로 분석 속도 향상
> * **DB Manager:** 스캔 이력 조회, 수정, 삭제가 가능한 통합 관리 도구 탑재

---

## 📑 목차 (Table of Contents)
1. [🔐 법적 고지 및 윤리 규정](#-legal--ethical-notice-중요)
2. [✨ v3.0.0 핵심 변경 사항](#-v300-whats-new)
3. [🚀 주요 기능](#-key-features)
4. [✅ 지원 진단 항목 (KISA)](#-supported-audit-list-kisa)
5. [🛠 기술 스택](#-technology-stack)
6. [🗓 로드맵](#-roadmap)
7. [📜 라이선스](#-license)

---

## 🔐 Legal & Ethical Notice (중요)

> ⚠ **[경고] 본 프로그램은 반드시 인가된 자산 및 네트워크 환경에서만 사용해야 합니다.**

- 본 도구는 **네트워크 자산 식별, 서비스 정보 수집, OS 설정 취약점 진단 기능**을 포함합니다.
- 사전 허가 없이 제3자의 네트워크 또는 시스템을 스캔하는 행위는 **정보통신망법 등 관련 법률**에 의해 **형사·민사 책임**이 발생할 수 있습니다.
- 사용자는 본 도구 사용에 따른 **모든 법적 책임을 스스로 부담**합니다.
- **실행 절차:** 프로그램 최초 실행 시, 위 사항에 대한 **법적 고지 동의(Disclaimer Dialog)** 과정을 거쳐야만 기능이 활성화됩니다.

---

## ✨ v3.0.0 What's New

### 🎨 1. 완전히 새로워진 Pro UI/UX
- **Deep Dark Theme:** 장시간 분석 업무에 최적화된 고대비 다크 모드 디자인 적용.
- **Unified Dashboard:** 탭 전환 없이 한 화면에서 타겟 설정, 인증, 포트 구성을 직관적으로 제어하는 통합 뷰.
- **Smart Feedback:** 상단 툴바(Toolbar) 도입 및 실시간 통계 현황판(Status Board) 배치.

### 🗺️ 2. 네트워크 토폴로지 맵 (Topology Map)
- **Interactive Graph:** 스캔된 자산을 노드 그래프로 시각화하여 네트워크 구조를 한눈에 파악.
- **Offline Ready:** 인터넷 연결 없이도 동작하는 독립형(Stand-alone) HTML 리포트 생성.
- **Detail View:** 자산 노드 클릭 시 IP, OS 정보, 사용자 메모(Tag) 즉시 확인.

### 🔐 3. 강력한 보안 및 성능 (Hybrid Obfuscation)
- **Cython Compiled Core:** 핵심 스캔 엔진(`core`, `utils`)을 C언어 레벨 바이너리(`.pyd`)로 컴파일하여 속도 향상.
- **PyArmor Protection:** 최신 난독화 기술을 적용하여 소스 코드 보호 및 무단 변조 방지.

### 📊 4. 통합 데이터 관리 (DB Manager)
- **Embedded Manager:** 별도 도구 없이 프로그램 내에서 스캔 이력 조회, 메모 수정, 데이터 삭제 가능.
- **Persistent Storage:** SQLite 기반의 로컬 저장소를 통해 스캔 결과 영구 보관.

---

## 🚀 Key Features

### 1. 📡 Network Asset Discovery
- **Native Ping Sweep:** OS 내장 명령어를 활용한 빠르고 안정적인 생존 호스트 탐지
- **OS Fingerprinting:** TTL 및 배너 분석을 통한 운영체제 식별
- **Dependency Free:** Npcap 등 별도 드라이버 설치가 필요 없는 Portable 환경

### 2. 🔍 Port Exposure Scanning
- **Flexible Modes:** Fast Scan (Top 1000), Full Scan (1-65535), Custom Range 지원
- **High Performance:** 멀티스레딩 아키텍처 기반의 고속 TCP Connect 스캔
- **Service Detection:** 활성 포트의 서비스 데몬 및 버전 정보 수집

### 3. 🛡️ Vulnerability Audit (Server Security)
- **Credential Audit:** SSH(Linux) / WinRM(Windows) 기반의 계정 및 설정 진단
- **KISA Compliance:** 주요 정보통신기반시설 기술적 취약점 분석 평가 가이드라인 준수
- **Auto Classification:** 운영체제(Windows/Linux) 자동 식별 후 맞춤형 스크립트 실행

### 4. 📄 Professional Reporting
- **PDF Report:** 경영진 보고용 요약 차트 및 상세 조치 가이드가 포함된 고품질 보고서
- **Excel Export:** 자산 관리 대장으로 활용 가능한 원시 데이터(Raw Data) 시트 제공
- **Visual Map:** 네트워크 구조도(HTML) 내보내기 지원

---

## ✅ Supported Audit List (KISA)

> ℹ **[참고]** 진단 기능은 대상 자산에 대한 **관리자 계정(SSH/WinRM)** 정보가 필요합니다.

### 🐧 Linux Server (Unix 계열) - 72 Items
| 코드 | 항목명 | 주요 점검 내용 |
|:---:|---|---|
| **U-01** | root 원격 접속 제한 | `sshd_config` 내 PermitRootLogin 설정 점검 |
| **U-02** | 패스워드 복잡성 설정 | `pwquality.conf` 등 암호 정책 설정 점검 |
| **U-54** | Session Timeout 설정 | 유휴 세션 자동 로그아웃 설정 여부 |
| ... | ... | (KISA 가이드라인 U-01 ~ U-72 지원) |

### 🪟 Windows Server - 80 Items
| 코드 | 항목명 | 주요 점검 내용 |
|:---:|---|---|
| **W-01** | Administrator 계정 이름 변경 | 기본 관리자 계정명 변경 및 비활성화 여부 |
| **W-36** | 화면 보호기 설정 | 화면 보호기 대기 시간 및 암호 설정 여부 |
| **W-60** | 최신 핫픽스 적용 | Windows 보안 업데이트 적용 상태 및 주기 점검 |
| ... | ... | (KISA 가이드라인 W-01 ~ W-80 지원) |

---

## 🛠 Technology Stack

- **Core:** Python 3.13+, Cython (Compiled Modules)
- **GUI:** PySide6 (Qt for Python), QWebEngineView
- **Visualization:** PyVis, NetworkX
- **Data:** SQLite3, OpenPyXL
- **Security:** PyArmor (Obfuscation), Keyring (Safe Storage)

---

## 🗓 Roadmap

### ✅ v3.0.0 (Current)
- [x] **New UI:** 전문가용 Deep Dark 테마 및 통합 설정 뷰
- [x] **Visualization:** PyVis 기반 네트워크 토폴로지 맵 구현
- [x] **Data Mgmt:** 내장 DB 매니저 및 메모(Tagging) 기능 추가
- [x] **Security:** 하이브리드 난독화(Cython+PyArmor) 빌드 시스템 구축

### 🔮 Future Updates
- [ ] **AI Analysis:** 스캔 결과에 대한 AI 기반 위험도 자동 분석 및 코멘트
- [ ] **Remote Agent:** 분산 네트워크 환경을 위한 에이전트 기반 스캔 지원
- [ ] **Scheduler:** 정기 점검을 위한 자동 예약 스캔 기능
- [ ] **SIEM Link:** Syslog/Webhook을 통한 관제 시스템 연동

---

---

## 🆘 트러블슈팅 및 필수 요구사항 (Troubleshooting)

**"Clean Install"된 Windows 환경에서 실행 시 아래 사항을 반드시 확인해주세요.**

### 1. 프로그램이 반응 없이 종료될 때 (MSVC Runtime)
개발 도구가 설치되지 않은 순정 Windows에서는 실행에 필요한 C++ 런타임 라이브러리가 없을 수 있습니다.
실행 시 오류 메시지가 뜨거나 무반응일 경우, 아래 Microsoft 공식 패키지를 설치해주세요.
* **Download:** [Microsoft Visual C++ Redistributable (x64) 최신버전](https://aka.ms/vs/17/release/vc_redist.x64.exe)

### 2. "액세스가 거부되었습니다" 또는 스캔 결과가 없을 때
본 도구는 패킷 레벨의 스캔을 수행하므로 **관리자 권한**이 필수입니다.
* **해결:** 실행 파일(`exe`) 우클릭 > **"관리자 권한으로 실행"** 선택

### 3. 백신 프로그램이 파일을 삭제하거나 차단할 때 (False Positive)
본 프로그램은 보안을 위해 소스 코드가 난독화(PyArmor)되어 있으며, 디지털 서명이 포함되지 않은 단독 실행 파일입니다.
이로 인해 **Windows Defender**나 백신이 이를 트로이 목마로 **오탐지**할 수 있습니다.
* **해결:** 백신 실시간 감시를 잠시 끄거나, 해당 파일을 **[검사 예외 항목]**으로 설정한 후 실행해주세요.
    > *Z-Vuln Scan은 사용자 PC에 어떠한 악성 행위도 하지 않음을 보증합니다.*

### 4. 화면이 하얗게 나오거나 맵이 안 뜰 때
구형 PC나 그래픽 드라이버가 설치되지 않은 가상 머신(VM)에서는 토폴로지 맵이 정상 작동하지 않을 수 있습니다.
* **해결:** 그래픽 카드 드라이버를 최신으로 업데이트하거나, 3D 가속 기능이 켜진 환경에서 실행해주세요.

---

## 📜 License

**Proprietary License**

Copyright © 2026 **Z-Vuln Scan Team**. All Rights Reserved.

본 소프트웨어는 **상용/비공개 소프트웨어**입니다. 저작권자의 사전 서면 허가 없이 본 소프트웨어의 전부 또는 일부를 무단으로 복제, 배포, 수정, 역공학하는 행위는 엄격히 금지됩니다.

*Built with open-source components: PySide6 (LGPL), PyVis (BSD), OpenPyXL (MIT).*
