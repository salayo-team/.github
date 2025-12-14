# 🌍 LocalLife — 로컬 기반 AI 적성 추천 체험 플랫폼

<div align="center">

<img width="2839" height="1435" alt="Local_Life_UI_Image" src="https://github.com/user-attachments/assets/0b4e4aa4-7fa8-4e52-8c2c-893ad7ab3f02" />

### **2025 KDT 해커톤 참가작 · 예선 진출팀 (Salayo Team)** 

청년과 로컬 크리에이터를 연결하는 AI 기반 적성 추천 및 지역 체험 서비스

![Hackathon](https://img.shields.io/badge/2025%20KDT%20해커톤-예선진출-blue)
![Status](https://img.shields.io/badge/Status-MVP%20Complete-success)
[![기간](https://img.shields.io/badge/프로젝트_기간-2025.06.20~2025.12.20-green?style=flat)]()
[![license](https://img.shields.io/badge/license-Salayo%20Custom%20License-blue)](https://github.com/salayo-team/local-life-backend/blob/main/LICENSE)

📎 [ERD 전체 보기](https://www.erdcloud.com/d/yiwNwJeESMSkuQD9A)
📎 [API 명세서 (Swagger)](https://salayo-team.github.io/locallife-api-docs/api-docs.html)
📎 [요구사항 명세서 (SRS)](https://github.com/salayo-team/local-life-backend/blob/develop/.github/docs/software-requirements-specification.pdf)

</div>

---

## 📑 목차

<a href="#-서비스-개요-overview">
  <img src="https://img.shields.io/badge/서비스_개요-424242?style=for-the-badge" />
</a>

<a href="#-프로토타입-prototype">
  <img src="https://img.shields.io/badge/프로토타입-616161?style=for-the-badge" />
</a>

<a href="#-기획-배경--목표">
  <img src="https://img.shields.io/badge/기획_배경_&_목표-757575?style=for-the-badge" />
</a>

<a href="#-요구사항-명세-srs">
  <img src="https://img.shields.io/badge/요구사항_명세-9E9E9E?style=for-the-badge" />
</a>


<a href="#-사용자-흐름-요약-user-flow-overview">
  <img src="https://img.shields.io/badge/사용자_흐름-616161?style=for-the-badge" />
</a>


<a href="#%EF%B8%8F-시스템-아키텍처--기술-스택">
  <img src="https://img.shields.io/badge/시스템_아키텍처_&_기술스택-424242?style=for-the-badge" />
</a>


<a href="#-핵심-기능-요약">
  <img src="https://img.shields.io/badge/핵심_기능-757575?style=for-the-badge" />
</a>

<a href="#-브랜치-전략--컨벤션-요약">
  <img src="https://img.shields.io/badge/브랜치_전략_&_컨벤션-9E9E9E?style=for-the-badge" />
</a>

<a href="#-프로젝트-일정표--마일스톤">
  <img src="https://img.shields.io/badge/마일스톤_&_일정표-616161?style=for-the-badge" />
</a>

<a href="#-프로젝트-결과">
  <img src="https://img.shields.io/badge/프로젝트_성과-424242?style=for-the-badge" />
</a>

<a href="#-팀-소개">
  <img src="https://img.shields.io/badge/팀_소개-757575?style=for-the-badge" />
</a>

<a href="#-contributing">
  <img src="https://img.shields.io/badge/Contributing-9E9E9E?style=for-the-badge" />
</a>

<a href="#-repository-링크">
  <img src="https://img.shields.io/badge/Repository-616161?style=for-the-badge" />
</a>

<a href="#-license">
  <img src="https://img.shields.io/badge/License-424242?style=for-the-badge" />
</a>


---

## 🌱 서비스 개요 (Overview)

**LocalLife**는 청년이 자신의 적성을 기반으로 **로컬 크리에이터의 직업을 체험**하고,

해당 지역의 정착 가능성을 돕는 **지역 순환형 커뮤니티 플랫폼**입니다.


- 프로젝트 이름: **LocalLife — 로컬 기반 AI 적성 추천 체험 플랫폼**
- 프로젝트 유형: **2025 K-Digital Training 해커톤 예선 과제 / MVP**
- 프로젝트 개요: **청년 적성 탐색 → 지역 정착 → 지역 경제 활성화**를 목표로 하는 디지털 사회 서비스
  - 개발 기간:  
  - 2025년 K-Digital Training 해커톤 예선 일정에 맞춰 기획·개발
  - 2025.06.20 ~ 2025.12.20.
  - **[Local Life project Roadmap](https://github.com/orgs/salayo-team/projects/2/views/4)**

---

## 🎨 프로토타입 (Prototype)

<img width="7323" height="5086" alt="Local Life Prototype 8 3MB" src="https://github.com/user-attachments/assets/2bdbce17-a8eb-4195-aaef-b6a324dce924" />

- 서비스 메인 플로우: 온보딩, 체험 클래스, 예약/결제, 매거진, 리뷰까지 포함한 Figma 프로토타입 기반으로 UI/UX 설계
- 모바일 우선 반응형 웹 구조, 로컬 크리에이터/청년(일반 사용자)/관리자의 각 플로우를 분리 설계


---

## 🔍 기획 배경 & 목표

### 📌 문제 인식

1. **청년의 진로 불확실성 증가** 
   - 자신의 적성을 발견하지 못한 채, 기존의 획일적인 삶 외의 선택지를 찾는 청년층 증가
   - 전공/스펙은 있지만 어떤 적성이 자신에게 맞는지 확신하지 못해, 진로 체험을 필요로 하는 청년층 증가
  
2. **로컬 크리에이터의 디지털 홍보/판로 부족**
   - 농가·공방·문화 크리에이터 등은 체험 프로그램을 운영하지만, 디지털 채널 부족으로 홍보 한계
  
3. **“체험 → 진로”로 이어지는 구조 부재**
   - 단순 여행/관광 중심 플랫폼은 많지만, **직업 체험을 진로 탐색과 연결해주는 구조는 부족**

### 🎯 서비스 목표

1. **적성 기반 지역 직업 체험 제공**
   - AI 적성 진단(5가지 적성 타입) → 지역 체험 클래스 추천 구조 설계
     
2. **로컬 크리에이터의 안정적 수익 구조 지원**
   - 예약/정산/후기/매거진 인터뷰 등, **지속 가능한 수익 모델**을 제공
     
3. **청년 적성 탐색 → 지역 정착 → 지역 활성화의 선순환 구조**
   - 체험에 참여한 청년이 **지역 정착·창직(로컬 크리에이터 전환)** 까지 이어지는 로드맵 설계

### 🧑‍💼 주요 타겟 페르소나

- **청년(일반 사용자)**
  - 수도권을 벗어나 지역 정착에 대한 가능성을 고민하는 청년
  - 진로에 대한 확신이 없는 상태에서 적성에 맞는 체험을 통해 나에게 맞는 일을 찾고 싶은 청년
    
- **로컬 크리에이터 / 소규모 사업자**
  - 농가, 공방, 카페, 로컬 브랜드, 문화/예술 기획자 등
  - 자신의 콘텐츠를 **체험/클래스 형태로 판매**하고 싶은 창작자
    
- **지자체 / 공공기관**
  - 지역 정착·관광·문화 활성화를 위해 **청년 유입 프로그램**이 필요한 기관
 
---

### ✨ 주요 기능 소개
 
- **AI 적성 검사** 기반 직무 & 지역 체험 추천
 
- **예약·결제·후기**까지 통합된 사용자 플로우

- **로컬 크리에이터**가 직접 운영하는 체험 등록/관리 시스템 제공

> 💻 상세 기술 구조 및 API는 Backend README에서 확인  
> 👉 [Backend Repository 바로가기](https://github.com/salayo-team/local-life-backend)

---

## 📄 요구사항 명세 (SRS)

서비스 기획 및 도메인 설계는 **요구사항 명세서**를 기준으로 진행되었습니다.

- 도메인별 요구사항 (회원, 관리자, 매거진, 체험 프로그램, 예약, 결제, AI 적성 추천, 온보딩, 리뷰, 검색)
- 권한/보안/성능 고려사항 (Soft Delete, 검수 프로세스, 조회수 동시성, N+1 방지 등)

**문서 링크**

  - 📎 [요구사항 명세서 (PDF)](https://github.com/salayo-team/local-life-backend/blob/develop/.github/docs/software-requirements-specification.pdf)

---

## 🔄 사용자 흐름 요약 (User Flow Overview)

서비스는 아래 세 사용자 유형 중심으로 구성됩니다.

> 예선 과제 기획서에서 정의한 **청년(일반 사용자) / 로컬 크리에이터 / 관리자**의 사용자 플로우를 기준으로 구현되었습니다.


### 👤 청년(일반 사용자)
* AI 기반 온보딩 → 적성 추천 → 체험 검색 → 예약/결제 → 후기 작성

### 🧑‍🌾 로컬 크리에이터
* 크리에이터 등록 → 프로그램 운영 → 예약 승인/거절

### 🛠 관리자
* 검수/승인 → 프로그램 상태 관리 → 매거진/콘텐츠 운영 



> 📌 **전체 흐름 다이어그램 및 상세 설명 보기**
> 
> 👉 [Backend README — 사용자 흐름 전체 보기](https://github.com/salayo-team/local-life-backend?tab=readme-ov-file#-사용자-흐름-user-flow)


---

## 🏗️ 시스템 아키텍처 & 기술 스택

### 🧱 전체 구조

```
Client (Web / Mobile 추후 개발 예정)
       ↕
Backend API (Spring Boot, JPA, Spring Security)
       ↕
MySQL (주요 도메인 데이터) + Redis (캐시/세션/토큰 관리)
       ↕
AI Engine (Spring AI - 적성 진단/추천)
       ↕
AWS S3 (파일, 이미지 업로드)
       ↕
GitHub Actions + Docker (CI/CD & 배포 파이프라인)
```



---

### 🛠 기술 스택

| 분류                           | 기술 스택                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Language**                 | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat\&logo=openjdk\&logoColor=white)                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Backend Framework**        | ![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat\&logo=spring\&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat\&logo=Spring%20Boot\&logoColor=white) ![JPA](https://img.shields.io/badge/JPA-59666C?style=flat\&logo=hibernate\&logoColor=white)                                                                                                 |
| **AI**                       | ![Spring AI](https://img.shields.io/badge/Spring%20AI-6DB33F?style=flat\&logo=spring\&logoColor=white) ![ChatGPT](https://img.shields.io/badge/chatGPT-74aa9c?style=flat\&logo=openai\&logoColor=white)                                                                                                                                                                                                                                                                                                                                    |
| **Database & Migration**         | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat\&logo=MySQL\&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat\&logo=Redis\&logoColor=white) ![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat\&logo=flyway\&logoColor=white)                                                                                                                                                                                                                                                                                                                                                    |
| **Infra / DevOps**           | ![AWS EC2](https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat\&logo=Amazon%20AWS\&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat\&logo=Docker\&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat\&logo=githubactions\&logoColor=white) |
| **Auth & Security**          | ![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat\&logo=Spring%20Security\&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=flat\&logo=jsonwebtokens\&logoColor=white)                                                                                                                                                                                                                                                                                                              |
| **Search / Query**           | ![QueryDSL](https://img.shields.io/badge/QueryDSL-6DB33F?style=flat\&logo=QueryDSL\&logoColor=white)                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **File & External Services** | ![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=flat\&logo=Amazon%20S3\&logoColor=white) ![Spring Cloud AWS](https://img.shields.io/badge/Spring%20Cloud%20AWS-6DB33F?style=flat\&logo=spring\&logoColor=white) ![PortOne(Iamport)](https://img.shields.io/badge/PortOne%20\(Iamport\)-111111?style=flat\&logoColor=white)                                                                                         |
| **Mail & Notification**      | ![Spring Mail](https://img.shields.io/badge/Spring%20Mail-6DB33F?style=flat\&logo=spring\&logoColor=white) ![Jakarta Mail](https://img.shields.io/badge/Jakarta%20Mail-007396?style=flat\&logo=maildotru\&logoColor=white)                                                                                                                                                                                                                                                                                                                 |
| **Docs & Collaboration**     | ![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat\&logo=Swagger\&logoColor=black) ![Notion](https://img.shields.io/badge/Notion-000000?style=flat\&logo=notion\&logoColor=white)                                                                                                                                                                                                                            |
| **Support Libraries**        | ![Lombok](https://img.shields.io/badge/Lombok-CA0C00?style=flat\&logo=apachemaven\&logoColor=white)                                                                                                                                                                                                                                                                                                                                                                                                                                    |

---


## ✨ 핵심 기능 요약

### 🎯 AI 적성 기반 추천

- 온보딩 질문을 통해 **5가지 적성 타입** 도출
- 적성 + 선호 지역 + 카테고리 기반으로 체험 프로그램 매칭
- 추후 “지역 거주·창업”까지 확장 가능한 추천 구조 설계

### 🗺 지역 체험 탐색 & 예약

- 카테고리/지역 필터 기반 체험 프로그램 탐색
- 체험 프로그램 상세페이지에서 일정/가격/정원 확인
- 예약/결제/환불/결제 이력 관리

### 🧑‍🌾 로컬 크리에이터 운영

- 체험 클래스 등록/수정/삭제
- 예약 승인/거절
- 본인 클래스의 리뷰 조회/답글 작성

### 📰 매거진 & 지역 브랜딩

- 관리자 인터뷰 기반 **로컬 크리에이터 매거진** 기능
- 지역/크리에이터 스토리 아카이빙 및 브랜딩

---

## 🌿 브랜치 전략 & 컨벤션 요약
[![PRs](https://img.shields.io/github/issues-pr/salayo-team/local-life-backend?label=pull%20requests)](https://github.com/salayo-team/local-life-backend/pulls)
[![Closed PRs](https://img.shields.io/github/issues-pr-closed/salayo-team/local-life-backend?label=closed%20pull%20requests)](https://github.com/salayo-team/local-life-backend/pulls?q=is%3Apr+is%3Aclosed)
[![Issues](https://img.shields.io/github/issues/salayo-team/local-life-backend)](https://github.com/salayo-team/local-life-backend/issues)
[![Closed Issues](https://img.shields.io/github/issues-closed/salayo-team/local-life-backend?label=closed%20issues)](https://github.com/salayo-team/local-life-backend/issues?q=is%3Aissue+is%3Aclosed)
### 🌳 Branch Strategy

Git Flow 브랜치 전략과 **Squash & Merge** 머지 방식을 조합해 사용합니다. 

👉 자세한 내용은 **[Git Flow 브랜치 전략 문서](https://github.com/salayo-team/local-life-backend/blob/develop/.github/docs/git_flow.pdf)** 를 참고하세요.


| 브랜치 | 용도 |
|--------|------|
| `main` | 운영/배포용 프로덕션 브랜치 |
| `develop` | 통합 개발 브랜치 (기능 브랜치 머지 대상) |
| `feature/*` | 도메인·기능 단위 개발 브랜치 (예: `feature/member`, `feature/payment`, `feature/admin` 등) |
| `docs/*` | 문서 작업용 브랜치 (예: `docs/api-documentation`) |
| `hotfix/*` | 운영 중 긴급 이슈 수정 브랜치 (예: `hotfix/critical-security-fix`) |

> 기본 구조:  
> `main (production)`  
> └─ `develop (개발 통합)`  
> &nbsp;&nbsp;&nbsp;&nbsp;├─ `feature/...`  
> &nbsp;&nbsp;&nbsp;&nbsp;├─ `docs/api-documentation`  
> &nbsp;&nbsp;&nbsp;&nbsp└─ `hotfix/...`  

### 🔄 Merge 전략

- **feature → develop**
  - 방식: **Squash & Merge**
  - 목적: 여러 커밋을 기능 단위 1개의 커밋으로 정리
- **develop → main**
  - 방식: **Merge Commit** 또는 **Squash & Merge**
  - 목적: 프로덕션 배포를 위한 코드 동결 및 검수
- **hotfix → main & develop**
  - 생성: `main` 브랜치에서 `hotfix/*` 브랜치 생성
  - 머지: 수정 완료 후 `main`과 `develop`에 각각 Merge Commit

### 🕰️ 운영 규칙 요약

- 모든 기능 개발은 `develop`에서 분기한 `feature/*` 브랜치에서 진행
- PR 병합 방식: `feature/* → develop` 은 반드시 **Squash & Merge** 사용
- PR 제목에서 `(#5)`와 같은 PR 번호는 제거하고, **의미 있는 한 줄 설명**을 사용
- 머지 완료 후:
  - 로컬 `develop` 최신화 (`git pull origin develop`)
- 하나 이상의 **코드 리뷰 승인(Approve)** 을 받은 뒤에만 머지 진행

---

### 💬 Commit Convention (with gitmoji)

GitHub Rules 문서를 기반으로 **“깃모지 + 타입(소문자) : 작업 내용”** 형식을 사용합니다.


> 기본 형식  
> `이모지 type : 작업 내용`
> 
> `✨ feat : 회원 가입 기능 추가`
> `🔧 add : createMember() 메서드 수정`


👉 자세한 내용은 **[Commit Convention 문서](https://github.com/salayo-team/local-life-backend/blob/develop/.github/docs/github_rules.pdf)** 를 참고하세요.

---

## 📅 프로젝트 일정표 / 마일스톤

[![Milestones](https://img.shields.io/badge/GitHub-전체%20마일스톤-blue?style=flat&logo=github)](https://github.com/salayo-team/local-life-backend/milestones)
[![MVP Milestone](https://img.shields.io/badge/Milestone-MVP%20개발-brightgreen?style=flat&logo=target)](https://github.com/salayo-team/local-life-backend/milestone/1)
[![Feature Expansion](https://img.shields.io/badge/Milestone-Feature%20Expansion-yellow?style=flat&logo=rocket)](https://github.com/salayo-team/local-life-backend/milestone/4)
[![Project Board](https://img.shields.io/badge/Project-Backlog%20Board-orange?style=flat&logo=github)](https://github.com/orgs/salayo-team/projects/2/views/1)


### 단계별 로드맵 

1. **기획 & 리서치**
   - 문제 정의, 타겟 설정, 페르소나 작성
  
2. **요구사항 정의 & 도메인 설계**
   - 요구사항 명세서, ERD, 시스템 아키텍처 설계
   
3. **MVP - 초기 기능 개발** 
   - 회원/인증, AI 적성 진단/추천, 온보딩, 체험 프로그램, 예약/결제, 리뷰, 관리자
   
4. **기획 디벨롭 및 해커톤 제출**   
   - 페르소나 타겟 확장, Notion 설계 문서, 사용자 중심 UX 개선 

5. **Feature Expansion - 부가 기능 또는 후순위 기능 추가 개발** 
   - 매거진, AI 대화형 재설계, 체험 프로그램 추천, 필터링 정렬, 검색 Full-Text INDEX + Ngram 설정
     
6. **테스트 & 리팩토링**
   - 코드 컨벤션/예외 처리/로깅 기준 정리
     
7. **문서화**
   - Swagger 문서,  README 정리

---

## 🏆 프로젝트 결과

### 🎞️ 성과

- **2025 K-Digital Training 해커톤 예선 진출 🎉**
- **MVP 기준 핵심 플로우 구현**
  - 온보딩 → AI 적성 진단 → 프로그램 추천 → 예약 → 체험 후기
- **로컬 크리에이터/관리자까지 포함한 3자 구조 완성**
- **GitHub 기반 협업 규칙/코드 컨벤션/Swagger 문서화 체계 구축**


<img width="4659" height="2574" alt="Image" src="https://github.com/user-attachments/assets/6e876f53-a4f9-447b-a2cc-a63b2ec10613" />



### 📚 인사이트

- 지역 기반 서비스에서는 **정보 구조화와 검수 프로세스가 매우 중요함**
- 프로그램·매거진·리뷰 등 **도메인 간 관계와 상태 관리가 복잡하여 설계 완성도가 서비스 품질에 직접적인 영향을 미침**
- Git Flow, gitmoji 컨벤션, Swagger 기반 문서화를 통해 **팀 협업 생산성이 유의미하게 향상됨**

---

## 👥 팀 소개

<div align="center">

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/jiyoon0000.png" width="110" style="border-radius: 50%; border: 2px solid #ddd;" /><br/>
      <b>김지윤</b><br/>
      <sub>BE · 인증/인가 · 파일/S3업로드 · 매거진/피드백/관리자 · 배포 · 기획&문서</sub><br/>
      <a href="https://github.com/jiyoon0000">@jiyoon0000</a>
    </td>
    <td align="center">
      <img src="https://github.com/j-hann.png" width="110" style="border-radius: 50%; border: 2px solid #ddd;" /><br/>
      <b>한지연</b><br/>
      <sub>BE · 체험프로그램 · 예약/결제 · 검색/필터링&정렬 · 기획&문서</sub><br/>
      <a href="https://github.com/j-hann">@j-hann</a>
    </td>
    <td align="center">
      <img src="https://github.com/sooyeoneo.png" width="110" style="border-radius: 50%; border: 2px solid #ddd;" /><br/>
      <b>허수연</b><br/>
      <sub>BE · AI적성추천&온보딩 · 리뷰/필터링&정렬 · 기획&문서</sub><br/>
      <a href="https://github.com/sooyeoneo">@sooyeoneo</a>
    </td>
  </tr>
</table>

</div>


---

## 🤝 Contributing

본 프로젝트는 **2025년 12월부로 개인 디벨롭 체계로 전환**되었습니다.

현재 기여·코드 활용 기준은 아래 요약을 따릅니다.

---

### 1. Fork & 개인 확장 개발

- 모든 팀원은 프로젝트 종료 후 **자유롭게 Fork하여 개인 레포에서 개발을 이어갈 수 있습니다.**
- 단, **다른 팀원이 작성한 코드/아이디어를 사용할 경우 반드시 작성자 표기**가 필요합니다.

#### ✔️ 작성자 표기 예시

- README: Contributors + 원본 레포 링크
- Commit/PR: `original: @github_id`
- Code 주석: `// original: @github_id (LocalLife project)`

---

### 2. Organization 레포 기여 기준

- Org 레포는 **공통 문서·가이드·템플릿 보관용**으로 유지됩니다.
- 기여 방식(요약):
    - 이슈 등록 → 브랜치 생성 → gitmoji 커밋 → PR 작성 → 모든 리뷰어 승인 → **Squash & Merge**

---

### 3. 협업 기본 원칙

- LocalLife는 **모든 팀원이 함께 만든 공동 성과물**입니다.
- 작성자 표기는 단순 규칙이 아니라,
    **기여 존중 및 책임 명확화를 위한 필수 원칙**입니다.
- 포트폴리오·개인 확장 개발에서도 동일한 기준을 유지합니다.

---

### 📌 자세한 기준은 아래 이슈를 반드시 참고해주세요

👉 [**Contributing Detail Issue 기여 문서 상세 내용 확인하기**](https://github.com/salayo-team/local-life-backend/issues/182)


---

## 📬 Repository 링크

- **Organization**: https://github.com/salayo-team
- **Backend**: https://github.com/salayo-team/local-life-backend

---

## 📄 License

본 프로젝트는 **2025 K-Digital Training 해커톤 및 포트폴리오 목적**으로 개발되었습니다.

- ✅ 교육 및 참고 목적의 사용 가능
- ❌ 사전 동의 없는 상업적 이용 금지
- ⚠️ 코드 사용 시 **출처(LocalLife / Salayo Team) 명시 필수** 및 팀원에게 사전 문의 필요

---

<div align="center">

**LocalLife** - 지역과 청년이 함께 성장하는 플랫폼  
Made by **Salayo Team**

</div>
