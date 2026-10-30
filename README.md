<div align="center">

# x-media

**Free n8n templates and the visuals behind my posts on AI agents, automation, and guardrails.**

[![X](https://img.shields.io/badge/follow-@SaiTarunRonanki-000000?logo=x&logoColor=white)](https://x.com/SaiTarunRonanki)
[![n8n templates](https://img.shields.io/badge/n8n-templates-EA4B71?logo=n8n&logoColor=white)](./templates)
[![Website](https://img.shields.io/badge/site-saitarun.com-6C63FF)](https://saitarun.com)

</div>

---

## Start here: free templates

| Template | What it does | Get it |
|----------|--------------|--------|
| **AI Incident Agent · 8 Guardrail Gates** | Alert in, Claude drafts a patch, 8 gates and a human approve it before anything ships | [Open →](./templates/ai-agent-8-gates) |
| **Lead Approval Flow** | Claude scores a lead and drafts a reply, a human approves before it sends | [Open →](./templates/lead-approval-flow) |
| **LLM Retry Budget** | Backoff, model fallback, and a hard stop for any LLM call | [Open →](./templates/llm-retry-budget) |
| **Silence Alert** | Pings Slack when a workflow quietly stops running | [Open →](./templates/silence-alert) |

Import any `.n8n.json` file in n8n with **Workflows → Import from File**. No keys are stored in any template. Full list in [`templates/`](./templates).

---

## What's in this repo

```
x-media/
├── README.md                 ← you are here
├── templates/                ← free n8n workflows, one folder each
│   ├── README.md             ← template index
│   └── <template-name>/
│       ├── README.md
│       └── <template-name>.n8n.json
└── YYYY-MM-DD/               ← media for that day's posts
    ├── <topic>.png           ← diagrams and cards
    └── <topic>.mp4           ← motion videos
```

| Folder | Contents |
|--------|----------|
| [`templates/`](./templates) | Ready-to-import n8n workflows with setup docs |
| `YYYY-MM-DD/` | Images and videos used in posts that day |

---

## Media archive

| Date | Topics |
|------|--------|
| [2026-10-27](./2026-10-27) | Model swap gate, retry budget, missed reply |
| [2026-10-26](./2026-10-26) | Confidence router, read/write split, silence alert |
| [2026-10-25](./2026-10-25) | Ops pipeline, reliability gate |
| [2026-10-23](./2026-10-23) | Approve by risk, automate first vs decide first |
| [2026-10-22](./2026-10-22) | Lead approval flow |

Newest first.

---

## Conventions

- **Folders:** templates go in `templates/<name>/`; post media goes in a dated `YYYY-MM-DD/` folder.
- **Names:** lowercase, hyphenated, named for the idea (`reliability-gate.png`, not `img1.png`).
- **Formats:** images as `.png`, videos as `.mp4` (H.264).
- **Secrets:** never committed. Templates read keys from environment variables.
- **Adding a template:** create its folder, add the workflow and a README, then add a row to the table above and to [`templates/README.md`](./templates/README.md).

---

## Use and share

Templates and visuals are free to use and remix. A mention or a tag on X is appreciated.

<div align="center">

Built by **Sai Tarun Ronanki** · [X](https://x.com/SaiTarunRonanki) · [saitarun.com](https://saitarun.com)

</div>
