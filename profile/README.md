# PromptJang — พร้อมแจ้ง

**Async reliability and observability for webhook delivery.**

Webhooks fail silently. Retries are hard to get right. Observability is an afterthought. PromptJang fixes all three — so you can focus on building your product, not debugging delivery.

PromptJang (พร้อมแจ้ง) means *"Ready to Inform"* in Thai. Every webhook you send is tracked, retried with exponential backoff, and delivered with full visibility into what happened and when.

## What PromptJang Does

- **Reliable Delivery** — Automatic retries with exponential backoff. Events flow through a state machine: `Queued → Processing → Delivered`. If delivery fails, PromptJang retries up to the configured limit, then marks the event as expired with a full audit trail.
- **HMAC Signature Verification** — Every inbound event is verified against an HMAC-SHA256 signature. No unsigned payloads reach your endpoints.
- **Event Replay** — Re-deliver any past event with one API call. Useful for recovering from downstream outages without re-processing from source.
- **SSRF Protection** — Webhook target URLs are validated against private IPs, localhost, link-local, and carrier-grade NAT ranges. No internal network exposure.
- **Delivery Observability** — Track every delivery attempt: HTTP status code, response body, latency, and error details. Know exactly what happened and when.
- **Per-Tenant Isolation** — Organizations, API keys, and endpoints are fully isolated. Cross-tenant access is enforced at every layer.

## Tech Stack

Built for the edge, with security and performance as first-class concerns:

| Layer | Technology |
|---|---|
| Runtime | Rust on Cloudflare Workers (WebAssembly) |
| Database | Cloudflare D1 (SQLite at the edge) |
| Object Storage | Cloudflare R2 (event payloads) |
| Message Queue | Cloudflare Queues (delivery pipeline) |
| Cache | Cloudflare KV (rate limiting) |
| Billing | Stripe |

## Links

- **Website**: [promptjang.net](https://promptjang.net) — coming soon
- **Docs**: [docs.promptjang.net](https://docs.promptjang.net) — coming soon

## License

All projects are licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Contact

- Facebook: [Thanaphoom Babparn](https://www.facebook.com/thanaphoom.mart/)
- LinkedIn: [Thanaphoom Babparn](https://www.linkedin.com/in/thanaphoom-babparn/?locale=en_US)
- Website: [TP Coder — Portfolio](https://portfolio.tpcoder.dev/)
