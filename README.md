# 소한민 (Hanmin So) | Backend & AI Developer

## 🔗 Contact & Channels
* **Email:** world2013@naver.com
* **GitHub:** [https://github.com/starskein](https://github.com/starskein)

---

## 🎯 Portfolio Objective
> **"데이터와 아키텍처의 병목을 찾아내고 최적의 솔루션을 설계합니다."**
> 백엔드 시스템의 안정성과 AI 모델의 효율성을 동시에 고민하는 개발자 소한민입니다. C++ 기반의 로우레벨 성능 최적화 경험부터 LangGraph를 활용한 최신 AI Agent 설계까지, 기술의 경계를 넘나들며 실질적인 성능 향상을 이끌어내는 데 강점이 있습니다.

## 💡 Introduction
* **수치 기반의 성능 개선을 지향합니다.**
  * 졸업프로젝트에서 MPEG V-DMC 소프트웨어의 복잡도를 분석하여 부호화 속도를 11.4% 개선했으며, 이 과정에서 발생한 메모리 예외와 동기화 문제를 논리적으로 해결했습니다.
* **복잡한 워크플로우를 체계화합니다.**
  * 다중 모달 데이터가 혼재된 AI 교육 콘텐츠 생성 과정을 LangGraph 상태 그래프로 구조화하여 유지보수성과 확장성이 높은 시스템을 구축했습니다.
* **검증된 AI 역량을 보유하고 있습니다.**
  * AI 실무 활용 능력을 인증하는 **AICE Associate** 자격 취득을 통해, 데이터 해석부터 모델링 및 최적화까지의 전 과정을 능숙하게 수행할 수 있음을 증명했습니다.

## 🛠 Skills & Tools
* **Languages:** Python, C++
* **AI & Data:** Keras, Scikit-learn, LangChain, LangGraph, Pandas
* **DevOps & Tools:** Git, OpenMP, Valgrind, Intel Advisor, Gradio, SQL

---

## 💻 Projects

### 1. 다이나믹 메시 압축 소프트웨어 복잡도 분석 및 최적화 (졸업 프로젝트)
* **🔗 GitHub:** [3D-Mesh-Compression-Optimizer](https://github.com/starskein/3D-Mesh-Compression-Optimizer/tree/main)
* **기간:** 2024.02.15 – 2024.10.29 (9개월)
* **목표:** MPEG V-DMC 표준 소프트웨어의 복잡도 분석 및 최적화를 통한 부호화 속도 향상
* **사용 기술:** C++, OpenMP, Intel Advisor, Valgrind, Multithreading
* **핵심 성과:**
  * Intel Advisor 프로파일링을 통한 병목 구간 특정 및 OpenMP 병렬 처리 적용
  * 병렬화 과정의 `std::bad_alloc` 메모리 예외 및 Race Condition 해결 (`std::mutex` 및 `std::lock_guard` 활용)
  * **[성능 최적화]** 최종적으로 **압축 속도 약 11.4% 개선** 달성

### 2. LangGraph 기반 AI 교육 콘텐츠 자동 생성기
* **🔗 GitHub:** [LangGraph-AI-Edu-Generator](https://github.com/starskein/LangGraph-AI-Edu-Generator)
* **목표:** PPT 기반 맞춤형 강의 영상 및 요약본 자동 생성 파이프라인 구축
* **사용 기술:** Python, LangGraph, OpenAI API, SerpAPI, Gradio
* **핵심 성과:**
  * LangGraph 상태 그래프 기반의 '스크립트 생성 - RAG - 음성 합성' 워크플로우 설계
  * SerpAPI 연동을 통한 최신 지식 보완 및 Gradio 기반 웹 대시보드 구축

### 3. 항공사 고객 만족도 예측 (Airline Satisfaction Prediction)
* **🔗 GitHub:** [airline-satisfaction-prediction](https://github.com/starskein/airline-satisfaction-prediction)
* **목표:** 항공 고객 데이터를 분석하여 만족도 예측 모델 구축 및 운영 전략 수립
* **사용 기술:** Python, Pandas, Keras, Scikit-learn
* **핵심 성과:**
  * 재사용 가능한 엔드투엔드 전처리 모듈 개발 및 **정확도 0.93** 달성
  * 모델 재학습 전략별 성능 비교를 통해 최적의 유지보수 가이드라인 도출

---

## 🎓 Education & Credentials
* **KT 에이블스쿨 (KT AIVLE School) 9기** | AI/개발자 트랙 수료 예정
* **한양대학교 컴퓨터소프트웨어학 전공**
* **AICE Associate (AI Certificate for Everyone)** | 한국지능정보사회진흥원/KT 주관 취득
