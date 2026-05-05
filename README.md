# MeshToken API Documentation

> OpenAI-compatible API for distributed AI inference. Cheaper, faster, mesh-powered.

## Quick Start

```bash
curl https://api.meshtok.com/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer $MESHTOK_API_KEY" \
  -d '{
    "model": "mesh/qwen-7b",
    "messages": [{"role": "user", "content": "Hello!"}]
  }'
```

## Supported Models

| Model ID | Provider | Mode |
|----------|----------|------|
| `mesh/qwen-7b` | Distributed Network | eco |
| `openai/gpt-4o` | OpenAI | fast |
| `anthropic/claude-sonnet-4` | Anthropic | fast |
| `deepseek/deepseek-v3` | DeepSeek | fast |

## Modes

- **fast** — Direct API relay. Lowest latency. Standard pricing.
- **eco** — Distributed inference via idle compute nodes. ~50-80% cheaper. Slightly higher latency.

## SDK Examples

- [Python](./examples/python)
- [JavaScript](./examples/javascript)
- [cURL](./examples/curl)

## Project Roadmap

See [MESHTOK_PLAN.md](./MESHTOK_PLAN.md)

## License

MIT
