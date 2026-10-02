# onestop.artus.kr — 주식회사 총무부

1인 창업 원스톱 세팅 회사 "주식회사 총무부"의 홈페이지. 정적 HTML/CSS, 빌드 도구 없음.

```
public/            ← Cloudflare Pages 배포 루트
  index.html       홈 (1페이지)
  404.html
  favicon.svg
  _headers
  data/history.json  변경 이력 (모든 변경을 여기에 기록)
```

## 배포
Cloudflare Pages 프로젝트 `onestop` (계정 prodigen@gmail.com). GitHub 자동 빌드 연동 없음 → 직접 업로드:

```
npx wrangler pages deploy public --project-name onestop --branch main --commit-dirty=true
```

배포 전 `npx wrangler whoami` 로 prodigen 계정인지 확인.

## 도메인
- https://onestop.artus.kr (artus.kr 존: prodigen 계정, CNAME onestop → onestop.pages.dev)
- 업무 메일 hello@onestop.artus.kr

## 운영
진행 관리는 상황판(전경도 · 할 일 · 아카이브): https://claude.ai/artifact/1mzK1TXXnAfJmQMrBYFQzE
