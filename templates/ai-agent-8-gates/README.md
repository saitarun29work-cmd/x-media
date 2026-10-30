# AI Incident Agent · 8 Guardrail Gates (n8n template)

A free n8n workflow by [@SaiTarunRonanki](https://x.com/SaiTarunRonanki): one webhook in, Claude diagnoses and drafts a patch, and nothing ships without passing 8 gates.

## The 8 gates

1. **Webhook Dedup** drops duplicate alerts seen in the last 10 minutes
2. **Schema Gate** rejects bad payloads before they reach the model
3. **Router** sends each alert down the right path
4. **MCP Scope** limits which tools the agent may touch
5. **Few-Shot** grounds the model with known-good examples
6. **Sandbox Verify** checks the patch before anyone sees it
7. **Confidence Gate** escalates to a human when the agent isn't sure
8. **Slack Approval** keeps a human on the final yes

## Use it

1. Download `ai-agent-8-gates.n8n.json`.
2. In n8n: **Workflows → Import from File**.
3. Set `ANTHROPIC_API_KEY` as an environment variable, and connect your Slack credentials on the approval node.
4. POST an alert to the webhook path `agent-alert`.

No keys are stored in the file.

If it helps, follow me on X for more agent builds: [@SaiTarunRonanki](https://x.com/SaiTarunRonanki)
