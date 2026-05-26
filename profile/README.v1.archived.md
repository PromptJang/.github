# PromptJang - พร้อมแจ้ง

Welcome to **PromptJang** (พร้อมแจ้ง), the open-source **Flight Recorder and Communication Bus for AI Agents**.

As the agent economy scales, AI systems need a safe, reliable, and trackable way to communicate with external APIs, other agents, and human operators. PromptJang moves beyond simple B2C notifications, providing a high-performance routing, governance, and observability layer designed specifically for human notification, callback notifier layer, and your AI Agent mailbox.

**Our Vision: The standard, secure communication layer for the AI Agent ecosystem.**

This organization serves as our open-source home. We are building developer-first infrastructure that ensures agent communications are structured, traceable, and safe—from local testing to distributed enterprise production.

## 🚀 Core Capabilities

  * **Agent-First Ingress (HTTP & MCP):** Native Webhook endpoints and Model Context Protocol (MCP) integration, allowing LLMs to discover and use PromptJang as a native tool instantly.
  * **Intent-Based Routing:** Stop hardcoding API integrations in your agent prompts. Emit an intent, and let PromptJang validate the JSON schema (bouncing hallucinations) and route it to the correct downstream system.
  * **The "Flight Recorder" (Observability):** Deep trace visibility into every payload. Track token usage, latency, and view sequence diagrams of multi-agent negotiations.
  * **Enterprise Governance:** Built-in middleware for PII masking, rate limiting, and exact-once delivery semantics (Idempotency).
  * **Multi-Channel Egress:** Seamlessly fan-out payloads to other AI Agent webhooks, enterprise chat (Slack, Discord), or traditional human channels (Email, Push).
  * **Progressive Architecture:** Run as a zero-config, single binary monolith for local development, or scale out to a distributed Pub/Sub consumer architecture using Redis/Postgres for production.

## 💡 About the Name

"PromptJang" (พร้อมแจ้ง) is a Thai phrase meaning *"Ready to Inform."* It reflects our mission: ensuring your infrastructure is always ready to receive prompts, route intents, and deliver agent communications securely and reliably.

## 📄 License

All core projects within this organization are licensed under the [MIT License](https://www.google.com/search?q=LICENSE), keeping the foundation open and accessible for all developers.

## 📬 Contact & Maintainers

For any inquiries, architectural discussions, or feature suggestions, please open an issue on the relevant repository.

**Connect with the creator:**

  * Facebook: [Thanaphoom Babparn](https://www.facebook.com/thanaphoom.mart/)
  * FB Page: [TP Coder](https://www.facebook.com/tpcoder)
  * LinkedIn: [Thanaphoom Babparn](https://www.linkedin.com/in/thanaphoom-babparn/?locale=en_US)
  * Website: [TP Coder — Portfolio](https://portfolio.tpcoder.dev/)

-----

*Thank you for visiting PromptJang\! Let's build the future of agent infrastructure.*
