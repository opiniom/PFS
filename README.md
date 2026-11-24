# PNS (Personal Net-worth & Spending)

**동명대학교 인공지능응용학과** Java 웹 프로그래밍 기말 프로젝트로 개발 예정인 **AI 목표 코칭 기반 반응형 웹 가계부 서비스**입니다.  
가계부의 모든 기본 기능을 PC·모바일 반응형 웹으로 제공하며, **목표(금액·차·건물) 및 기간(10개월·1년·10년) 기반 AI 달성 가능성·월 저축액 플래너**와 **실시간 AI 과소비 잔소리** 기능을 핵심 차별점으로 제공합니다.

> 현재 **기획 및 중간 발표 준비 단계**입니다. 실제 구현 코드는 중간 발표 이후 순차적으로 업로드됩니다.

## 핵심 기능
### 기본 가계부 (Core Ledger)
- **회원 관리**: Spring Security 기반 회원가입, 로그인/로그아웃
- **수입·지출 & 고정지출 관리**: 거래 내역 CRUD, 반복 고정지출 관리, 다중 조건 검색·필터링
- **캘린더 & 대시보드**: 월별 총 수입·지출·저축 요약 및 일별 내역 조회
- **통계 시각화**: Chart.js 기반 카테고리별 지출 비율 및 월별 추이 그래프
- **예산 관리**: 월별 목표 예산 설정 및 초과 경고

### 핵심 차별점 (AI 재무 코치 & 일일 정산)
- **맞춤 시간 일일 정산 & 미정산 이월 (지속성·편리성)**: 사용자가 정한 시간에 하루의 수입·지출 용도를 한 번에 확인·정산하며, 놓친 날의 미정산 내역은 다음 날 정산 시간에 자동으로 모아 일괄 정산
- **AI 목표 시뮬레이터**: 목표(금액, 내 차, 건물 등)와 기간(10개월, 1년, 10년 등)을 입력하면 달성 가능성(%)과 매월 권장 저축액, 절약 전략을 AI가 산출·제안
- **AI 과소비 잔소리**: 예산 초과나 목표 저축 페이스 이탈 시, 설정한 목표와 연결해 현실적이고 유쾌한 잔소리/코칭 피드백 제공

## 기술 스택
- **Backend**: Java 17, Spring Boot 3.x, Spring MVC, Spring Security, Spring Data JPA
- **AI Integration**: LLM API (Gemini API 등) + Java 재무 계산 하이브리드 엔진
- **Frontend**: Thymeleaf, HTML5, CSS3, JavaScript (ES6+), Bootstrap 5, Chart.js
- **Database**: H2 (개발용) / MySQL 8.0 (시연·운영용)
- **Build & Tools**: Gradle, Git & GitHub

## 문서 및 산출물
- 프로젝트 기획서: [docs/PLAN.md](docs/PLAN.md)
- 중간 발표 자료(PPT): [docs/presentation/PNS_중간발표.pptx](docs/presentation/PNS_중간발표.pptx)

## 팀원 (동명대학교 인공지능응용학과)
- **변의겸**: Backend Core, DB/JPA 설계, Spring Security 인증, AI 목표 시뮬레이터 & 과소비 잔소리 연동
- **차승제**: 반응형 UI/UX (Bootstrap 5 + Thymeleaf), 수입·지출/고정지출 CRUD, 캘린더, Chart.js 통계 시각화
