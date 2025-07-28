# 🤖 TrAI-Bot : AI 기반 무역 규제 레이더 플랫폼

복잡하고 파편화된 무역 규제 정보를 AI 채팅으로 명쾌하게 해결하고, 실시간 변동사항까지 알아서 챙겨주는 든든한 대화형 무역 정보 파트너입니다. TrAI-Bot은 신뢰할 수 있는 정보를 즉시 제공함으로써 중소기업의 규제 준수 비용과 운영 리스크를 획기적으로 절감하는 것을 목표로 합니다.

## 📂 Repositories
- Frontend (React, TypeScript) : https://github.com/GodsB1025/trade-frontend

- Backend (Spring Boot, Java) : https://github.com/GodsB1025/trade-backend

- AI Server (FastAPI, Python) : https://github.com/GodsB1025/trade-python

-----

### 🔥 무엇을 해결하나요?

수출입 실무자는 정보 부족이 아닌 **정보의 비대칭성**이 초래하는 예측 불가능한 리스크 때문에 고통받습니다. TrAI-Bot은 다음과 같은 현장의 핵심적인 문제들을 해결합니다.

  * **HS Code 오분류 리스크**

      * **문제점**
        
        전문 지식 없이는 정확한 HS Code 분류가 어려워, 잘못 기재 시 수십억 원대의 관세 추징 및 통관 지연이라는 치명적 결과로 이어질 수 있습니다.
    
      * **TrAI-Bot의 해결책**
        
        자체 RAG(검색 증강 생성) 시스템을 통해 AI 답변의 근거를 신뢰할 수 있는 내부 지식 베이스(PostgreSQL+pgvector)와 외부 웹 정보(관세청 등)로 제한합니다. 모든 답변에 검증 가능한 출처를 명시하여 AI의 환각(Hallucination) 현상을 억제하고 정보의 신뢰도를 극대화합니다.

  * **복잡한 비관세장벽의 공포**

      * **문제점**
        
        국가별로 상이하고 수시로 변경되는 인증, 성분 규제 등 '비관세장벽'은 비전문가가 모든 변수를 파악하고 대응하기 불가능에 가깝습니다.
        
      * **TrAI-Bot의 해결책**
        
        복합적인 질문을 다단계로 분석하는 프롬프트 체이닝 기술을 통해, 사용자가 놓칠 수 있는 비관세장벽 요소를 AI가 심층적으로 분석하고 종합적인 답변을 제공합니다.

  * **극심한 정보 탐색 비효율**

      * **문제점**
        
        신뢰할 수 있는 정보가 관세청, 식약처 등 여러 기관에 흩어져 있어, 통합 정보 획득을 위해 막대한 시간과 노력이 소요됩니다.
      * **TrAI-Bot의 해결책**
        
        지능형 통합 검색을 통해 단일 채팅창에서 HS Code 분류, 규제 조회, 통계 분석, 화물 추적 등 필요한 모든 정보를 한 번에 조회하고 맞춤형 답변을 받을 수 있습니다.

  * **지속적인 정보 추적의 어려움**

      * **문제점**
        
        관세율, 규제, 고시 등은 수시로 변경되지만, 실무자가 모든 변경사항을 놓치지 않고 제때 파악하는 것은 현실적으로 불가능하며, 중요한 개정을 놓치면 곧바로 비용 증가로 이어집니다.
        
      * **TrAI-Bot의 해결책**
        
        프롬프트 체이닝 기반 지능형 모니터링 시스템이 단순 키워드 감지를 넘어 정보의 사실 여부까지 교차 검증하여 알려줍니다. 시스템은 사용자가 북마크한 정보와 관련된 최신 뉴스를 감지하고, 해당 국가의 관세청 등 공식 웹사이트에서 발표 내용을 교차 확인한 후, 변경된 핵심 정보(관세율 수치, 발효일 등)를 정밀하게 추출하여 최종 요약된 알림을 즉시 발송합니다.

-----

