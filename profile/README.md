# Fullmoon-OSS

**풀문(Fullmoon) 네트워크의 공개 개발 생태계예요.**

하나의 PostgreSQL 원장을 여러 봇·대시보드·클라이언트가 함께 읽는 구조를
오픈소스로 공개하고 있어요. 각자 화폐를 만들지 않고, 같은 원장을 같은 정의로
읽는 것 — 그게 이 조직의 전부예요.

## 레포

| 레포 | 내용 |
|---|---|
| [fullmoon-sdk](https://github.com/Fullmoon-OSS/fullmoon-sdk) | 공식 경제 API 클라이언트 — 의존성 0, Node 18+. 모듈 카탈로그(커뮤니티 모듈) 데이터가 여기 살아요 |
| [fullmoon-economy-api](https://github.com/Fullmoon-OSS/fullmoon-economy-api) | 읽기 전용 경제 HTTP API 서버예요 |
| [fullmoon-modules](https://github.com/Fullmoon-OSS/fullmoon-modules) | 모듈 카탈로그 사이트 — [modules.fullmoon.ink](https://modules.fullmoon.ink)에서 서빙돼요 |
| [fullmoon-docs](https://github.com/Fullmoon-OSS/fullmoon-docs) | 개발자 가이드·정책이에요 |
| [fullmoon-client](https://github.com/RedHatOnTop/fullmoon-client) | 풀문 전용 마인크래프트 클라이언트 — 원클릭 접속 런처 + 네이티브 워프 GUI (GPL-3.0) |

## 빠른 시작

```bash
curl -s https://api.fullmoon.ink/economy/v1/health
# → { "ok": true, "service": "economy-api", "readOnly": true }
```

시작 가이드는 [fullmoon-docs](https://github.com/Fullmoon-OSS/fullmoon-docs)에
있어요.

## 모듈 등록

SDK·API 위에 만든 봇·대시보드·도구는
[modules.fullmoon.ink](https://modules.fullmoon.ink) 카탈로그에 등록할 수 있어요.
[MODULES.md](https://github.com/Fullmoon-OSS/fullmoon-sdk/blob/main/MODULES.md)의
절차대로 — git이 편하면 PR, 아니면 이슈 한 장으로도 등록할 수 있어요.

## 라이선스

SDK·API·모듈·문서는 MIT, fullmoon-client는 GPL-3.0이에요.
