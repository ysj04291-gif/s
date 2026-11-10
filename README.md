# Claude 공식 스킬 TOP 5 따라 해보기

[anthropics/skills](https://github.com/anthropics/skills) 저장소의 공식 스킬 중 5개를
이 저장소의 `.claude/skills/` 폴더에 그대로 복사해 두었습니다.
(원본 커밋: `2c5958e`, 각 폴더의 `LICENSE.txt` 참고 — Apache 2.0)

이 저장소를 Claude Code로 열면 **별도 설치 없이** 5개 스킬이 바로 잡힙니다.
`/skills` 로 목록을 확인할 수 있어요.

## 다섯 가지 스킬과 바로 써볼 문장

| # | 스킬 | 하는 일 | 이렇게 말해 보세요 |
|---|------|---------|-------------------|
| 1 | `skill-creator` | 말로 설명하면 나만의 스킬을 만들어 줌 | "매일 아침 회의록을 요약하는 스킬 만들어 줘" |
| 2 | `frontend-design` | 템플릿 같은 뻔한 화면을 피하게 해 줌 | "frontend-design 스킬로 내 카페 소개 랜딩 페이지 만들어 줘" |
| 3 | `webapp-testing` | 사이트를 직접 열어 눌러 보고 스크린샷까지 찍음 | "방금 만든 페이지를 webapp-testing으로 열어서 버튼 눌러 보고 스크린샷 찍어 줘" |
| 4 | `mcp-builder` | 외부 서비스 연결 도구(MCP 서버)를 만들어 줌 | "날씨 API를 쓰는 MCP 서버를 TypeScript로 만들어 줘" |
| 5 | `doc-coauthoring` | 기획서를 단계별로 같이 씀 | "새 앱 기획서를 같이 써 보자" |

추천 순서: **2 → 3** (페이지 만들고 바로 테스트) → **5** → **4** → **1**

## 다른 프로젝트에서도 쓰고 싶다면 (플러그인 설치)

Claude Code에서 아래 두 줄을 입력하세요.

```
/plugin marketplace add anthropics/skills
/plugin install example-skills@anthropic-agent-skills
```

또는 이 저장소의 `.claude/skills/` 안 폴더를 `~/.claude/skills/` 에 복사하면
모든 프로젝트에서 사용할 수 있습니다.

## 참고
- `webapp-testing` 은 Python + Playwright 가 필요합니다 (`pip install playwright && playwright install chromium`).
- `mcp-builder` 는 Node.js 또는 Python 환경이 필요합니다.