### 📈 기대 효과

  * **경제적/산업적 효과**

    HS Code 오분류, 인증 미비 등 핵심 리스크를 사전에 차단하여 막대한 잠재적 손실을 예방하고 기업의 수출 경쟁력을 근본적으로 강화합니다. 1개 품목의 해외 규정 파악에 평균 2시간이 소요되는 작업을 5분 내로 단축시켜, **1인 무역 담당자 기준 연간 약 231만 원 이상의 인건비 절감 효과**를 기대할 수 있습니다.

  * **사회적 효과**

    자본과 인력이 부족한 중소기업 및 개인도 누구나 평등하게 정확한 정보에 접근하게 하여, 대기업과 중소기업 간 정보 비대칭 문제를 해소하고 공정한 경쟁 환경을 조성합니다. 복잡한 규제와 절차를 투명하고 이해하기 쉽게 제공하여 **수출입 시장의 진입 장벽을 획기적으로 낮추고 대한민국 무역의 저변을 확대**하는 데 기여합니다.

-----

### ✨ 주요 기능 및 핵심 경험

#### 🎯 1. 지능형 통합 채팅, 단 한 번의 질문으로 얻는 확신

<img width="1715" height="1035" alt="Traibot 메인 화면" src="https://github.com/user-attachments/assets/76df0dfc-de40-440e-aa53-87802fb60380" />

  * **통합 자연어 질의**

    "유럽에 비건 선크림을 수출할 때 필요한 HS코드, 관세율, 필수 인증과 환경 규제가 뭔가요?"와 같이 복잡한 질문을 `POST /api/chat` 단일 엔드포인트에서 한 번에 처리합니다.

  * **검증 가능한 종합 답변**

    프롬프트 체이닝 기법을 통해 AI가 다단계로 추론하고 검증하여, 관세와 비관세 정보를 종합한 체계적인 답변을 제공합니다. 또한 모든 분석 결과에는 답변의 신뢰도를 높이고 사용자가 직접 사실을 검증할 수 있도록, 신뢰할 수 있는 **출처의 URL과 핵심 원문을 명확하게 함께 제시**합니다.

  * **AI 사고 과정 투명화**

    AI가 어떤 단계를 거쳐 답변을 생성하는지 SSE(Server-Sent Events)를 통해 실시간으로 보여주어 분석 과정의 신뢰도를 높입니다.
<img width="1056" height="1264" alt="답변" src="https://github.com/user-attachments/assets/eac5240e-d884-4ce2-998a-c346377b4a0a" />

#### 👤 2. 개인화 및 회원 전용 기능, 나만을 위한 맞춤형 정보 관리

<img width="1715" height="2423" alt="대시보드" src="https://github.com/user-attachments/assets/c6e7c30a-bb87-43b8-bd1c-c004fd16c0ca" />
<img width="1914" height="888" alt="채팅 내역" src="https://github.com/user-attachments/assets/7747ba72-659e-4b1a-a096-222236cea1c2" />

  * **회원/비회원 차별화**

    회원은 모든 대화 기록이 영구 저장되어 언제든 다시 확인할 수 있으며, 비회원은 세션이나 DB 저장 없이 가볍고 프라이빗한 휘발성 채팅을 경험할 수 있습니다.

  * **동적 북마크 기능**

    AI가 채팅 중 유효한 HS코드나 규제 정보를 감지하면, SSE 스트림의 메타데이터를 통해 실시간으로 북마크 추가 버튼을 생성하여 관심 목록을 손쉽게 구성할 수 있습니다.

  * **개인화 대시보드**

    북마크한 항목들의 최신 현황, 새로운 변동사항 알림, 과거 채팅 기록 등을 한눈에 모아볼 수 있는 나만의 정보 허브를 제공합니다.

#### 🤖 3. 능동적 리스크 관리, 잠든 사이에도 나를 지켜주는 AI 파트너

  * **24시간 자동 모니터링**

    북마크에 저장된 항목과 관련된 전 세계의 정보 변화(관세율 변경, 규정 강화 등)를 24시간 자동으로 감시합니다.

  * **실시간 SMS/이메일 알림**

    "베트남, 철강 품목 반덤핑 관세 15%p 부과 결정"과 같이 AI가 요약하고 검증한 핵심 정보가 사용자의 휴대폰(SMS)과 이메일로 즉시 발송되어 치명적인 리스크를 사전에 방지합니다.
    <img width="774" height="466" alt="스크린샷 2025-07-19 163346" src="https://github.com/user-attachments/assets/18c8feb1-26dd-4366-ab2f-1201cee85a17" />

