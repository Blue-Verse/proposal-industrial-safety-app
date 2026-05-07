# 산업 현장 안전 규정 정보 제공 앱 개발 — 제안 분석 로그

> 생성일: 2026-05-07
> 공고 URL: https://www.wishket.com/project/155139/

## 1. 공고 파싱 결과

```yaml
job:
  title: "산업 현장 안전 규정 정보 제공 앱 개발"
  category: "개발/디자인/기획 - 안드로이드/iOS/기타(IT 서비스 구축)"
  budget_range: "30,000,000원"
  duration: "90일"
  tech_stack:
    - AWS
    - express.js
    - Firebase Cloud Messaging
    - MySQL
    - Node.js
    - React Native
  description: "건설·제조 현장 근로자가 복잡한 안전 규정을 텍스트·음성·이미지로 검색하는 모바일 앱과 관리자가 교육 이수·일일 점검을 시스템화하여 기관 제출용 증빙으로 출력하는 통합 플랫폼"
  requirements:
    - "사용자 앱(Android/iOS): 로그인, 안전 규정 열람, 텍스트/음성/이미지 복합 검색, 일일 안전 점검(체크리스트+사진)"
    - "관리자 웹: 대시보드, 안전 규정 관리(HWP→텍스트, 키워드 태그), 교육 실적 관리, 점검 현황 조회, PDF 출력, 회원 관리"
    - "STT API 음성 검색"
    - "Vision AI 이미지 사물 인식 검색"
    - "FCM 푸시 알림"
    - "월 단위 유지보수 계약 가능 업체 우대"
  client_questions: []
  deadline: "2026-05-21"
  job_post_url: "https://www.wishket.com/project/155139/"
  urls: []
  images: []
```

## 2. URL/이미지 분석

공고 본문에 외부 참고 URL 및 첨부 이미지 없음 — 분석 단계 생략. 위시켓 공고 본문 텍스트만으로 요구사항이 충분히 정의되어 있음 (요구사항 정의서 보유 명시).

## 3. 실현 가능성 분석 (내부용)

- **프로젝트 유형**: 모바일 앱(RN) + 풀스택 웹 + 외부 AI API 연동 → "조건부 가능", 버퍼 +20%
- **기본 공수 산정** (AI 보조 없이):
  - 기획/설계: 8 M/D
  - UI/UX 디자인: 12 M/D
  - 모바일 앱(RN): 25 M/D
  - 관리자 웹: 12 M/D
  - 백엔드/외부 API/인프라: 27 M/D
  - QA/배포: 6 M/D
  - 합계: 90 M/D
- **AI 절감률 50% 적용**: 45 M/D
- **모바일+외부 API 버퍼 +20%**: 약 54 M/D
- **달력 일수 변환**: 54 × (7/5) = 약 75.6일 → 약 76일
- **클라이언트 예상 기간**: 90일
- **판정**: 클라이언트 90일 ≥ 산정 76일 → **클라이언트 기간 그대로 사용** (서두를 필요 없음, 외부 API 정확도 튜닝·스토어 심사 버퍼 확보)

클라이언트 노출용 공수표는 보수적으로 48 M/D로 산정 (1인 풀가동 기준 75일 수렴, 단가 약 562,500원/MD).

## 4. 포트폴리오 매칭

| 후보 | 매칭 점수 | 근거 |
|-----|---------|-----|
| Harmony Link | 9/10 | 모바일 앱 + 관리자 웹 + 외부 AI API + RBAC + 멀티테넌트 — 구조 100% 일치 |
| Pilates App | 9/10 | React Native + Node.js 정확 매치, 3 플랫폼 동시 출시 경험 |
| Connectin | 8/10 | OCR(이미지 인식) 외부 API 연동 → Vision AI 연동에 직접 적용, Express.js 정확 매치 |

**최종 선정 3개**: Harmony Link, Pilates App, Connectin

## 5. 최종 제안 요약

- **지원 금액**: 25,500,000원 (VAT 별도) — 클라이언트 예상 30,000,000원의 85%
- **지원 기간**: 90일 (Phase 1 기획·디자인 22일 / Phase 2A 백엔드·관리자 웹 28일 / Phase 2B 모바일·외부 API 22일 / Phase 3 QA·배포 18일)
- **핵심 제안 포인트**:
  1. 현장 친화적 복합 검색 UX (음성·이미지를 1차 진입 동선으로)
  2. HWP → 검색 가능 데이터 변환 파이프라인 (3종 검색 인덱스 일관성)
  3. 기관 제출용 PDF 증빙 자동화 (고용노동부 점검 대응)
  4. 요구 기술 스택 100% 일치(AWS+Express+RN+MySQL+FCM) + 월 단위 유지보수 계약 가능

