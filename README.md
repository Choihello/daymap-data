# daymap-data

[Seoul Daymap](https://seoul-daymap.vercel.app)의 **파생 데이터 발행소**입니다.
원본 수집 저장소(seoul-pulse)는 비공개이며, 여기에는 사이트가 공개
서빙하는 파생물만 올라옵니다.

- `starlog/YYYY-MM-DD.json` — 밤 21시 무렵 서울 121개 구역의 혼잡 스냅샷
  (별자리 일지의 원료). `starlog/index.json`이 날짜 목록.
- `crowd/recent24h.json` — 직전 24시간 구역별 혼잡 시계열 집계.

발행: seoul-pulse의 GitHub Actions(수집 워크플로의 Publish 스텝).
소비: seoul-daymap.vercel.app이 raw.githubusercontent.com 으로 읽습니다.

> 2026-08-25에 Vercel Blob(무료 한도 연산 초과 서스펜드)에서 이관했습니다.
