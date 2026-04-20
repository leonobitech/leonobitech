<div align="center">

# ![Typing](https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=700&size=32&duration=3500&pause=1000&color=F77208&center=true&vCenter=true&width=820&height=80&lines=Leonobitech;AI-Driven+Automation+for+SMBs;Agents+%C2%B7+Pipelines+%C2%B7+Production+Infra)

### 🚀 Transform Your Business with AI-Driven Solutions

**Production AI automation** — we ship **complete agent stacks** for sales, bookings, and customer service to small & medium businesses in **LATAM**.

<br>

<a href="https://www.leonobitech.com/"><img alt="Website" src="https://img.shields.io/badge/🌐_leonobitech.com-F77208?style=for-the-badge&logoColor=white"/></a>&ensp;
<a href="https://github.com/leonobitech"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>&ensp;
<img alt="Status" src="https://img.shields.io/badge/live_in_production-success?style=for-the-badge"/>&ensp;
<img alt="Region" src="https://img.shields.io/badge/🌎_LATAM-0A66C2?style=for-the-badge&logoColor=white"/>

<br><br>

**📊 Shipping in real-time →**

<a href="https://github.com/leonobitech/backend"><img alt="backend" src="https://img.shields.io/github/last-commit/leonobitech/backend?label=backend&style=flat-square&color=F77208"/></a>&ensp;
<a href="https://github.com/leonobitech/frontend"><img alt="frontend" src="https://img.shields.io/github/last-commit/leonobitech/frontend?label=frontend&style=flat-square&color=F77208"/></a>&ensp;
<a href="https://github.com/leonobitech/agents"><img alt="agents" src="https://img.shields.io/github/last-commit/leonobitech/agents?label=agents&style=flat-square&color=F77208"/></a>&ensp;
<a href="https://github.com/leonobitech/hardware"><img alt="hardware" src="https://img.shields.io/github/last-commit/leonobitech/hardware?label=hardware&style=flat-square&color=F77208"/></a>&ensp;
<a href="https://github.com/leonobitech/mcp-infrastructure"><img alt="mcp-infra" src="https://img.shields.io/github/last-commit/leonobitech/mcp-infrastructure?label=mcp-infra&style=flat-square&color=F77208"/></a>

</div>

---

## 🎯 What we build

We build the **intelligence layer** that operates your business — the agents that talk to your customers, the pipelines that automate your workflows, the integrations that connect your existing stack (CRM, databases, messaging) to **Claude** and orchestrate it all.

End-to-end: **the agents themselves, the production infrastructure, and the custom MCP servers** that connect Claude to the tools your business already uses. No duct-tape, no demos that break in prod — real systems running 24/7 on our VPS.

---

## 🎯 Why Leonobitech

- **We ship, we don't prototype.** Every system here runs in production, not in a demo video.
- **Full-stack accountability.** From the agent prompts to the Docker containers — one team owns the whole pipeline.
- **Claude-native architecture.** Built on Anthropic's stack, deeply integrated through custom MCP servers.
- **LATAM-priced, US-quality engineering.** SMB-friendly pricing without compromises on architecture or reliability.

---

## 💼 Product Suite

| Product | What it does |
|---------|--------------|
| 💬 **WhatsApp Sales Agent** | Qualifies inbound leads 24/7. Identifies intent, scores prospects, hands off qualified conversations to the sales team with full context. |
| 📅 **Booking Agent** | Schedules meetings across the team's calendars, confirms via WhatsApp/email, generates payment links end-to-end. |
| 🎙️ **Voice AI Agent** | Realtime conversational interface for inbound calls. Optional **3D avatar** (LemonSlice) for brand presence. Built on LiveKit. |
| 🧩 **Custom MCP Integrations** | We connect Claude to your existing stack — Odoo CRM, Baserow, n8n workflows, WhatsApp Business API, custom databases. |
| 🧠 **RAG Pipelines** | Context-aware AI answers grounded in your documents, FAQs, and product data using **Qdrant** as the vector store. |
| 🇦🇷 **Argentina Fiscal Compliance** | **Odoo 19** with AFIP/ARCA electronic invoicing (WSAA/WSFE) out of the box. |