## 6. 최종 산출물 (8단계 출력 전문)

### 6.1 제안서 사이트 URL

https://proposal-router.claude-ai-b27.workers.dev/proposal-industrial-safety-app/

### 6.2 지원 금액 (복사용)

```
25,500,000원
```

### 6.3 지원 기간 (복사용)

```
90일
```

### 6.4 클라이언트 질문 답변

공고에 별도 클라이언트 질문 없음 — 해당 없음.

### 6.5 지원 내용 (복사용)

```
안녕하세요, 산업 현장 안전 규정 정보 제공 앱 개발 프로젝트에 지원합니다.

본 프로젝트에 대한 상세 제안서(견적서, 공수계산서, PRD, 일정, 포트폴리오)를 별도 페이지로 준비하였습니다. 아래 링크에서 확인해 주시면 감사하겠습니다.
▶ 제안서 상세 페이지: https://proposal-router.claude-ai-b27.workers.dev/proposal-industrial-safety-app/
▶ 위시켓 포트폴리오: https://www.wishket.com/partners/p/blueverse1/

---

<프로젝트 진행 제안>

■ 프로젝트 분석
- 건설·제조 현장 근로자가 복잡한 안전 규정을 텍스트·음성·이미지 3종 검색으로 즉시 참조하는 모바일 앱과, 관리자가 교육 이수·일일 점검 데이터를 시스템화하여 고용노동부 등 기관 제출용 증빙으로 출력하는 통합 안전 관리 플랫폼을 90일 내 구축합니다.
- 핵심 차별 포인트: (1) 장갑·먼지·소음 환경에 적합한 음성·이미지 1차 진입 검색 UX, (2) HWP 규정 데이터 → 3종 검색 인덱스 일관성, (3) 기관 제출용 PDF 증빙 자동화, (4) 요구 기술 스택(AWS·Express·React Native·MySQL·FCM) 100% 일치.

■ 작업 일정

[Phase 1 — 기획·UI/UX 디자인] Day 1–22
- 요구사항 정의서 기반 상세 기획, IA·플로우, ERD·API 명세, UI 키트 및 전 화면 디자인, 외부 API(STT·Vision) 후보 검증

[Phase 2A — 백엔드·인프라·관리자 웹 코어] Day 23–50
- AWS 인프라(EC2/RDS/S3), Express API, 인증, 안전 규정 CRUD, 관리자 웹 핵심 기능 구축

[Phase 2B — 모바일 앱·외부 API 연동] Day 51–72
- React Native 사용자 앱(Android/iOS), STT 음성 검색·Vision 이미지 검색·FCM 푸시 통합, 일일 점검 사진 업로드

[Phase 3 — 통합 QA·배포·인수] Day 73–90
- E2E 테스트, 디바이스 호환성, Google Play·App Store 등록, 운영 환경 배포, 운영·관리자 매뉴얼

■ 마일스톤 및 산출물
- M1 (Day 22): 화면 설계서·디자인 승인, 외부 API 선정 완료
- M2 (Day 50): 관리자 웹 베타 — 규정·교육·점검 데이터 입력·조회
- M3 (Day 72): 모바일 앱 베타 — 텍스트·음성·이미지 검색·점검 제출
- M4 (Day 90): 정식 배포 — 스토어 등록, 운영 배포, PDF 출력 검증
- 최종 산출물: 기획 설계서(스토리보드), 디자인 원본 파일(Figma), 소스 코드 일체, API 명세·DB 스키마·운영 매뉴얼

■ 미팅 시 협의 필요 사항
- 외부 API 선정: STT(Google Cloud Speech-to-Text vs Naver Clova), Vision(Google Cloud Vision vs AWS Rekognition) — 비용·정확도 검증 후 결정
- HWP 규정 데이터의 1차 입력 범위 및 키워드 태그 정책
- 기관 제출용 PDF 양식 표준 (고용노동부 점검 시 요구 양식 사전 검토)
- AWS 계정 소유 주체 (클라이언트 직접 vs 위탁 운영) 및 월 호스팅·유지보수 계약 조건
- Google Play Console·Apple Developer Program 계정 보유 여부

---

<유사 프로젝트 진행 경험>

▶ 시니어 주간보호 관리 플랫폼 (2025, 약 6개월)
- 프로젝트 유형: B2B SaaS 헬스케어, 모바일 앱 + 관리자 웹 + AI 분석 멀티테넌트
- 핵심 기능: 케어 로그·투약 관리(현장 사진·체크리스트), 관리자 대시보드·통계·전자서명·증빙 출력, AI 건강 분석 외부 API 연동, RBAC 다단계 권한
- 유사점: 모바일 앱 + 관리자 웹 + 백엔드의 다중 플랫폼 구조, 현장 데이터(사진·체크리스트)를 모바일에서 입력하고 관리자 웹에서 통계·증빙으로 활용하는 흐름, 외부 AI API 연동 경험, 다중 역할 RBAC가 본 프로젝트와 매우 유사
- 기술 스택: Flutter, NestJS, Next.js, TypeScript, MySQL, AWS CDK, Docker

▶ 필라테스 프랜차이즈 관리 플랫폼 (2019.09–2019.12, 4개월)
- 프로젝트 유형: B2B2C 앱·O2O, 3 플랫폼 동시 출시
- 핵심 기능: 수업 예약·강사·출결·결제·CRM·커뮤니티, 본사·지점·강사·회원 4단계 권한, Android·iOS·Web 동시 출시
- 유사점: 요구 기술 스택(React Native + Node.js)과 정확히 일치, 모바일 앱과 관리자 웹을 동일 일정에 동시 출시한 경험, 다단계 권한(현장 관리자·근로자·시스템 관리자) RBAC 설계 경험
- 기술 스택: React Native, React, Node.js, JavaScript, MySQL

▶ 디지털 명함·네트워킹 플랫폼 (2025.05–2025.08, 3개월)
- 프로젝트 유형: B2B 플랫폼, 외부 API 다수 연동
- 핵심 기능: OCR 명함 이미지 인식·자동 입력, BLE 근거리 사용자 탐색, Express.js 마이크로서비스 63 API 엔드포인트
- 유사점: 이미지 인식 외부 API(OCR) 연동 경험은 본 프로젝트의 카메라 사물 인식(Vision AI) 연동에 그대로 활용 가능, Express.js 기반 API 서버 운영 경험, 모바일 카메라로 촬영 → 인식 결과를 검색에 활용하는 UX 패턴 동일
- 기술 스택: Flutter, Next.js, TypeScript, Express.js, PostgreSQL, Docker

---

<사용 기술과 툴>

▶ 개발 기술
- 모바일: React Native (Android·iOS 동시)
- 관리자 웹: Next.js + TypeScript
- 백엔드: Node.js + Express.js
- 데이터베이스: MySQL (AWS RDS)
- 인프라: AWS (EC2·RDS·S3·CloudFront·Route53)
- 푸시 알림: Firebase Cloud Messaging
- 외부 API: STT (Google Cloud Speech-to-Text 또는 Naver Clova), Vision (Google Cloud Vision 또는 AWS Rekognition)
- 컨테이너: Docker

▶ 개발 도구 및 인프라
- 버전 관리: GitHub
- CI/CD: GitHub Actions
- 클라우드: AWS
- 컨테이너: Docker

▶ 커뮤니케이션
- 일일 진행 공유: Slack 또는 카카오톡
- 주간 미팅: Zoom / Google Meet
- 문서 공유: Notion 또는 Google Docs
- 이슈 트래킹: GitHub Issues
```

### 6.6 관련 포트폴리오 추천 (위시켓 폼 입력용)

1. **시니어 주간보호 관리 플랫폼 (Harmony Link)** — 모바일 앱 + 관리자 웹 + 외부 AI API + RBAC + 멀티테넌트, 본 프로젝트와 구조 100% 일치
2. **필라테스 프랜차이즈 관리 플랫폼 (Pilates App)** — React Native + Node.js 정확 매치, Android·iOS·Web 3 플랫폼 동시 출시 경험
3. **디지털 명함·네트워킹 플랫폼 (Connectin)** — OCR 이미지 인식 외부 API 연동 경험 → Vision AI 연동에 직접 적용, Express.js 백엔드 정확 매치

