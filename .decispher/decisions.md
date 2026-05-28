<!-- DECISION-DFAE8267 -->
## Decision: Migrate from Umbraco to Contentful for CMS functionality

**Status**: Active  
**Date**: 2026-05-26  
**Severity**: Critical

**Files**:
- `infrastructure/cms`
- `frontend/content-integration`

**Rules**:
```json
{
  "conditions": [
    {
      "type": "file",
      "pattern": "infrastructure/cms/**/*",
      "content_rules": [
        {
          "mode": "string",
          "patterns": [
            "Umbraco",
            ".NET",
            "Windows"
          ]
        }
      ]
    },
    {
      "type": "file",
      "pattern": "frontend/content-integration/**/*",
      "content_rules": [
        {
          "mode": "string",
          "patterns": [
            "Umbraco",
            ".NET"
          ]
        }
      ]
    }
  ],
  "match_mode": "any"
}
```

### Context

**Decision:** Replace the planned Umbraco CMS implementation with Contentful as a headless CMS solution, delivering content via REST and GraphQL APIs.

---

<!-- DECISION-8F17E97D -->
## Decision: Increase MCP session inactivity window from 30 to 45 minutes

**Status**: Active  
**Date**: 2026-05-25  
**Severity**: Warning

**Files**:
- `redis_ttl_config`
- `mcp_logs_session_logic`

**Rules**:
```json
{
  "conditions": [
    {
      "type": "file",
      "pattern": "*(redis_ttl_config|mcp_logs_session_logic)*",
      "content_rules": [
        {
          "mode": "regex",
          "start": 0,
          "pattern": "(30|0\\.5)\\s*(minutes|m)"
        }
      ],
      "content_match_mode": "any"
    }
  ],
  "match_mode": "all"
}
```

### Context

**Decision:** Update the MCP session inactivity window definition from 30 minutes to 45 minutes across the Redis TTL and mcp_logs session gap logic.
