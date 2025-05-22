# 👨‍💻 Wojin Shin | Backend & AI Developer

> **문과 출신에서 Django Contributor로.**  
> 실전 프로젝트 중심으로 백엔드/AI 분야에 강점을 가진 개발자입니다.

---

## ✨ 핵심 요약

- 🧠 Django Contributor – [PR #19359](https://github.com/django/django/pull/19359)
- 💰 소비 예측 기반 건강기능식품 추천 시스템 개발
- 🎧 의뢰 기반 Discord 음악 봇 외주 제작
- 🧠 AI 모델 최적화 및 데이터 증강 경험 보유

---

## 🛠️ Tech Stack

**Back-End**: `Java`, `Spring Boot`, `Django`, `FastAPI`, `MySQL`, `Redis`  
**AI/ML**: `PyTorch`, `KoBERT`, `GRU`, `GPT API`, `Whisper`, `Scikit-learn`, `FAISS`  
**Infra**: `Docker`, `Jenkins`, `Linux`, `AWS S3`, `NGINX`  
**Front-End**: `React`, `Vue.js`, `Vite`, `TailwindCSS`, `Recoil`  
**Tools**: `Git`, `GitLab CI`, `Jupyter`, `Postman`, `Notion`, `Figma`

---

## 💼 프로젝트 경험

### 🏔️ Ollana - 등산 추천 및 페이스 메이커 어플 (삼성청년소프트웨어AI아카데미 자율 프로젝트)
**2025.04 ~ 2025.05 | Spring Boot + FastAPI + Flutter + Kotlin + Jenkins + Docker + Sonarqube**  
🔗 [GitHub 보기](https://github.com/zebra0345/Ollana)  

**🙋 역할**
- AI(100%) / Backend(25%) / Deploy(100%)
  - 사용자 설문 기반 맞춤 산 추천
  - 거리기반, 테마기반 맞춤 산 추천
  - Tensorflow 모델 기반 사용자 생체데이터 분석
  - 사용자 운동 형태 분석 및 조언 제공


**⚠️ Trouble Shooting**
- **데이터 불균형 문제** → SMOTE기법, 다운샘플링으로 샘플 균형 해소(저, 중, 고 = 1:6:1 이였던 것 1:1:1로)
- **모델 정확도, 과적합 문제** → 모델이 0, 1, 2 중 1에 해당하는 데이터에 과적합, Focal Loss로 클래스별 가중치 부여, early stop을 callback으로 사용, AdamW와 dropout 0.4로 Softmax 상승(정확도 40 ->75%)
- **K-means 클러스터링 문제** → 데이터 내부 이상치, 특히 제주도에 해당하는 산 데이터(한라산) 으로 인한 클러스터 오류, 데이터 전처리 작업을 통해 해결

### 💰 MMM – 소비 패턴 예측 플랫폼 (삼성청년소프트웨어AI아카데미 특화 프로젝트)
**2025.02 ~ 2025.04 | Spring Boot + FastAPI + KoBERT + GRU + Jenkins + Docker**  
🔗 [GitHub 보기](https://github.com/zebra0345/MMM)

**🙋 역할**
- AI(100%) / Backend(20%) / Deploy(10%)
  - 소비자 소비 이력을 분석하여 건강기능식품을 추천하는 AI 플랫폼
  - GRU 기반 소비패턴 예측, FAISS로 유사 소비자 검색 최적화
 
  
**⚠️ Trouble Shooting**
- **모델 학습 시간 증가** → FAISS 기반 벡터 인덱싱 도입  (인덱싱 도입으로 시간복잡도 O(1)로 감소)
- **데이터 부족** → Sliding window로 소비 데이터 증강  
- **소비 태그 자동 분류 정확도 문제** → KoBERT tokenizer만 가져와서 직접 모델 구성

---

### 🎧 Discord 음악봇 (외주 프로젝트)
**2025.04 | Python + FastAPI + Discord.py + Docker**  
🔗 [GitHub 보기](https://github.com/zebra0345/bot_sample.git)

**🙋 역할**
- AI(100%) / Backend(100%)
  - 실 사용자 기반 음악 큐 요청 → 스트리밍 봇 구현
  - Ollama 기반 장르 분석 + FastAPI 분산 처리 설계

**⚠️ Trouble Shooting**
- **봇 Block 현상** → FastAPI로 음악 전처리 API 분리  
- **자원 미해제** → 종료 시 리소스 초기화 함수 수동 설계  
- **대량 동시 접속 문제** → 메시지 큐 방식으로 비동기 처리 구현

---

### 🗣 DreamMoA – AI 화상 스터디 플랫폼 (삼성청년소프트웨어AI아카데미 공통 프로젝트)
**2024.01 ~ 2024.02 | FastAPI + GPT + GRU + YOLOv8 + React**  
🔗 [GitHub 보기](https://github.com/zebra0345/dream_project)


**🙋 역할**
- AI(100%) / Backend(50%)
  - 실시간 집중도 분석, 요약, 자막 제공 플랫폼
  - GPT 요약, Whisper 자막, GRU 집중도 분석 적용


**⚠️ Trouble Shooting**
- **LSTM 과부하 문제** → GRU 모델로 변경  
- **성별 편향** → 여성 데이터 수집 후 재학습  
- **정규화 문제** → 이중 정규화 제거 및 표준화 방식 변경

---

### 💳 금융상품 추천 웹 서비스 (삼성청년소프트웨어AI아카데미 관통 프로젝트)
**2024.11 | Django + Vue.js + GPT API**  
🔗 [GitHub 보기](https://github.com/zebra0345/finSetProject)

**🙋 역할**
- Backend(100%) / Frontend(10%)
  - 금융 성향 분석을 통한 상품 추천 서비스
  - 카카오맵 및 소셜로그인 연동

  
**⚠️ Trouble Shooting**
- **HTTPS 미연동으로 인한 카카오 API 오류** → HTTPS 인증 및 Callback URL 수정  
- **DB 정규화 문제** → 회원, 예금, 적금 테이블 분리로 해결

---

### ☀️ SolarBEMS – 태양광 발전 IoT 모니터링 (스마트그리드 IoT 융합 SW 전문가 과정 중간프로젝트)
**2023.12 ~ 2024.01 | Java + Flask + Spring Boot**  
🔗 [GitHub 보기](https://github.com/2023-SMHRD-KDT-IOT-4/SolarBEMS)

**🙋 역할**
- Backend(50%) / Frontend(50%)
  - 태양광 데이터 수집 → 사용자 시각화 시스템
  - 반응형 프론트엔드 구현

  
**⚠️ Trouble Shooting**
- **아두이노 연동 오류** → 모델 교체  
- **회로 불량** → 브레드보드 재설계

---

### 💊 건강기능식품 추천 시스템 (기업연계)
**2024.02 ~ 2024.03 | Spring + Flask + KNN + Clustering**  
🔗 [GitHub 보기](https://github.com/2023-SMHRD-KDT-IOT-4/yeahaRepo)

**🙋 역할**
- AI(80%) / Backend(30%)
  - 생애주기 + 건강검진 데이터를 기반으로 건강기능식품 추천
  - 군집 내 주요 질병 특징 기반 추천 로직 구현(KNN)


**⚠️ Trouble Shooting**
- **분류 정확도 낮음** → 특히 당뇨군에서 30% 정확도 -> 인자 재설계, 파라미터 튜닝으로 75 ~ 80% 까지 상승  
- **설문 기반 데이터 편향** → 설문 검증 로직 강화

---

### 🎥 영화 추천 시스템 (토이 프로젝트)
**2024.04 | Python + NLP**  
🔗 [GitHub 보기](https://github.com/zebra0345/movie.git)

**🙋 역할**
- AI(100%)
  - 줄거리 기반 코사인 유사도 추천 시스템


**⚠️ Trouble Shooting**
- **제목 중심 토크나이저 정확도 편차** → 고정된 tokenizer로 저장 후 재활용  
- **유사도 기준 모호** → 코사인 유사도로 유사 작품 판단 기준 명확화

---

## 🎓 이력 요약

- 삼성 청년 소프트웨어 아카데미 (SSAFY) 수료 중 (2024~)  
- 스마트그리드 IoT 융합 SW 전문가 과정 수료 (2023~2024)  
- 이글이비전 인턴 (2024.04 ~ 2024.05)

---

## 📫 Contact

[![Email](https://img.shields.io/badge/zebra0345@naver.com-D14836?style=flat)]()
