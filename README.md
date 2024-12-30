# ClazzBridge
## 효율적인 학습을 위한 수강생과 강사의 소통 솔루션

### 개발자 소개
권준성 - Full Stack Developer
- React 기반 프론트엔드 개발
- Spring Boot 기반 백엔드 서버 구축
- 실시간 소통 기능 구현
- 데이터베이스 설계 및 구현

### 기술 스택
**Frontend**
- React
- JavaScript (ES6+)
- Redux (상태 관리)
- Socket.io-client
- Tailwind CSS
- React Query

**Backend**
- Java
- Spring Boot
- Spring Security
- Spring Data JPA
- WebSocket
- JWT

**Database**
- MySQL
- JPA/Hibernate

**Development & Deployment**
- Git/GitHub
- Docker
- CI/CD (Jenkins)
- Apache Web Server

### 주요 기능 구현

**1. 실시간 채팅 시스템**
- WebSocket과 Socket.io를 활용한 실시간 통신 구현
- Spring WebSocket 서버 구현
- 채팅 데이터 MySQL 저장 및 관리
- 실시간 메시지 송수신 처리

**2. 사용자 인증 시스템**
- Spring Security 기반 인증 구현
- JWT 토큰 기반 인증
- Access Token / Refresh Token 관리
- 권한 기반 접근 제어

**3. 데이터베이스 설계 및 구현**
- MySQL 데이터베이스 설계
- JPA Entity 관계 설정
- 데이터 정규화
- 인덱스 설계 및 쿼리 최적화

**4. REST API 설계 및 구현**
- RESTful API 설계
- Spring Boot 기반 API 서버 구현
- API 문서화 (Swagger)
- 요청/응답 데이터 검증

**5. 프론트엔드 구현**
- Redux를 활용한 전역 상태 관리
- React 컴포넌트 설계
- 반응형 UI/UX 구현
- API 연동 및 데이터 처리

### 문제 해결 사례

**1. 데이터 동기화 문제 해결**
- 문제: 실시간 채팅 데이터 동기화 불일치
- 해결: 
  - WebSocket 연결 상태 관리 개선
  - 메시지 큐 도입
  - 데이터베이스 트랜잭션 처리 개선

**2. 성능 최적화**
- 문제: 대용량 데이터 처리 시 응답 지연
- 해결:
  - JPA N+1 문제 해결
  - 데이터베이스 인덱스 최적화
  - 캐싱 전략 도입

### 시스템 아키텍처
```
Frontend (React)
├── Components
├── Redux Store
├── Socket Management
└── API Integration

Backend (Spring Boot)
├── Controllers
├── Services
├── Repositories
├── Security
└── WebSocket

Database (MySQL)
├── Users
├── Messages
├── Courses
└── Assignments
```

### API 구조
```
REST API
├── /api/auth
│   ├── /login
│   └── /register
├── /api/chat
│   ├── /rooms
│   └── /messages
├── /api/courses
└── /api/assignments

WebSocket
├── /ws/chat
└── /ws/notifications
```

### CI/CD 파이프라인
1. Git Push
2. Jenkins Build
   - Frontend Build (npm)
   - Backend Build (Maven)
3. Docker Image Build
4. Docker Push
5. Server Deploy
   - Frontend: Apache Web Server
   - Backend: Spring Boot Application
   - Database: MySQL Server

### 프로젝트 성과
- 실시간 소통 환경 구축으로 사용자 경험 개선
- 안정적인 데이터 처리 시스템 구축
- 효율적인 학습 관리 시스템 제공
- 시스템 확장성 및 유지보수성 확보

### 배운 점
1. **풀스택 개발 경험**
   - Frontend와 Backend 통합 개발 경험
   - 데이터베이스 설계 및 최적화
   - 실시간 통신 구현

2. **기술적 성장**
   - Spring Boot 기반 서버 개발 능력 향상
   - React 컴포넌트 설계 능력 향상
   - 데이터베이스 최적화 기술 습득

3. **프로젝트 관리**
   - Git 기반 협업 경험
   - CI/CD 파이프라인 구축
   - 애자일 방법론 실무 적용
