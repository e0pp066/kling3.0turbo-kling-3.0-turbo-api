# Kling 3.0 Turbo API (kling-3.0-turbo / kling3.0turbo) — api guide with published pricing

> **720P $0.1144; 1080P $0.1432** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-3338dd)** · **[Get an API key](https://go.apimart.ai/k-4d686f)**

Everything here refers to **kling-3.0-turbo** — also written **kling3.0turbo** or **kling 3.0 turbo**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `720P` | $0.1144 |
| `1080P` | $0.1432 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $11.44 |
| 1,000 | $114.4 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/videos/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"kling-3.0-turbo","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
