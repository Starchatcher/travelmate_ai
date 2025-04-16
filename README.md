# ✈️ TravelMate_AI

**AI 기반 맞춤형 여행 일정 추천 서비스**  
사용자의 감정, 예산, 여행 스타일 및 실시간 정보를 기반으로 여행 일정을 자동 생성하고 추천하는 대화형 웹 애플리케이션입니다.

---

## 🔧 프로젝트 개요

- **프로젝트명**: TravelMate_AI
- **개발기간**: 2025.03 ~ 진행 중
- **주요기능**:
  - AI 기반 여행 일정 추천 (날씨/감정 기반)
  - 실시간 예약 연동 (숙소, 교통 등)
  - 사용자 감정분석 및 추천 로그 기록
  - 커뮤니티 기반 후기, QnA, 찜하기 기능
  - 관리자 모드 및 통계 대시보드 제공

---

## 🧩 기술 스택

| 영역         | 사용 기술                                         |
|--------------|--------------------------------------------------|
| **Frontend** | React, TypeScript, HTML5, CSS3, Figma            |
| **Backend**  | Java 21, Spring MVC, MyBatis, REST API           |
| **Database** | Oracle 11g (ERD 26개 테이블)                     |
| **AI Module**| Python (Flask, pandas, scikit-learn 등)          |
| **Infra**    | AWS EC2, Nginx, GitHub Actions (CI/CD), Docker   |
| **API 연동** | Kakao Map, Weather API, 공공데이터 API 등        |

---

## 📁 프로젝트 구조

```
TravelMate_AI/
│
├── backend/             # Spring MVC + MyBatis 백엔드 서버
├── frontend/            # React + TypeScript 프론트엔드
├── ai/                  # Python 기반 Flask AI 모듈
├── docs/                # 기획서, ERD, 기술서, 보고서 등
├── sql/                 # TravelMate_AI.sql, insert.sql 등
└── README.md            # 프로젝트 소개 문서
```

---

## 📦 주요 기능 요약

| 기능 영역       | 설명 |
|----------------|------|
| 여행일정 추천  | 감정, 지역, 날씨 등 기반 맞춤 추천 |
| 예약 시스템     | ERP형 예약 통합 관리 (숙소/렌터카/관광) |
| 게시판 & 찜하기 | 자유게시판, QnA, 찜 기능 포함 |
| 관리자 기능     | 관리자 전용 답변, 신고 처리, KPI 확인 |
| AI 분석/기록    | 추천 로그, 감정 태깅, 피드백 수집 |

---

## 📌 ERD / 데이터 구조

- 총 26개 테이블
- ERD 및 전체 SQL 스크립트는 `/docs` 또는 `/sql` 폴더 참조  
  → `TravelMate_AI.sql` / `ERD_완성본_관계상세.dbml`

---

## 🛠️ 설치 및 실행 방법

### 1. 백엔드 실행 (Spring Boot)

```bash
cd backend
./gradlew bootRun
```

### 2. 프론트엔드 실행 (React)

```bash
cd frontend
npm install
npm start
```

### 3. AI 모듈 실행 (Flask)

```bash
cd ai
python app.py
```

---

## 👤 개발자

- **정세현**  
  한국 ICT 인재개발원 / AI 웹서비스 개발자 과정  
  Github: [github.com/sehyeon](https://github.com/sehyeon)  
  이메일: sehyeon@example.com

---

## ⭐ 기타

- Oracle SQL Developer 사용
- ERD & 테이블 DDL: `docs/TravelMate_AI_테이블리스트_및_기술서.xlsx`
- 실제 EC2 서버 배포 예정 (AWS + Nginx + Oracle 연동 테스트 완료)