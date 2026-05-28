# mcp — MCP (Model Context Protocol)

Decispher's Live Context surface — tools agents call to fetch decisions, topics, intents, and constraints.

1 context unit. Full bodies served via `get_context_for_topic({ topic: "mcp" })`.

## Units in this topic

- **Increase MCP session inactivity window from 30 to 45 minutes** (id: 8f17e97d-1c8e-4b9e-98dd-35802d1200ad) · decision · MEDIUM

For the full body of any unit: `get_decision({ decisionId: "<id>" })`.

For the curated topic context bundle: `get_context_for_topic({ topic: "mcp" })`.
