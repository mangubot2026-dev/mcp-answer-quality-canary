# Error-Actionability Translation for MCP Tool Failures

Classifies MCP tool failures (bare isError + prose) into host-enforced recovery verdicts - category, retryable, retry-after, repair target, replay-safety - from per-server error-dialect profiles; strips raw prose from model context and refuses unsafe resends at the gateway. Solo $9/mo, Fleet $19/mo, verdict API $0.002 per check via x402; first month free once per operator.

## Connect (remote MCP, streamable HTTP)

- MCP endpoint: `https://textforagents.com/products/error-actionability-translation/mcp`
- Transport: streamable HTTP (also accepts POST at the product base URL)
- Auth: `Authorization: Bearer <token>` — get a token self-serve:
  `POST https://textforagents.com/products/error-actionability-translation/register` then
  `POST /trial` (one-time free trial) or `POST /subscribe` (x402, Base USDC).

Example client config:

```json
{
  "mcpServers": {
    "error-actionability-translation": {
      "url": "https://textforagents.com/products/error-actionability-translation/mcp",
      "headers": { "Authorization": "Bearer <your-token>" }
    }
  }
}
```

## Docs

- Full machine-readable docs: https://textforagents.com/products/error-actionability-translation/llms.txt
- OpenAPI: https://textforagents.com/products/error-actionability-translation/openapi.json
- A2A agent card: https://textforagents.com/agent-cards/error-actionability-translation.json
- Catalog: https://textforagents.com/products/ ("Other Products")

Provider: TextForAgents LLC · Support: support@textforagents.com
