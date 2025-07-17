# **🤖 TrAI-Bot : AI 기반 무역 규제 레이더 플랫폼**

복잡하고 파편화된 무역 규제 정보를 AI 채팅으로 명쾌하게 해결하고, 실시간 변동사항까지 알아서 챙겨주는 든든한 대화형 무역 정보 파트너입니다.

### **📝 프로젝트 소개**

TrAI-Bot (Trade AI Bot)은 정보의 홍수 속에서 길을 잃은 중소기업 수출입 실무자들을 위한 AI 기반 무역 정보 플랫폼입니다. 사용자는 더 이상 여러 사이트를 헤매며 정보를 짜깁기할 필요 없이, 복잡한 무역 질문을 자연어 채팅으로 해결할 수 있습니다. TrAI-Bot은 명확한 근거와 출처를 제시하여 정보의 '확신'을 제공하고, 24시간 자동 모니터링과 실시간 알림을 통해 보이지 않는 '비관세장벽' 리스크까지 관리해주는 든든한 AI 파트너입니다.

-----

### **🔥 무엇을 해결하나요?**

수출입 실무자는 정보 부족이 아닌 '**정보의 불확실성**' 때문에 고통받습니다. TrAI-Bot은 이러한 핵심적인 문제들을 해결합니다.

  * "**이 HS코드가 정말 맞을까?**" - 확신 부재의 문제
      * 여러 사이트를 뒤져 찾은 정보가 최신인지, 정확한지 확신할 수 없어 잘못된 신고로 인한 관세 추징 및 통관 지연 리스크에 노출됩니다.
      * **TrAI-Bot의 해결책** : AI가 RAG(검색 증강 생성) 시스템을 통해 최신 법령 및 데이터를 분석하고, 신뢰할 수 있는 출처를 명시하여 답변의 확신을 제공합니다.
  * "**내가 놓친 규제는 없을까?**" - 보이지 않는 장벽의 공포
      * 수시로 바뀌는 국가별 인증(CE, FCC), 환경 규제, 기술 표준 등 '비관세장벽'은 하나만 놓쳐도 전량 폐기, 반송 등 막대한 손실로 이어질 수 있는 숨겨진 지뢰입니다.
      * **TrAI-Bot의 해결책** : 북마크 기반 24시간 자동 모니터링과 실시간 SMS/이메일 알림을 통해 사용자가 신경 쓰지 못하는 사이에도 리스크를 감지하고 즉시 알려줍니다.

-----

### **✨ 주요 기능 및 핵심 경험**

TrAI-Bot은 사용자에게 세 가지 혁신적인 경험을 제공합니다.

#### **🎯 경험 1 : 단 한 번의 질문으로 얻는 확신**

  * **통합 자연어 질의** : "유럽에 비건 선크림을 수출할 때 필요한 HS코드, 관세율, 필수 인증과 환경 규제가 뭔가요?"와 같이 복잡한 질문을 한 번에 처리합니다.
  * **구조화된 종합 답변** : 프롬프트 체이닝 기법을 통해 AI가 다단계로 추론하고 검증하여, 관세와 비관세 정보를 종합한 체계적인 답변을 제공합니다.
  * **신뢰할 수 있는 출처 제시** : 모든 핵심 정보에 "출처 : EU 관세청 TARIC DB"와 같이 명확한 출처를 함께 제시하여 교차 검증이 가능합니다.
  * **AI 사고 과정 투명화** : Claude AI가 어떤 단계를 거쳐 답변을 생성하는지 SSE(Server-Sent Events)를 통해 실시간으로 보여주어 분석 과정의 신뢰도를 높입니다.

#### **👤 경험 2 : 나만을 위한 맞춤형 정보 관리**

  * **회원/비회원 차별화 서비스**
      * **비회원** : 가입 없이 핵심 채팅 기능을 즉시 체험할 수 있으며, 모든 대화는 서버에 저장되지 않아 개인정보 유출 걱정이 없습니다.
      * **회원** : 모든 대화 내용이 HSCode 개정 주기에 맞춰 5년간 안전하게 보관되며, 북마크, 대시보드 등 모든 개인화 기능을 사용할 수 있습니다.
  * **동적 북마크 기능** : AI가 채팅 중 유효한 HS코드나 규제 정보를 감지하면, SSE 스트림의 메타데이터를 통해 실시간으로 북마크 추가 버튼을 생성하여 관심 목록을 손쉽게 구성할 수 있습니다.
  * **개인화 대시보드** : 북마크한 항목들의 최신 현황, 새로운 변동사항 알림, 과거 채팅 기록 등을 한눈에 모아볼 수 있는 나만의 정보 허브를 제공합니다.

