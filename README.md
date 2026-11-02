# Bin Zhang

**Senior Backend & AI Engineer | Go, Python, FastAPI**

I build reliable backend services, API integrations, and AI-enabled workflows. I have 9+ years of engineering experience at ByteDance and Tencent, with a focus on distributed systems, high-concurrency services, and production-ready automation.

Based in Beijing, China. Open to remote backend, API integration, and AI engineering projects.

## What I build

- **Backend systems:** Go and Python microservices, REST APIs, background jobs, and event-driven workflows.
- **Data and infrastructure:** PostgreSQL, MySQL, Redis, Docker, and cloud deployments.
- **AI applications:** FastAPI services, LLM integrations, RAG, tool calling, and human-in-the-loop automation.
- **Reliability work:** Idempotency, rate limiting, retries, failure recovery, observability, and performance debugging.

## How I work

- Start with a clear input, expected output, and acceptance criteria.
- Use explicit state machines and deterministic workflows where they are simpler than autonomous agents.
- Design for timeouts, duplicate requests, partial failures, and third-party API limits.
- Keep secrets and personal data out of logs, and test critical failure paths.
- Deliver readable code, setup instructions, and practical operational documentation.

## Selected experience

### ByteDance / TikTok — Senior Backend Engineer

Go and Python microservices for search ad creative workflows, global traffic serving, and high-throughput AIGC asset processing. Work includes rate-limit governance, fault tolerance, distributed systems, and automated operations.

### Tencent — Senior Backend Engineer

Backend architecture for operational automation, including state machines for batch task dispatch, reliable message-notification pipelines, and compensation for partially completed workflows. Also helped drive an education product from its initial MVP to commercialization.

## Featured projects

### [fastapi-reliable-integration-lab](https://github.com/halibut735/fastapi-reliable-integration-lab)

Production-grade reliable third-party API integration pattern built with **FastAPI**, **SQLAlchemy (Async)**, and explicit state machines:
- **DB-enforced idempotency:** Unique constraint on `idempotency_key` prevents duplicate processing and double charges.
- **Explicit deterministic state machine:** Clear transitions across received, in-progress, retry scheduled, ambiguous, and terminal states.
- **Controlled fault injection mock:** Simulates upstream timeouts, 429 rate limits with `Retry-After`, and in-flight gateway disconnects.
- **Reconciliation workflow:** Authoritative partner status queries resolve ambiguous network drops without blind retries.
- **Bounded async workers & backoff:** Concurrency-limited worker pool with full jitter exponential backoff.
- **Redacted structured logging:** Automatically masks tokens, Authorization headers, signatures, and synthetic PII.
- **Docker Compose & automated tests:** Complete test suite verifying failure recovery and edge cases.

## Current focus

Publishing practical backend and AI engineering demos with runnable quickstarts, automated tests, failure scenarios, and clear limitations. Next focus: a bounded-concurrency Go worker pool lab covering context timeouts, race detection, and observability.
