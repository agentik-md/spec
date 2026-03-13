# AGENTIK.md

The AI Agent Safety Stack — 12 open specifications for AI agent safety, quality, and accountability.

> One file per concern. Drop it in your repo. Your agent reads it on startup.

- Full specification: [agentik.md](https://agentik.md)
- AI-readable: [llms.txt](https://agentik.md/llms.txt)
- License: MIT

---

## The AI Agent Safety Stack

Agentik.md maintains twelve plain-text Markdown file conventions for autonomous AI systems. Each specification addresses a specific concern.

### Operational Control

| Spec | Purpose | Repo | Site |
|------|---------|------|------|
| KILLSWITCH.md | Emergency stop — halt all agent activity | [killswitch-md/spec](https://github.com/killswitch-md/spec) | [killswitch.md](https://killswitch.md) |
| THROTTLE.md | Rate and cost control — slow down before hitting limits | [throttle-md/spec](https://github.com/throttle-md/spec) | [throttle.md](https://throttle.md) |
| ESCALATE.md | Human notification and approval — pause and ask before acting | [escalate-md/spec](https://github.com/escalate-md/spec) | [escalate.md](https://escalate.md) |
| FAILSAFE.md | Safe fallback — revert to last known good state | [failsafe-md/spec](https://github.com/failsafe-md/spec) | [failsafe.md](https://failsafe.md) |
| TERMINATE.md | Permanent shutdown — no restart without human intervention | [terminate-md/spec](https://github.com/terminate-md/spec) | [terminate.md](https://terminate.md) |

### Data Security

| Spec | Purpose | Repo | Site |
|------|---------|------|------|
| ENCRYPT.md | Data classification and protection — define what must be encrypted | [encrypt-md/spec](https://github.com/encrypt-md/spec) | [encrypt.md](https://encrypt.md) |
| ENCRYPTION.md | Cryptographic standards and key rotation — technical implementation | [encryption-md/spec](https://github.com/encryption-md/spec) | [encryption.md](https://encryption.md) |

### Output Quality

| Spec | Purpose | Repo | Site |
|------|---------|------|------|
| SYCOPHANCY.md | Anti-sycophancy — require citations, enforce honest disagreement | [sycophancy-md/spec](https://github.com/sycophancy-md/spec) | [sycophancy.md](https://sycophancy.md) |
| COMPRESSION.md | Context compression — summarise safely without losing critical info | [compression-md/spec](https://github.com/compression-md/spec) | [compression.md](https://compression.md) |
| COLLAPSE.md | Drift prevention — detect collapse, enforce recovery | [collapse-md/spec](https://github.com/collapse-md/spec) | [collapse.md](https://collapse.md) |

### Accountability

| Spec | Purpose | Repo | Site |
|------|---------|------|------|
| FAILURE.md | Failure mode mapping — every error state and response | [failure-md/spec](https://github.com/failure-md/spec) | [failure.md](https://failure.md) |
| LEADERBOARD.md | Agent benchmarking — track quality, detect regression | [leaderboard-md/spec](https://github.com/leaderboard-md/spec) | [leaderboard.md](https://leaderboard.md) |

---

## Why This Exists

AI agents spend money, send messages, modify files, and call external APIs — often autonomously. Regulations are catching up:

- **EU AI Act** (August 2026) — mandates human oversight and shutdown capabilities
- **Colorado AI Act** (June 2026) — requires impact assessments and transparency
- **US state laws** — California, Texas, Illinois and others have active AI governance requirements

These specifications give you a standardised, auditable record of your agent's safety boundaries.

---

## Quick Start

Copy the specifications from the individual GitHub repositories into your project root:

```
your-project/
├── AGENTS.md
├── CLAUDE.md
├── KILLSWITCH.md     ← start here
├── THROTTLE.md       ← add for fine-grained control
├── ENCRYPT.md        ← add if handling sensitive data
├── README.md
└── src/
```

Your agent framework will load the file at startup and parse the key-value pairs. No dependencies, no build step, no authentication required.

---

## Contributing

PRs welcome for additional detection patterns, language-specific parsers, and integration guides. Visit the individual specification repositories to contribute.

---

## Licence

MIT — see [LICENSE](LICENSE) for details.

## Disclaimer

This specification is provided "as-is" without warranty of any kind. It does not constitute legal, regulatory, or compliance advice in any jurisdiction. Use does not guarantee compliance with any applicable law, regulation, or standard — including the EU AI Act (2024/1689), Colorado AI Act (SB 24-205), or any other legislation. Organisations should consult qualified professionals to determine their regulatory obligations. The authors accept no liability for any loss or consequence arising from use of this specification.
