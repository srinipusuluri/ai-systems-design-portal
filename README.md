# AI Systems Design Portal

A single-page learning portal for **production AI systems design**: the engineering fundamentals that keep LLM applications, RAG pipelines and agent platforms fast, reliable, secure and affordable at scale.

Open [`ai-systems-design-portal.html`](ai-systems-design-portal.html) in any modern browser. There is no build step and nothing to install.

## What's inside

### 12 fundamentals

Each module covers one core engineering question and includes concept cards, Mermaid diagrams, code samples, trade-off tables, pitfalls, external resources and a self-check.

| # | Module | Core question |
|---|--------|---------------|
| 01 | Rate limiting | How do we control request volume? |
| 02 | Streaming | How do we return responses progressively? |
| 03 | Idempotency | How do we prevent duplicate operations? |
| 04 | LLM serving | How do we serve models efficiently? |
| 05 | Batching | How do we process multiple requests efficiently? |
| 06 | Caching | How do we avoid repeated computation? |
| 07 | Reliability | How do we keep systems operational? |
| 08 | Privacy & security | How do we protect sensitive data? |
| 09 | Load balancing | How do we distribute workloads? |
| 10 | Backpressure | How do we prevent overloaded services from collapsing? |
| 11 | Observability | How do we understand system behavior? |
| 12 | Cost optimization | How do we control inference and infrastructure costs? |

### Putting it together

- **Enterprise AI reference architecture**: API gateway, AI gateway, agent orchestrator, RAG engine, tool layer, LLM serving and response processing, mapped to the fundamentals each one applies.
- **Five enterprise scenarios**: fintech payment agent, customer service agent, voice AI agent, enterprise RAG platform and multi-agent platform.
- **Design decision matrix**: 12 questions to answer before going to production.

### Interactive labs

1. **Token bucket rate limiter**: adjust capacity, refill rate and cost, then send bursts and watch requests get accepted or rejected with 429.
2. **Exponential backoff with full jitter**: see the delay cap and a random sample for each retry attempt.
3. **Availability calculator**: convert an SLA into allowed downtime, and compute end-to-end availability across serial dependencies.
4. **Token cost estimator**: estimate daily and monthly spend, with settings for cache hit rate and routing to a smaller model. The prices are placeholders; enter your provider's current rates.

### Practice

- **6-week roadmap**: a checklist from distributed-systems basics to production engineering.
- **Knowledge check**: 14 scenario questions with explanations.
- **Capstone project**: an enterprise AI gateway built with FastAPI, Redis, Kafka, PostgreSQL/pgvector, vLLM, SSE streaming, an agent orchestrator and OpenTelemetry.
- **Resource library**: 55 searchable links to books, papers, docs and courses.

## Features

- Light and dark themes. The page follows your OS setting, and the toggle overrides it.
- Module completion, roadmap progress and quiz answers are saved in your browser's `localStorage`. They are never sent anywhere.
- Responsive layout with a collapsible sidebar on mobile.
- Diagrams render with [Mermaid](https://mermaid.js.org/) 10.9.1, loaded from jsDelivr. **Diagrams need an internet connection**; offline, the rest of the page still works.

## Hosting with GitHub Pages

1. Go to **Settings → Pages** in this repository.
2. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
3. The portal will be served at
   `https://srinipusuluri.github.io/ai-systems-design-portal/ai-systems-design-portal.html`

## Notes

Example limits, latencies, token counts and costs are illustrative, not universal defaults. External links point to third-party sites and may change over time.
