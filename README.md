# DeviceAgent Remote

ESP32-C6 WoL 보드 리모컨 웹 페이지 (MQTT over WSS, EMQX Cloud).
주소: https://kmmun94.github.io/deviceagent-remote/

- 비밀번호·명령 서명 키는 페이지에 없음 — 각 기기 브라우저(localStorage)에만 저장
- `wake`는 HMAC-SHA256 서명 명령으로만 보냄 (`wake|ts|nonce|sig`)
- 원본: private repo `DeviceAgent` 의 `web/index.html` — 수정은 원본에서 하고 여기로 복사

## Commit messages

```text
<area>[(scope)]: <summary>

<body — optional, Korean OK>
```

- area: `web` (index.html) · `docs` (README) · `repo` (hooks, agent rules, config)
- summary: English, imperative, lowercase start, ≤72 chars, no trailing period
- **No AI attribution** — no `Co-Authored-By:`, "Generated with …", or 🤖 for any tool (Claude, Codex, Grok …)
- Enforced by `.githooks/commit-msg`; enable once per clone:

```bash
git config core.hooksPath .githooks
```
