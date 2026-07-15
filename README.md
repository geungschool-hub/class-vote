# 학급 임원 선거 (class-vote)

학급회장·부회장 선거용 실시간 투표/개표 앱.

- `index.html` — 학생용 투표소 (핸드폰). 학번 확인 → 기표 → 투표함 투입. **후보가 1명이면 자동 찬반 투표.**
- `admin.html` — 교사용 개표 현황판 (전자칠판). 선거 개설 → 실시간 투표함 → 개표(한 표씩 「正」자 집계) → 당선 발표.

백엔드: Firebase RTDB `vote/` 경로 (gongju7-vocab, 무인증 공개경로 — 규칙 정본은 ai-tool `시험목표제출/database.rules.json`).

비밀투표: 표(ballots)는 학번과 분리 저장되어 누가 누구를 찍었는지 남지 않음. 명부(voters)는 학번만 기록.

Claude AI로 이 앱을 제작함 by 고은표