-----

### 💡 기술 선택 및 이유

| 분야 | 기술 | 선택 이유 |
| :--- | :--- | :--- |
| **Backend** | <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white"> <img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white"> <img src="https://img.shields.io/badge/Spring Security-6DB33F?style=flat-square&logo=spring-security&logoColor=white"> <img src="https://img.shields.io/badge/JPA-59666C?style=flat-square"> <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white"> <img src="https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black"> | 입증된 안정성과 확장성, 강력한 엔터프라이즈 생태계를 바탕으로 복잡한 비즈니스 로직, 데이터베이스 관리, 인증 시스템을 견고하게 처리하기 위해 선택했습니다. |
| **AI Server** | <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"> | Python의 풍부한 AI 라이브러리(LangChain 등)를 활용하고, 비동기 처리를 통한 높은 성능으로 AI 모델 추론 및 서빙에 최적화된 환경을 구축했습니다. |
| **Frontend** | <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black"> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"> <img src="https://img.shields.io/badge/Tanstack-FF4154?style=flat-square&logo=tanstack&logoColor=white"> <img src="https://img.shields.io/badge/Zustand-000000?style=flat-square&logo=zustand&logoColor=white"> | 컴포넌트 기반 아키텍처로 복잡한 UI를 효율적으로 관리하고, 정적 타이핑을 통해 코드 안정성과 유지보수성을 확보하기 위해 선택했습니다. |
| **Database** | <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"> <img src="https://img.shields.io/badge/pgvector-2E8555?style=flat-square"> <img src="https://img.shields.io/badge/pg_partman-663399?style=flat-square"> | RAG 시스템의 핵심인 벡터 검색을 위해 **pgvector**를, 대용량 채팅 로그의 성능 저하를 방지하기 위해 **pg_partman**을 이용한 연도별 자동 파티셔닝을 도입하여 확장성을 확보했습니다. |
| **AI & RAG** | <img src="https://img.shields.io/badge/Claude 3-D97757?style=flat-square"> <img src="https://img.shields.io/badge/LangChain-FFFFFF?style=flat-square&logo=langchain&logoColor=black"> <img src="https://img.shields.io/badge/Voyage AI-1A2B34?style=flat-square"> | 복잡한 규제 문서 해석에 강점을 보이는 **Claude 3**를 메인 모델로, **LangChain**으로 RAG 파이프라인을 구축했습니다. 고성능 **Voyage-3-large (1024차원)** 임베딩 모델로 검색 정확도를 높였습니다. |
| **Cache & Queue** | <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"> | 단순 캐싱을 넘어, SMS 인증 요청 시 Race Condition 제어, 신뢰성 있는 큐(Reliable Queue) 패턴을 적용해 알림 메시지 유실 방지 등 안정적인 분산 시스템을 구축했습니다. |
| **Communication** | <img src="https://img.shields.io/badge/SSE-FF6347?style=flat-square"> | AI의 답변 생성 과정을 실시간으로 보여주기 위해, 양방향 통신이 불필요한 해당 기능에는 WebSocket보다 가볍고 효율적인 SSE를 채택했습니다. |

-----

### 🛡️ 보안 설계

  * **인증 및 권한 부여**

    **JWT 기반의 정교한 토큰 정책**을 적용합니다. Access Token(30분)은 클라이언트 상태로 관리하고, Refresh Token(최대 30일)은 **HttpOnly 쿠키**에 저장하여 CSRF(Cross-Site Request Forgery) 공격을 방어하며 보안을 강화했습니다.

  * **데이터 암호화**

    사용자의 휴대폰 번호와 같이 민감한 개인정보는 **AES-256 알고리즘으로 암호화**하여 데이터베이스에 저장함으로써, 데이터 유출 시에도 정보의 기밀성을 보장합니다.

  * **안정적인 서비스 운영**

    DDoS 공격 등 비정상적인 트래픽으로부터 서비스를 보호하기 위해 API 엔드포인트별로 **요청 빈도를 제어하는 Rate Limiting** 정책을 적용합니다.

  * **데이터베이스 보안**

    데이터베이스 함수 생성 시 `SECURITY DEFINER` 옵션을 사용하되, 해당 함수의 실행 권한을 PUBLIC이 아닌 실제 애플리케이션 서비스 전용 역할(ROLE)에만 최소한으로 부여하여 **최소 권한 원칙**을 준수합니다.

