# 📈 TaeHyeong Kim

<p align="left">
  <!-- Core Language -->
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <!-- Data Frameworks -->
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <!-- AI / ML / LLM Frameworks -->
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=LangChain&logoColor=white" />
</p>

> **Software Engineer** specializing in **AI Systems & Quantitative Analysis**.
> 
> "데이터의 흐름 속에서 본질적인 문제를 발굴하고, AI 오케스트레이션과 효율적인 퀀트 알고리즘을 통해 신뢰성 높은 해결책을 구현합니다."

---

## 🎯 Focus Areas

* **Data Engineering & Analysis:** `pandas`와 `NumPy`를 활용한 금융·가상자산 시계열 데이터의 효율적인 전처리 및 전략 백테스팅 구현
* **AI Retrieval & Security:** LLM 시스템의 RAG(검색 증강 생성)를 위한 데이터 청킹 최적화 및 안정적인 프롬프트 보안 필터링 적용
* **Model Pipeline Integration:** 머신러닝 피처 엔지니어링 및 다양한 오픈소스 LLM 프레임워크를 연동한 모듈형 AI 파이프라인 흐름 구축

---

## 🧑‍💻 Selected Projects

### 🚀 [crypto-pilot](https://github.com/KTHYEONG/crypto-pilot)
> **가상자산 데이터 수집, 백테스팅 및 트레이딩 자동화 시스템**
> `Time-Series Pipeline` · `Vectorized Backtesting` · `pandas/NumPy` · `Docker`

* **Data Flow:** [거래소 API] -> [Rate Limit 준수 수집] -> [로컬 DB 적재] -> [Pandas 벡터화 백테스팅] -> [성과 지표 추출]
* **배경 & 도전 과제 (Problem & Challenge)**
  * 트레이딩 전략 검증을 위해 거래소 API로부터 방대한 시계열 데이터를 누수 없이 수집하고, 반복적인 전략 성과 분석(수익률, MDD 등) 계산 시 발생하는 연산 지연 병목 해결 필요
* **해결 방안 & 핵심 구현 (Key Implementations)**
  * **안정적인 수집 파이프라인 설계:** 가상자산 거래소 오픈 API의 제한 정책(Rate Limit)을 준수하고, 네트워크 예외 상황에서도 중단 없이 로컬 데이터베이스에 시계열 데이터를 적재하는 파이프라인 구현
  * **벡터 연산 기반 백테스팅 엔진:** 파이썬 루프문 대신 `pandas` 및 `NumPy` 벡터 연산을 적극 활용하여 전략 시뮬레이션의 속도를 극대화하고 핵심 투자 지표 검증 기능 탑재
  * **컨테이너 환경 자동화:** 일관된 구동 환경 및 배치 작업 관리를 위해 `Docker` 기반의 자동화 파이프라인 구축

---

### 🚀 [Witches-Chat-Core](https://github.com/Hyonso/Witches-Chat-Core)
> **LLM 인젝션 차단 및 지능형 RAG 데이터 처리 엔진**
> `RAG Data Pipeline` · `Prompt Security` · `LangChain` · `VectorDB`

* **Data Flow:** [문서 입력] -> [계층형 청킹 & Vector 적재] -> [질의 패턴 분석] -> [가드레일 검증] -> [안전한 컨텍스트 합성]
* **배경 & 도전 과제 (Problem & Challenge)**
  * 프로덕션 LLM 서비스 운영 시 데이터 전처리 품질에 따른 RAG 답변 왜곡(Hallucination) 현상과, 입력 데이터 조작을 통한 시스템 지시문 탈취 및 보안 우회(Prompt Injection) 리스크 대응 필요
* **해결 방안 & 핵심 구현 (Key Implementations)**
  * **프롬프트 보안 및 가드레일 설계:** 사용자 입력 데이터 파이프라인 단계에서 악의적인 주입 패턴과 우회 지시문을 정밀 사전 탐지 및 정제하는 런타임 보안 방어 시스템 개발
  * **지능형 RAG 데이터 파이프라인 설계:** 비정형 문서의 맥락을 보존하는 계층형 청킹(Chunking) 전략 수립 및 정밀 검색을 위한 벡터 데이터베이스 최적화 수행
  * **LangChain 오케스트레이션 설계:** 오남용 및 프롬프트 누출(Leakage)을 원천 차단하기 위해 원천 데이터와 시스템 가이드를 분리하고 정제된 컨텍스트만 안전하게 제공하도록 구성

---

### 🚀 [Emori](https://github.com/KTHYEONG/Emori)
> **한국어 감정 분석 및 맞춤형 공감 텍스트 생성을 위한 미세 조정(Fine-Tuning) 시스템**
> `🏆 2025년 한국정보기술학회 추계종합학술대회 동상 수상`
> `SLM Fine-Tuning` · `Sentiment Classification` · `PyTorch` · `scikit-learn`

* **배경 & 도전 과제 (Problem & Challenge)**
  * 텍스트 일기 데이터에서 사용자의 미세한 감정 상태를 다각도로 분류하고, 정밀하게 인지된 감정 맥락에 매끄럽게 호응하는 공감형 답변 문장을 유기적으로 생성해내는 결합 파이프라인 필요
* **해결 방안 & 핵심 구현 (Key Implementations)**
  * **감정 분류 및 생성 파이프라인 통합:** 텍스트에서 감정을 다중 레이블로 판별하는 감성 분석 모듈(`scikit-learn` 기반 머신러닝 분석)과, 도출된 감정 도메인에 기반해 자연스러운 위로 메시지를 출력하는 생성 모듈 간 유기적 흐름 결합
  * **소형 언어 모델(SLM) 파인튜닝:** 한국어 감정 대화 훈련 데이터셋을 수집 및 정제하고, 제한된 리소스 환경 내 효율적인 서빙을 위해 오픈소스 소형 모델(Llama3 7B 등)을 대상으로 지도 미세 조정(SFT) 수행
  * **안정성 중심의 데이터 파이프라인:** 예외적 입력(공백, 비정상 텍스트 패턴) 전처리 필터링을 구축하여 분류 정확도를 높이고 부적절한 대화 출력을 사전에 제어

---

## ✉️ Contact & Links

* **GitHub:** [@KTHYEONG](https://github.com/KTHYEONG)
* **Email:** `xogud3624@gmail.com`
