# 👨‍💻 Wojin Shin's GitHub Portfolio

> **문과 출신에서 Django Contributor로.**  
> **실제 서비스 운영 경험과 오픈소스 기여를 바탕으로, 기술을 실용적으로 다루는 백엔드 & AI 개발자입니다.**

---

## ✨ 요약

- 🧠 **Django 공식 기여자** – [PR #19359](https://github.com/django/django/pull/19359)  
- 💰 **소비 예측/저축 유도 플랫폼 MMM** – KoBERT 검색 + GRU 예측 기반 소비 분석 및 태깅  
- 🎧 **의뢰 기반 Discord 음악봇 제작** – FastAPI + OLLAMA 장르 분석 + Docker로 운영 안정성 확보  

---

## 🛠️ Tech Stack

### 📦 Back-end  
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat&logo=spring-boot&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=django&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)

### 🧠 AI / ML  
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![KoBERT](https://img.shields.io/badge/KoBERT-%23121011?style=flat&logo=python&logoColor=white)
![GPT API](https://img.shields.io/badge/GPT_API-412991?style=flat&logo=openai&logoColor=white)
![Whisper](https://img.shields.io/badge/Whisper-000000?style=flat&logo=openai&logoColor=white)
![Cosine Similarity](https://img.shields.io/badge/Cosine%20Similarity-%23121011?style=flat&logo=python&logoColor=white)

### 🧱 Infra  
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat&logo=jenkins&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![AWS S3](https://img.shields.io/badge/AWS%20S3-569A31?style=flat&logo=amazons3&logoColor=white)

### 💻 Front-end  
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat&logo=vue.js&logoColor=white)

### 🧰 Dev Tools  
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-FCA121?style=flat&logo=gitlab&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white)

---

## 💼 대표 프로젝트

### 💰 MMM – 무조건 모으는 머니  
**2025.02 ~ 2025.04 | Spring Boot + FastAPI + GRU + KoBERT + Jenkins + Docker**  
> AI 기반 소비 패턴 분석 및 예측 플랫폼

- **소비 데이터 전처리 및 토큰화**  
  : SK KoBERT 토크나이저를 이용해 약 2,000만 건의 소비 데이터를 단어 단위로 토큰화하고 임베딩 벡터 생성  
- **FAISS Index 압축 적용**  
  : 임베딩된 상호명 데이터를 FAISS로 압축하여 검색 속도 O(1) 구현, 시스템 효율 향상  
- **소비 예측 모델 설계**  
  : GRU 모델을 사용해 시계열 소비 내역 예측, 슬라이싱 윈도우 기법을 통해 데이터 증강  
  : MSE, RMSE 기준 0.대 성능 확보  
- **Spring Boot ↔ FastAPI 연동 설계**  
  : AI 예측 서버(FastAPI)와 백엔드(Spring Boot) 간 REST API 통신 구조 설계  
- **CI/CD 자동화**  
  : Jenkins + Docker 기반으로 서비스 전체 파이프라인 자동화

🔗 [GitHub 보기](https://github.com/zebra0345/MMM)

---

### 🎧 Discord 고기능 음악 봇  
**2025.04 | Python + FastAPI + Discord.py + Docker**  
> 실 사용자 의뢰 기반 음악 봇 개발

- **비동기 음악 예약/전처리 서버 구성**  
  : FastAPI 기반 서버에서 YouTube 메타데이터를 비동기 처리, Discord.py와 기능 분리하여 서버 부하 분산  
- **사용자 맞춤 기능 탑재**  
  : 재생목록 큐, 무한 반복 모드, 상태 메시지 업데이트 등 요청 기반 기능 구현  
- **OLLAMA 모델 기반 음악 장르 분류**  
  : 사용자가 등록한 음악에 대해 장르 자동 분류 후 큐 자동 삽입  
- **Docker 컨테이너 분리 배포**  
  : 음악 봇과 백엔드를 Docker로 분리해 안정적 운영 환경 구성

🔗 [GitHub 보기](https://github.com/zebra0345/bot_sample.git)

---

### 🧑‍💻 Django 오픈소스 기여  
**2024.04 | Django 공식 저장소 PR 반영 – [PR #19359](https://github.com/django/django/pull/19359)**  
> Django 5.1 릴리즈 반영: ASGIHandler의 비동기 처리 개선

- `ASGIHandler.read_body()`의 동기 처리 문제 해결  
  : Rollover 발생 시에도 비동기 write 처리를 적용하여 메모리 → 스레드 전환 지연 문제 제거  
- `python-stattle`, `gettar` 사용해 스레드풀 처리 구현  
- **관련 테스트 케이스 작성 및 코드 리팩토링**

---

### 🎥 영화 추천 알고리즘  
**2024.04 | Python + NLP**  
> 줄거리 기반 콘텐츠 유사도 추천 시스템

- 줄거리, 작가명을 KoBERT 기반 토큰화  
- 전체 DB에 대해 코사인 유사도 계산 → 가장 유사한 영화 리스트 반환

🔗 [GitHub 보기](https://github.com/zebra0345/movie.git)

---

### 🗣 DreamMoA – AI 화상 스터디 플랫폼  
**2024.01 ~ 02 | FastAPI + GPT + Whisper + OpenCV**  
> 실시간 화상 수업에서 자막, 요약, 집중도 분석을 제공하는 플랫폼

- **Whisper 모델 기반 실시간 자막 추출**  
- **OpenCV 기반 자세 추적 → 집중도 분석**  
  : 눈동자, 고개, 팔꿈치 위치 기반으로 사용자 집중도 판단  
- **GPT 기반 회의 요약 기능**  
  : 수업 종료 후 자동 스크립트 요약 리포트 제공

🔗 [GitHub 보기](https://github.com/zebra0345/dream_project)

---

### 💳 금융상품 추천 시스템  
**2024.11 | Django + GPT API + Vue.js**  
> 사용자 성향 기반 금융상품 추천 웹 서비스

- 사용자 성향은 GPT API를 활용해 분석  
- 현재 가입 상품 기반 유사 상품 추천 (rule-based 방식)  
- 전체 백엔드 로직 개발 및 프론트 일부 구현 (지도 연동 포함)

🔗 [GitHub 보기](https://github.com/zebra0345/finSetProject)

---

### ☀️ SolarBEMS  
**2023.12 ~ 2024.01 | Java + Flask**  
> 태양광 발전 시스템의 IoT 모니터링 및 사용자별 시각화

- 회원 로그인/관리 기능 구현 및 DB 설계  
- 사용자에 따라 대시보드 구성 변경  
- 대시보드 초기 디자인 및 구현 주도

🔗 [GitHub 보기](https://github.com/2023-SMHRD-KDT-IOT-4/SolarBEMS)

---

### 💊 건강기능식품 추천 시스템  
**2024.02 ~ 03 | Spring + KNN + 클러스터링**  
> 생애주기, 건강검진 정보 기반 건강기능식품 추천

- 설문을 통해 수집된 생활 패턴을 기반으로 KNN 분류  
- 비슷한 환자 군집에서 주요 영양소 추출 후 관련 건강식품 추천

🔗 [GitHub 보기](https://github.com/2023-SMHRD-KDT-IOT-4/yeahaRepo)

---

## 🎓 이력 요약

- 삼성 청년 소프트웨어 아카데미 (SSAFY, 2024~)  
- 스마트그리드 IoT 융합 SW 전문가 과정 수료 (2023~2024)  
- 이글이비전 프로 (2024.04 ~ 05)

---

## 📫 Contact

[![Email](https://img.shields.io/badge/zebra0345@naver.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:zebra0345@naver.com)  
[![GitHub](https://img.shields.io/badge/GitHub-zebra0345-181717?style=flat&logo=github)](https://github.com/zebra0345)

---

> 💬 기술은 문제를 푸는 도구라고 믿습니다.  
> 실용적인 구현력과 커뮤니케이션 능력을 바탕으로, **팀에 꼭 필요한 개발자**가 되겠습니다.
