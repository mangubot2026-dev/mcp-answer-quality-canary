# MCP Answer-Quality Canary

Continuously verifies that MCP servers answer correctly: real MCP protocol canary calls (list + seeded-record search) cross-checked against independent ground truth, returning agent-readable PASS / FAIL / UNKNOWN verdicts with defect classes (truncation, null result, wrong value, missing seeded record, pagination loop, timeout). $0.50 per server/month flat; first month free on the first 5 servers, once per operator.

## Connect (remote MCP, streamable HTTP)

- MCP endpoint: `https://textforagents.com/products/mcp-answer-quality-canary/mcp`
- Transport: streamable HTTP (also accepts POST at the product base URL)
- Auth: `Authorization: Bearer <token>` — get a token self-serve:
  `POST https://textforagents.com/products/mcp-answer-quality-canary/register` then
  `POST /trial` (one-time free trial) or `POST /subscribe` (x402, Base USDC).

Example client config:

```json
{
  "mcpServers": {
    "mcp-answer-quality-canary": {
      "url": "https://textforagents.com/products/mcp-answer-quality-canary/mcp",
      "headers": { "Authorization": "Bearer <your-token>" }
    }
  }
}
```

## Docs

- Full machine-readable docs: https://textforagents.com/products/mcp-answer-quality-canary/llms.txt
- OpenAPI: https://textforagents.com/products/mcp-answer-quality-canary/openapi.json
- A2A agent card: https://textforagents.com/agent-cards/mcp-answer-quality-canary.json
- Catalog: https://textforagents.com/products/ ("Other Products")

Provider: TextForAgents LLC · Support: support@textforagents.com