-----

### 💪 주요 기술적 도전과 해결

| 도전 과제 | 해결 방안 |
| :--- | :--- |
| **비동기 스트리밍과 다중 작업 처리** | **3단계 병렬 처리 아키텍처**를 설계하여 (1) AI 서버로부터 자연어 응답 스트리밍, (2) 상세 정보 준비, (3) 회원 대화 기록 저장을 Spring Boot에서 `CompletableFuture`를 통해 비동기 병렬 처리했습니다. 이를 통해 사용자는 AI 답변을 실시간으로 확인하면서 동시에 다른 UI가 업데이트되는 최적의 경험을 누릴 수 있습니다. |
| **외부 시스템의 장애 및 예측 불가능성에 대한 방어적 설계** | **다단계 폴백(Fallback) 전략**을 수립했습니다. Cache -> 외부 API -> 자체 폴백 분석기 순으로 동작하여, 외부 API 장애 시에도 시스템은 자체적으로 최소한의 핵심 기능을 제공합니다. 외부 API 응답을 처리할 때 예상치 못한 데이터 구조 변경에도 시스템이 중단되지 않도록 유연하게 설계했습니다. |
| **대규모 트래픽을 가정한 안정적인 데이터 처리** | **선제적인 데이터베이스 파티셔닝**을 도입했습니다. `pg_partman`을 활용해 `chat_sessions`, `chat_messages` 테이블을 생성일(`created_at`) 기준 연도별로 자동 분할하여, 데이터가 수백만 건 이상 증가해도 꾸준한 고성능을 유지할 수 있는 확장성을 확보했습니다. |

-----

### 🏗️ 시스템 아키텍처, 3단계 병렬 처리를 통한 UX 혁신

TrAI-Bot은 역할 분리를 통해 안정성과 효율성을 극대화했으며, 특히 **사용자 경험(UX) 최적화를 위해 설계된 '3단계 병렬 처리' 아키텍처**를 채택했습니다.

#### 1️⃣ 전체 시스템 아키텍처
<img width="1546" height="807" alt="시스템 아키텍처" src="https://github.com/user-attachments/assets/872cf8a9-208c-4625-9530-7001954a3594" />

#### 2️⃣ 3단계 병렬 처리 플로우

```mermaid
graph TD
    A[POST /api/chat] --> B((병렬 작업 오케스트레이터))
    
    B --> T1[Task 1, AI 응답 생성]
    B --> T2[Task 2, 상세정보 준비] 
    B --> T3[Task 3, 기록 저장]
    
    T1 --> E1[AI 서버 호출]
    T1 --> E2[실시간 스트리밍]
    
    T2 --> E3[HS Code 조회]
    T2 --> E4[규제 정보 수집]
    T2 --> E5[무역 통계 준비]
    
    T3 --> E6[회원 확인]
    T3 --> E7[대화 기록 저장]
    
    E2 --> SSE[SSE Stream Manager]
    E3 --> SSE
    E4 --> SSE
    E5 --> SSE
    SSE --> USER[사용자 화면]
```

#### 3️⃣ 사용자 경험 타임라인