#### **🤖 경험 3 : 잠든 사이에도 나를 지켜주는 AI 파트너**

  * **24시간 자동 모니터링** : 북마크에 저장된 항목과 관련된 전 세계의 정보 변화(관세율 변경, 규정 강화 등)를 24시간 자동으로 감시합니다.
  * **AI 기반 핵심 요약 및 검증** : 변화가 감지되면, AI가 여러 출처를 교차 검증하고 복잡한 원문의 핵심 내용만 정확하게 요약합니다.
  * **실시간 SMS/이메일 알림** : "베트남, 철강 품목 반덤핑 관세 15%p 부과 결정"과 같이 AI가 요약한 핵심 정보가 사용자의 휴대폰(SMS)과 이메일로 즉시 발송되어 치명적인 리스크를 사전에 방지합니다.

-----

### **🎬 스크린샷**

[1. 통합 채팅 및 AI 사고 과정]
(스크린샷 이미지를 여기에 삽입하세요)
[2. 회원 전용 대시보드]
(스크린샷 이미지를 여기에 삽입하세요)
[3. 실시간 알림 예시]
(스크린샷 이미지를 여기에 삽입하세요)

-----

### **🛠️ 기술 스택**

| 분야          | 기술 |
| :------------ | :--- |
| Backend       |      |
| Frontend      |      |
| Database      |      |
| AI & RAG      |      |
| Auth          |      |
| Communication |      |
| DevOps        |      |

-----

### **🏗️ 시스템 아키텍처**

TrAI-Bot은 이벤트 기반의 3단계 병렬 처리 아키텍처를 채택하여 최적의 응답성과 사용자 경험을 보장합니다.

```mermaid
graph TD
    subgraph "Client"
        A[사용자]
    end

    subgraph "Backend (FastAPI)"
        B(POST /api/chat)
        C{인증 상태 확인}
        D["AI 응답 생성<br/>(Task A)"]
        E["상세페이지 정보 준비<br/>(Task B)"]
        F["회원 대화 기록 저장<br/>(Task C)"]
        G((병렬 처리 매니저))
        H(SSE Stream)
        I["Auth Middleware<br/>(JWT)"]
        J["Private APIs<br/>/bookmarks, /dashboard"]
    end

    subgraph "AI & Data Services"
        K[Claude AI]
        L["RAG System<br/>(LangChain + VoyageAI)"]
        M["PostgreSQL<br/>(pgvector, pg_partman)"]
        N["Redis<br/>(Cache & Rate Limit)"]
    end

    A -- "자연어 질문" --> B
    B --> I
    B --> C

    C -- "회원" --> G
    C -- "비회원" --> G

    G --- D
    G --- E
    G --- F

    D -- "자연어 응답 스트림" --> H
    E -- "상세 버튼 정보" --> H
    F -- "저장 완료 상태" --> H

    D --> K
    D --> L
    L --> M
    E --> M
    F --> M

    H -- "실시간 SSE 이벤트" --> A

    A -- "API 요청" --> J
    J --> I
    I --> J
    J -- "DB 작업" --> M
    J -- "Cache 작업" --> N
```

**핵심 데이터 플로우**

1.  **질의 및 분기** : 사용자가 POST /api/chat으로 질문하면, 인증 미들웨어가 회원/비회원 여부를 판별합니다.
2.  **병렬 처리 시작** : 병렬 처리 매니저는 (A) AI 응답 생성, (B) 상세페이지 정보 준비, (C) 회원 기록 저장 세 가지 작업을 동시에 시작합니다.
3.  **실시간 SSE 스트리밍** : 각 작업의 결과(AI 답변, 상세 버튼, 저장 상태 등)는 준비되는 즉시 SSE 이벤트를 통해 클라이언트로 실시간 전송됩니다.
4.  **RAG 시스템 연동** : AI 응답 생성 시 RAG 시스템이 PostgreSQL의 벡터 데이터를 검색하여 정확하고 근거 있는 답변을 구성합니다.
5.  **지식 베이스 자가 학습 파이프라인** : 웹 검색을 통해 얻은 새로운 HSCode 정보는 백그라운드에서 자동으로 벡터화되어 hscode_vectors 테이블에 저장되어 시스템의 지식을 지속적으로 업데이트합니다.

-----

### **🗄️ 데이터베이스 스키마**

pgvector를 활용한 벡터 검색과 pg_partman을 통한 대용량 데이터 자동 파티셔닝을 적용하여 성능과 확장성을 확보했습니다.

