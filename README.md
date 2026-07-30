<div align="center">

<!-- Animated typing header -->
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=26&duration=3500&pause=1200&center=true&vCenter=true&width=720&lines=Raveesh+Agarwal;Commerce+infrastructure+for+an+AI-native+world;Go+%C2%B7+ConnectRPC+%C2%B7+Kubernetes+%C2%B7+MCP" alt="Raveesh Agarwal" />

**Director of Engineering, Commerce · [HighLevel](https://www.gohighlevel.com)**

*Building the systems that let millions of small businesses sell, invoice, and get paid.*

<br/>

[![Blog](https://img.shields.io/badge/Blog-Writing%20on%20cloud--native%20%26%20APIs-1a1a2e?style=for-the-badge&logo=hashnode&logoColor=white)](https://your-blog-url.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/your-handle)
[![Patent](https://img.shields.io/badge/US%20Patent-12%2C316%2C707%20B1-2d6a4f?style=for-the-badge&logo=googlescholar&logoColor=white)](https://patents.google.com/patent/US12316707B1)

</div>

---

## 🎯 Focus

Systems that scale across four hard axes:

| Axis | What it means in practice |
|---|---|
| 🌊 **Millions of sessions** | Checkout, invoicing, and document surfaces that hold up under real merchant traffic |
| 🛰️ **Distributed app fleets** | Multi-tenant services on GKE with strict service boundaries and mTLS everywhere |
| 🌍 **Global commerce constraints** | Payments, tax, compliance, and currency realities across markets |
| 🤝 **Human + AI workflows** | APIs designed so agents and people operate the same platform through the same contracts |

---

## 🏗️ How I design systems

Every system I build settles into the same shape — a layered substrate where each layer absorbs a class of problems so the layers above stay simple:

```mermaid
flowchart TB
    subgraph OPS["🧑‍💻 Operators — humans and agents, one front door"]
        HUMAN["Human interfaces"]
        AGENT["AI agents"]
    end

    subgraph CONTRACT["📜 Contract boundary — the schema leads"]
        SCHEMA["One definition → clients · servers · docs · agent tool manifests"]
    end

    subgraph DOMAIN["⚙️ Domain space — where complexity lives"]
        INV["Invariants enforced once, everywhere"]
        IDEM["Idempotency as a platform guarantee"]
        IMMUT["Immutable records · correction by append"]
    end

    subgraph SUB["🧱 Substrate — reliability primitives"]
        MESH["Zero-trust service mesh"]
        AUTHZ["Relationship-based authorization"]
        TRUTH["Double-entry truth store"]
        CACHE["Tiered caching"]
    end

    HUMAN --> SCHEMA
    AGENT --> SCHEMA
    SCHEMA --> DOMAIN
    DOMAIN --> SUB
```

The pattern behind the layers: complexity flows downward until it reaches the layer built to own it. Operators — human or agent — see one contract. The contract generates everything downstream. The domain enforces every invariant exactly once. The substrate makes correctness the default rather than a per-feature effort.

---

## 🧰 Depth

### Backend
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![ConnectRPC](https://img.shields.io/badge/ConnectRPC-161B22?style=flat-square&logo=buf&logoColor=white)
![Protobuf](https://img.shields.io/badge/Protocol%20Buffers-4285F4?style=flat-square&logo=google&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Istio](https://img.shields.io/badge/Istio-466BB0?style=flat-square&logo=istio&logoColor=white)
![GCP](https://img.shields.io/badge/GKE-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![TigerBeetle](https://img.shields.io/badge/TigerBeetle-F2A900?style=flat-square&logoColor=white)
![Temporal](https://img.shields.io/badge/Temporal-000000?style=flat-square&logo=temporal&logoColor=white)
![CNCF](https://img.shields.io/badge/CNCF-231F20?style=flat-square&logo=cncf&logoColor=white)
![AAIF](https://img.shields.io/badge/AAIF-0086FF?style=flat-square&logo=linuxfoundation&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-1a1a2e?style=flat-square&logo=modelcontextprotocol&logoColor=white)

- Service boundaries as a first-class design artifact — domain tiers, experience tiers, and per-niche translators
- Financial-grade data modeling: immutable documents, double-entry ledgers, idempotency as a platform guarantee
- Relationship-based authorization (ReBAC) for agency → location → resource hierarchies
- AI-first orchestration: protobuf-annotated services that self-describe as MCP tools

### Frontend
![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![PWA](https://img.shields.io/badge/Mobile%20Web%20Specialist-5A0FC8?style=flat-square&logo=pwa&logoColor=white)

- Large-scale state & caching systems
- Modular distribution architectures for app fleets
- BFF systems evolved into per-niche translation layers
- 📜 **US Patent 12,316,707 B1**

---

## 🤖 AI-native infrastructure

The interesting question of this decade: what does a commerce platform look like when its primary operators include software agents?

My current answers, in code and writing:

- **Protobuf → MCP codegen** — generating Model Context Protocol tool manifests directly from service definitions, so the API contract and the agent contract stay one artifact
- **Governance-aware annotations** — tool-level metadata (risk, side-effects, tenancy) declared in the schema, enforced at the boundary
- **ConnectRPC in production** — one wire contract serving browsers, mobile, service-to-service traffic, and agents

### 🔭 Active exploration

- **Durable execution with Temporal** — long-running workflows (migrations, replays, reconciliation, agent task chains) modeled as durable, resumable programs, so a crashed process resumes exactly where it stopped
- **AI governance** — how policy, risk tiers, audit trails, and human-approval gates attach to agent-invocable tools: declared in the schema, enforced at runtime, reviewable after the fact

---

## 🧑‍✈️ Engineering leadership

Leading two organizations at once: six years building the mobile organization to 20+ engineers, and the past year building the commerce organization to 40+ engineers across seven teams. How I run things:

- **User experience as proof of work** — took the mobile platform from 6,000 MAU and declining to 600,000 MAU and climbing: a 100× turnaround over five years, earned through platform rewrites, large-scale state & caching work, and modular distribution
- **Cadence as infrastructure** — the org runs on written, reviewable artifacts: team charters, quarterly business reviews, leveling memos, and recognition that names specific work. If it matters, it has a document and a rhythm
- **Teams that operate without a manager** — every engineer owns a single, clearly written charter; decisions route through the charter and the contract, so the team keeps shipping when any one person (including me) steps away
- **Coresphere** — a co-authored design philosophy for the platform's surfaces: nine tenets, with external builders treated as a first-class audience from day one

---

## 🧭 Philosophy

> Great engineering moves complexity out of the user space and into the system space.

- **Eliminate classes of problems.** A fixed bug helps once; a fixed invariant helps forever.
- **Reliability protects revenue.** Every 9 in a checkout path has a dollar value.
- **Abstractions compound.** The right primitive today is a hundred features tomorrow.
- **Platform empathy.** Build every internal surface as if you personally get paged for its rough edges.
- **Contracts first.** When the schema leads, the docs, clients, and agents all follow for free.

---

## 🌱 Community & beyond

- 🎤 Active in the cloud-native and MCP ecosystems — KubeCon + CloudNativeCon India, Open Source Summit India, MCP Dev Summit
- 🌉 Building internship pipelines that bring open-source contributors (GSoC / LFX alumni) into production engineering teams
- ✍️ Writing about Kubernetes, API architecture, and building agent-ready platforms
- 🎸 Chasing clean tones on a Yamaha Strat; listening on far-too-carefully-chosen IEMs
- 🥭 Planting a mango orchard in Jharkhand — the ultimate exercise in long-term systems thinking: water infrastructure first, harvest ladder second, patience throughout
- 🛸 Logging training hours in FPV drone simulators — acro mode is muscle memory earned one crash at a time

---

## 🎯 Direction

**Accessible, intelligent commerce infrastructure for SMBs worldwide** — where a two-person business gets the same financial substrate, the same reliability, and the same AI leverage as an enterprise.

---

<div align="center">

<!-- GitHub stats — replace username; delete this block if you prefer a quieter profile -->
<img src="https://github-readme-stats.vercel.app/api?username=raveesh-me&show_icons=true&theme=github_dark&hide_border=true&count_private=true" alt="GitHub stats" height="160"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=raveesh-me&layout=compact&theme=github_dark&hide_border=true" alt="Top languages" height="160"/>

<br/><br/>

*Systems worth building are the ones still running when you've moved on.*

</div>