```mermaid
%%{init: {'theme':'base', 'themeVariables': {'primaryTextColor': '#000000', 'primaryColor': '#ffffff', 'primaryBorderColor': '#000000', 'lineColor': '#000000', 'sectionBkgColor': '#f0f0f0', 'altSectionBkgColor': '#e0e0e0', 'gridColor': '#000000', 'c0': '#e1f5fe', 'c1': '#f3e5f5', 'c2': '#e8f5e8', 'c3': '#fff3e0'}}}%%
gantt
    title 사용자 체감 응답 시간 (3단계 병렬 처리)
    dateFormat X
    axisFormat %s초
    
    section 즉시 경험
    질문 입력        :done, q1, 0, 1
    AI 답변 시작      :done, ai1, 1, 2
    실시간 스트리밍   :active, stream, 2, 8
    
    section 백그라운드
    상세정보 준비      :crit, detail, 1, 6
    기록 저장         :back, 1, 4
    
    section 순차 활성화
    HS Code 버튼      :milestone, hs, 6, 0
    규제정보 버튼     :milestone, reg, 7, 0
    통계 버튼         :milestone, stat, 8, 0
```

#### 아키텍처 핵심 설명

**독립적인 서버 구성으로 확장성 확보**
비즈니스 로직을 처리하는 Spring Boot 서버, AI 추론을 전담하는 Python FastAPI 서버, 그리고 사용자 인터페이스를 위한 React 서버로 명확하게 분리되어 있습니다. 이러한 분산 아키텍처는 각 서버가 트래픽 부하에 따라 독립적으로 확장될 수 있도록 하여, 안정적이고 유연한 서비스 운영을 보장합니다.

**3단계 병렬 처리의 UX 혁신**

1.  **즉시성**
   
    사용자가 질문하면 바로 AI 응답 스트리밍 시작
   
3.  **동시성**
   
    상세 정보 준비와 기록 저장이 백그라운드에서 병렬 실행
    
5.  **연속성**
    로딩 없는 자연스러운 인터페이스 경험

이러한 병렬 처리 덕분에 사용자는 긴 로딩 시간을 기다릴 필요 없이, AI의 답변을 읽는 동시에 추가 정보를 탐색할 수 있는 버튼들이 활성화되는 끊김 없는(Seamless) 경험을 하게 됩니다.

-----

### ⚙️ 운영 및 유지보수 전략

  * **자동화된 유지보수**

    PostgreSQL 확장 모듈인 `pg_cron`을 활용하여 **HSCode 개정 주기에 맞춘 데이터 자동 정리**, **만료된 캐시 데이터 주기적 삭제** 등 필수 유지보수 작업을 스케줄링하여 수동 개입 없이 완전 자동화된 운영을 지향합니다.

  * **선제적인 성능 관리**

    대규모 데이터가 수정되는 `hscode_vectors` 테이블이나 쓰기 작업이 빈번한 `chat_messages` 테이블에 대해 주기적으로 `VACUUM` 및 `ANALYZE` 명령을 실행하여, **쿼리 플래너가 항상 최적의 실행 계획을 세우도록 선제적으로 관리**합니다.

  * **가시성 확보 및 모니터링**

    `v_pg_partman_bgw_status`, `v_system_health_v61` 등 스키마에 미리 정의된 **모니터링 뷰**를 Grafana, Datadog 같은 외부 모니터링 도구와 연동하여 시스템 상태를 시각화하고 이상 징후를 조기에 감지할 수 있는 환경을 구축합니다.

-----

### 🏁 시작하기

로컬 환경에서 프로젝트를 실행하려면 다음 단계를 따르세요.

#### 사전 요구사항

  * Java 17+
  * Python 3.10+
  * Node.js 18+
  * PostgreSQL 15+ (DB 서버는 로컬 또는 원격에 준비되어 있어야 합니다.)

#### 1. 레포지토리 클론

프로젝트 실행을 위해 3개의 레포지토리를 모두 클론합니다.

```bash
# Frontend
git clone https://github.com/GodsB1025/trade-frontend.git

# Spring Boot Backend
git clone https://github.com/GodsB1025/trade-backend.git

# Python AI Server
git clone https://github.com/GodsB1025/trade-python.git
```

#### 2. 환경 변수 설정

각 백엔드 프로젝트에 API 키 등 필요한 환경 변수를 설정해야 합니다.


##### **Spring Boot Backend (`trade-backend`)**

`trade-backend/src/main/resources/` 경로에 `application.properties` 파일을 생성하고, 아래 내용을 본인의 환경에 맞게 수정하여 추가합니다.