---

## 🏗 Under the Hood — What's Running in Production

```
┌─── VPS · 30 containers · Docker Compose · Traefik + Core (auth) ────┐
│                                                                     │
│  🤖 AI / LLM Layer                                                  │
│     • Claude (Anthropic)   (reasoning & orchestration)              │
│     • Custom MCP servers   (Odoo · n8n · Baserow · SSH · Notion)    │
│     • Qdrant               (vector DB for RAG pipelines)            │
│     • LiveKit + voice AI   (realtime conversational + 3D avatars)   │
│     • n8n                  (1,084 nodes · workflow orchestration)   │
│                                                                     │
│  💼 Business Systems                                                │
│     • Odoo 19              (ERP + Argentina ARCA e-invoicing)       │
│     • Baserow              (no-code DB · 8 tables)                  │
│     • Chatwoot             (customer messaging)                     │
│                                                                     │
│  🚀 Product Stack                                                   │
│     • Frontend             (Next.js 15 · TS · Docker)               │
│     • Backend              (Node · TS · Hexagonal · ESM · Rust)     │
│     • Hardware             (ESP32-C3 · Rust · Secure Boot)          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

---

## 🎯 Product Repos

| Repo | Stack | Role |
|------|-------|------|
| 🎨 [**frontend**](https://github.com/leonobitech/frontend) | Next.js · TypeScript | Customer-facing UI |
| ⚙️ [**backend**](https://github.com/leonobitech/backend) | Node · TypeScript · Hexagonal · Rust | Core API + 15 microservices mono-repo |
| 🔌 [**hardware**](https://github.com/leonobitech/hardware) | Rust · ESP32-C3 · ESP-IDF | IoT firmware with Secure Boot |
| 🎙️ [**agents**](https://github.com/leonobitech/agents) | Python · Realtime | Voice AI agents framework |

---

## 💎 Inside [`backend/repositories/`](https://github.com/leonobitech/backend/tree/main/repositories)

Our backend is a **mono-repo with 15 production microservices**, grouped by role:

<table>
<tr>
<td valign="top" width="50%">

**🎙️ Voice AI stack**

- [voice-agent](https://github.com/leonobitech/backend/tree/main/repositories/voice-agent) · LiveKit realtime
- [voice-agent-3D](https://github.com/leonobitech/backend/tree/main/repositories/voice-agent-3D) · LemonSlice avatar
- [voice-spike](https://github.com/leonobitech/backend/tree/main/repositories/voice-spike) · WebRTC · Piper TTS
- [livekit](https://github.com/leonobitech/backend/tree/main/repositories/livekit) · Production-hardened
- [piper-tts](https://github.com/leonobitech/backend/tree/main/repositories/piper-tts) · TTS service

</td>
<td valign="top" width="50%">

**🦀 Core services**

- [core-v2](https://github.com/leonobitech/backend/tree/main/repositories/core-v2) · Rust microservice foundation
- [core](https://github.com/leonobitech/backend/tree/main/repositories/core) · Infra + auth
- [Qdrant](https://github.com/leonobitech/backend/tree/main/repositories/Qdrant) · Vector DB for RAG

</td>
</tr>
<tr>
<td valign="top" width="50%">

**🤖 AI & business integrations**

- [1-appointment-agent](https://github.com/leonobitech/backend/tree/main/repositories/agents/leonobitech/1-appointment-agent) · Booking AI
- [odoo-mcp](https://github.com/leonobitech/backend/tree/main/repositories/odoo-mcp) · Odoo MCP server
- [odoo](https://github.com/leonobitech/backend/tree/main/repositories/odoo) · ERP config

</td>
<td valign="top" width="50%">

**🛠️ Supporting infra**

- [n8n](https://github.com/leonobitech/backend/tree/main/repositories/n8n) · Workflows
- [baserow](https://github.com/leonobitech/backend/tree/main/repositories/baserow) · No-code DB
- [redis](https://github.com/leonobitech/backend/tree/main/repositories/redis) · Cache
- [wa-signature-proxy](https://github.com/leonobitech/backend/tree/main/repositories/wa-signature-proxy) · WhatsApp proxy

</td>
</tr>
</table>

---

## 📦 Open-Source Blueprints

We open-source **reusable templates** for teams building AI-driven systems:

| Repo | What you get |
|------|--------------|
| 🔥 [**fullstack-mcp-playground**](https://github.com/leonobitech/fullstack-mcp-playground) ⭐ | Fullstack AI agent template — Claude + microservices + modular tools from UI gallery |
| 🛰️ [**remote-connector-claude**](https://github.com/leonobitech/remote-connector-claude) | Remote MCP Connector for Claude Desktop |
| 🧩 [**mcp-infrastructure**](https://github.com/leonobitech/mcp-infrastructure) | Operate a full VPS (n8n · Baserow · SSH · Notion) from Claude Code via natural language |
| 🐳 [**fullstack-infrastructure-blueprint**](https://github.com/leonobitech/fullstack-infrastructure-blueprint) | Docker · Traefik · HTTPS grid |
| 🎨 [**fullstack-frontend-core**](https://github.com/leonobitech/fullstack-frontend-core) | Next.js 15 · TS (ESM) · Docker |
| ⚙️ [**fullstack-backend-core**](https://github.com/leonobitech/fullstack-backend-core) | Hexagonal API · Node · TS · ESM |
| 🇦🇷 [**l10n_ar_arca_edi**](https://github.com/leonobitech/l10n_ar_arca_edi) | Odoo 19 · ARCA Electronic Invoicing (WSAA/WSFE) |
| 🇦🇷 [**l10n-argentina**](https://github.com/leonobitech/l10n-argentina) | Odoo modules for Argentina |

---

## 🛠 Tech Stack

**AI / LLM / Automation**

![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![Anthropic API](https://img.shields.io/badge/Anthropic_API-191919?style=for-the-badge&logo=anthropic&logoColor=white)
![MCP](https://img.shields.io/badge/Model_Context_Protocol-000000?style=for-the-badge)
![LiveKit](https://img.shields.io/badge/LiveKit-00C3B5?style=for-the-badge&logo=livekit&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant_(RAG)-DC244C?style=for-the-badge)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Odoo](https://img.shields.io/badge/Odoo-714B67?style=for-the-badge&logo=odoo&logoColor=white)

**Languages**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)

**Infrastructure**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-24A1C1?style=for-the-badge&logo=traefikproxy&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Baserow](https://img.shields.io/badge/Baserow-1F2937?style=for-the-badge)
![Chatwoot](https://img.shields.io/badge/Chatwoot-1F93FF?style=for-the-badge)

**Frontend & Backend**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Tokio](https://img.shields.io/badge/Tokio-232323?style=for-the-badge)

**Embedded & IoT**

![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![RISC-V](https://img.shields.io/badge/RISC--V-283272?style=for-the-badge&logo=riscv&logoColor=white)

---

## 👤 Built by

**[Felix M. Figueroa](https://github.com/FMFigueroa)** — Senior Software Engineer, AI + LLM systems, founder of Leonobitech.

- 6+ years shipping software across web, backend, and API systems
- 3+ years deep in AI and LLM-based systems
- Currently orchestrating agents and pipelines for real workflow automation

👉 Check his personal GitHub **[@FMFigueroa](https://github.com/FMFigueroa)** for the broader engineering portfolio (Rust embedded, IoT, systems programming, and more).

---

## 📬 Let's Talk

Automating a workflow for your business? Scaling a sales pipeline? Deploying a voice agent?

<div align="center">

### 🚀 [**leonobitech.com →**](https://www.leonobitech.com/)

*AI automation for SMBs · Built in LATAM · Shipping to production*

</div>
