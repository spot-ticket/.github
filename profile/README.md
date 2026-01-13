# Spot (스팟) - 음식 픽업 서비스
Spot은 대규모 트래픽 환경에서도 안정적인 음식 픽업 예약을 제공하기 위해 2.5개월간 진행한 프로젝트입니다. 
구름 인프라 Profect 5회차에 참가하여 2025년 12월 22일 ~ 2026년 2월 26일까지 진행되었습니다.

## 프로젝트 로드맵 (Project Roadmap)
본 프로젝트는 약 2.5개월간 총 3단계에 걸쳐 진행되었습니다.

### 1차: MVP(Minimum Viable Product) 개발
기간: 2025.12.22 ~ 2026.01.09

__프로젝트 위치__: https://github.com/spot-ticket/Spot.git

목표: 픽업 서비스의 핵심 기능 구현 (Monolith Architecture)

__주요 기능__:
- 사용자 인증 및 권한 관리 (Spring Security, JWT)
- 매장, 메뉴 정보 조회 및 생성
- Toss Payments 연동 및 결제 시스템 구현
- 동시성 제어를 통한 중복 예약 방지 설계
- 메뉴 주문 시스템 구현
- 실시간 주문 예약 및 결제 프로세스 구현
- Github Actions CI/CD를 이용한 코드 스타일 체크 및 빌드 테스트

### 2차: MSA(Microservices Architecture) 전환
기간: 2026.01.12 ~ 2026.01.29

목표: 분산환경을 고려하여 Monolith Architecture를 Microservices Arhitecture로 나눠 응답 속도를 체감합니다.

#### 3차: 인프라 고도화 및 안정화
기간: 2026.02.01 ~ 2026.02.28

---

## Tech Stack

### Backend
Java 21 / Spring Boot 3.5.9
Spring Data JPA

### Database
PostgreSQL 15.1

### Infrastructure & DevOps
- Docker
- CI/CD: GithubActions
- Provision: Terraform
- Maintenance: Ansible
- Deployment: AWS (EC2, RDS), Gabia
- System Architecture (Example)