```mermaid
erDiagram
    users {
        bigint id PK
        varchar email UK
        varchar password_hash
        varchar name
        varchar profile_image
        varchar refresh_token
        timestamp refresh_token_expires_at
        boolean remember_me_enabled
        boolean phone_verified
    }

    chat_sessions {
        uuid session_uuid PK "회원 전용 채팅 세션"
        bigint user_id FK
        varchar session_title
        timestamp created_at
        timestamp updated_at
    }

    chat_messages {
        bigint message_id PK
        uuid session_uuid FK
        varchar message_type
        text content
        jsonb hscode_analysis "AI 분석 결과 저장"
        timestamp created_at "PARTITION KEY"
    }

    bookmarks {
        bigint id PK
        bigint user_id FK
        varchar type
        varchar target_value
        varchar display_name
        boolean sse_generated
        boolean sms_notification_enabled
        boolean email_notification_enabled
        boolean monitoring_active
    }

    hscode_vectors {
        bigint id PK
        varchar hscode UK
        text product_name
        vector embedding "pgvector(2048)"
        jsonb metadata
    }

    users ||--o{ chat_sessions : "has"
    users ||--o{ bookmarks : "owns"
    chat_sessions ||--o{ chat_messages : "contains"
```

-----

### **🏁 시작하기**

로컬 환경에서 프로젝트를 실행하려면 다음 단계를 따르세요.

#### **사전 요구사항**

  * Python 3.10+
  * Node.js 18+
  * Docker & Docker Compose
  * PostgreSQL 15+ (pgvector 와 pg_partman 확장 기능이 설치되어 있어야 합니다.)

#### **1. 레포지토리 클론**

```bash
git clone https://github.com/your-repo/TrAI-Bot.git
cd TrAI-Bot
```

#### **2. 환경 변수 설정**

루트 디렉토리에 .env 파일을 생성하고 필요한 환경 변수를 설정합니다.

```
# Database
DATABASE_URL="postgresql://user:password@localhost:5432/traibot"
REDIS_URL="redis://localhost:6379"

# AI APIs
ANTHROPIC_API_KEY="your_claude_api_key"
VOYAGE_API_KEY="your_voyage_ai_api_key"

# JWT
JWT_SECRET="your_super_secret_key"
```

#### **3. 백엔드 실행 (Python/FastAPI)**

```bash
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload
```

#### **4. 프론트엔드 실행 (React/TypeScript)**

```bash
cd frontend
npm install
npm run dev
```

#### **5. 데이터베이스 실행 (Docker)**

Docker Compose를 사용하여 PostgreSQL과 Redis를 실행합니다.

```bash
docker-compose up -d
# 필요한 경우, 초기 파티션 생성 스크립트를 실행하세요.
# python scripts/setup_partitions.py
```

이제 `http://localhost:5173` 에서 TrAI-Bot을 사용할 수 있습니다. (Vite 기본 포트 기준)

-----

### **🚀 향후 계획**

저희는 현재의 성과에 만족하지 않고, 무역 업무의 전 과정을 책임지는 '**All-in-One 파트너**'로 발전해 나갈 것입니다.

  * **수출입 필요 서류 자동 초안 생성** : AI가 대화 내용을 바탕으로 상업송장(Commercial Invoice), 포장명세서(Packing List) 등의 초안을 자동으로 작성해주는 기능.
  * **AI 기반 최적 관세 FTA 컨설팅** : 사용자의 제품이 적용받을 수 있는 가장 유리한 FTA 협정세율을 AI가 찾아주고 추천하는 기능.
  * **글로벌 공급망 리스크 분석** : 특정 국가의 정치, 경제 상황 변화가 사용자의 수출입에 미칠 영향을 분석하고 예측하는 서비스.

-----

### **👨‍👩‍👧‍👦 팀 소개**

| 이름   | 역할                                          | GitHub                                                                       |
| :----- | :-------------------------------------------- | :--------------------------------------------------------------------------- |
| 홍태극 | 팀장, Backend & AI Engine 총괄, Frontend 지원 | [GitHub 프로필](https://www.google.com/search?q=https://github.com/GIT-Taek) |
| 김경보 | Backend, Frontend 지원                        | [GitHub 프로필](https://github.com/GodsB1025)                                |
| 이광원 | Frontend                                      | [GitHub 프로필](https://github.com/Lee-KwangWon)                             |
| 윤선현 | Frontend                                      | [GitHub 프로필](https://github.com/YOON-SEONHYUN)                            |