```properties
# JWT
jwt.secretkey=YOUR_JWT_SECRET_KEY

# OAuth
google.secretkey=YOUR_GOOGLE_SECRET_KEY
naver.secretkey=YOUR_NAVER_SECRET_KEY
kakao.secretkey=YOUR_KAKAO_SECRET_KEY

# AI & API Services
claude.api.key=YOUR_CLAUDE_API_KEY
voyage.api.key=YOUR_VOYAGE_API_KEY
deepl.api.key=YOUR_DEEPL_API_KEY
customs.api.key=YOUR_CUSTOMS_API_KEY_1
customs.api.key2=YOUR_CUSTOMS_API_KEY_2
comtrade.api.key=YOUR_COMTRADE_API_KEY

# SMS Service
sms.api.key=YOUR_SMS_API_KEY
sms.api.secret=YOUR_SMS_API_SECRET
sms.sender.number=YOUR_SMS_SENDER_PHONE_NUMBER

# Database & Cache
redis.host=YOUR_REDIS_HOST_ADDRESS
redis.password=YOUR_REDIS_PASSWORD
postgresql.password=YOUR_POSTGRESQL_PASSWORD

# Email Service
email.username=YOUR_GMAIL_ADDRESS
email.password=YOUR_GMAIL_APP_PASSWORD
```

##### **Python AI Server (`trade-python`)**

`trade-python` 프로젝트의 루트 경로에 `.env` 파일을 생성하고 아래 내용을 본인의 환경에 맞게 수정하여 추가합니다.

```env
DATABASE_URL=postgresql://YOUR_DB_USER:YOUR_DB_PASSWORD@YOUR_DB_HOST/YOUR_DB_NAME
DEBUG=True
ANTHROPIC_API_KEY=YOUR_ANTHROPIC_API_KEY
REDIS_HOST=YOUR_REDIS_HOST
REDIS_USERNAME=YOUR_REDIS_USERNAME
REDIS_PORT=6379
REDIS_PASSWORD=YOUR_REDIS_PASSWORD
VOYAGE_API_KEY=YOUR_VOYAGE_API_KEY
```

#### 3. 애플리케이션 실행

각 프로젝트 디렉터리에서 아래 명령어를 실행하여 서버를 구동합니다.

```bash
# 1. Spring Boot Backend 실행 (별도의 터미널에서)
cd trade-backend
./gradlew bootRun

# 2. Python AI Server 실행 (별도의 터미널에서)
cd ../trade-python
pip install -r requirements.txt
uvicorn main:app --reload --host 0.0.0.0 --port 8001

# 3. Frontend 실행 (별도의 터미널에서)
cd ../trade-frontend
npm install
npm run dev
```

모든 서버가 정상적으로 실행되면 `http://localhost:5173` (Vite 기본 포트)에서 TrAI-Bot을 사용할 수 있습니다.

-----

### 🚀 향후 계획

  * **수출입 필요 서류 자동 초안 생성**
    
    AI가 대화 내용을 바탕으로 상업송장(Commercial Invoice), 포장명세서(Packing List) 등의 초안을 자동으로 작성해주는 기능.
    
  * **AI 기반 최적 관세 FTA 컨설팅**
  
    사용자의 제품이 적용받을 수 있는 가장 유리한 FTA 협정세율을 AI가 찾아주고 추천하는 기능.
    
  * **글로벌 공급망 리스크 분석**

    특정 국가의 정치, 경제 상황 변화가 사용자의 수출입에 미칠 영향을 분석하고 예측하는 서비스.

-----

### 👨‍👩‍👧‍👦 팀 소개, NaN null 갖고 싶어

| 이름 | 역할 | GitHub |
| :--- | :--- | :--- |
| **홍태극** | 팀장, AI 아키텍쳐, Backend | [brain1401](https://github.com/brain1401) |
| **김경보** | Backend, Frontend | [GodsB1025](https://github.com/GodsB1025) |
| **이광원** | Frontend | [Lee-KwangWon](https://github.com/Lee-KwangWon) |
| **윤선현** | Frontend | [YOON-SEONHYUN](https://github.com/YOON-SEONHYUN) |
