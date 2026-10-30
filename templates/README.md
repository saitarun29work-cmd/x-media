# n8n Templates

Free, production-minded n8n workflows by [@SaiTarunRonanki](https://x.com/SaiTarunRonanki).

| Template | What it does | Folder |
|----------|--------------|--------|
| AI Incident Agent · 8 Guardrail Gates | Alert in, Claude drafts a patch, 8 gates and a human approve it | [`ai-agent-8-gates`](./ai-agent-8-gates) |

## Folder layout

Every template follows the same shape, so new ones slot in without changes:

```
templates/
├── README.md                  ← this index
└── <template-name>/
    ├── README.md              ← how it works, setup, config, customizing
    └── <template-name>.n8n.json
```

## Adding a template

1. Create `templates/<template-name>/` using lowercase-hyphen names.
2. Add the exported workflow as `<template-name>.n8n.json`, with no credentials or keys inside.
3. Copy the section layout of an existing template README.
4. Add a row to the table above.
