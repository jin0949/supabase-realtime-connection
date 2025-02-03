# Supabase Realtime Service

Supabase Realtime을 활용한 데이터베이스 변경 감지 서비스입니다. PostgreSQL의 변경 사항을 실시간으로 모니터링하고 처리합니다.

## 주요 기능

- Supabase Realtime 웹소켓 연결 관리
- PostgreSQL 테이블 변경 실시간 감지
- 비동기 이벤트 처리
- 자동 재연결 지원

## 시스템 구성

- `RealtimeService`: 실시간 이벤트 처리 핵심 클래스
- 비동기 콜백 처리 시스템
- 자동화된 연결 관리

## 모니터링 설정

- 스키마: public
- 테이블: laundry
- 이벤트 타입: INSERT

## 테스트

- 웹소켓 연결 테스트
- 실시간 이벤트 수신 테스트

## 환경 설정

필요한 환경 변수:
- DATABASE_URL
- JWT

## 실행 방법

```bash
python main.py
```

## 테스트 실행

```bash
pytest test_realtime.py
```

## 주의사항

- 적절한 JWT 토큰 필요
- 안정적인 네트워크 연결 필요
- 로깅 레벨 설정 확인

---
