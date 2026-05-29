# Unmapped Context

8 active context units in **First Project** are not yet assigned to a topic.
Fetch any unit's full body via MCP. Review and assign these from the Unmapped Review Queue in the Decispher dashboard.

| Title | Type | Severity | MCP fetch |
|-------|------|----------|-----------|
| Migrate from Umbraco to Contentful for CMS functionality | decision | HIGH | `decispher.get_decision({ decisionId: "dfae8267-c945-4f1b-bfe1-5321b12d8c87" })` |
| Phase 2 is the Decision Capture Engine (capture & intelligence layer) | decision | HIGH | `decispher.get_decision({ decisionId: "4ddf24a6-8c7a-438e-abb6-dbaeeaef1e4e" })` |
| Phase 2 pipeline: Sources → Recorders → Core Intelligence → Notifications → Dashboard | decision | HIGH | `decispher.get_decision({ decisionId: "b0a3128b-6658-4409-80b4-a5b2e0703890" })` |
| An LLM-powered Analyzer Service turns raw activity into structured decisions | decision | MEDIUM | `decispher.get_decision({ decisionId: "c516730e-6c60-4ff2-a1f2-b92ae0f16bab" })` |
| BullMQ on Redis is the message queue between recorders and the analyzer | decision | MEDIUM | `decispher.get_decision({ decisionId: "430932a3-f225-48ae-8791-b24632005528" })` |
| Decision Store is Postgres with embeddings | decision | MEDIUM | `decispher.get_decision({ decisionId: "81e99341-c4d5-405e-bea4-a4873d20d406" })` |
| Notification Service uses the Strategy Pattern for pluggable channels | convention | MEDIUM | `decispher.get_decision({ decisionId: "7e82c9e0-e875-4e42-82ee-b04ecd795fa2" })` |
| Two ingestion recorders: Slack Recorder Bot and Code Change Recorder | decision | MEDIUM | `decispher.get_decision({ decisionId: "6e1cdf57-adc7-41fe-9a1b-02cdeeb2bd2d" })` |
