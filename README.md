## Dhaval Patel

**Senior Backend Engineer**: distributed systems, high-throughput APIs, payments.<br>
Ahmedabad, India · open to remote · [LinkedIn](https://www.linkedin.com/in/dhaval-patel-14a06a194)

I design and run backend systems where latency, correctness and failure handling matter.
8+ years across payments, merchant-data platforms and business-process automation.

### Selected work

- **12K TPS data API.** Owned design and delivery of a reactive merchant-data service, in production at p95 68 ms / p99 125 ms. Its layered read path (Elasticsearch → retry → YugabyteDB fallback) keeps data available when one store fails.
- **Latency under load.** Traced the degradation to TLS-handshake and connection-acquisition delays with thread and TCP dumps, then moved the data layer from a blocking JDBC driver to a non-blocking client.
- **Payments correctness.** Idempotent Kafka consumers that record event IDs in the same transaction as the read model, with dead-letter routing. Optimistic locking on refund state. Charge and refund workflows on Step Functions with per-step retries and duplicate-event detection.
- **Early-stage ownership.** Sole backend engineer at a payments startup: GraphQL and REST APIs for merchant dashboards, DataLoader batching to remove N+1 queries, partial responses when a downstream dependency fails.
- **Runtime expression engine.** A service that evaluates user-written JavaScript and Python on GraalVM Polyglot to transform and validate datasets, called from business rules.
- **Migrations.** JDK 8 → 17, Ant → Gradle, blocking → reactive I/O, container-aware JVM memory sizing on Kubernetes.

### How I work

- **Measure first.** Load and soak tests, with p95/p99 numbers before and after each change.
- **Design for failure.** Bounded retries, circuit breakers, dead-letter queues and graceful degradation.
- **Ship safely.** Coverage gates and security scans in CI, blue-green deploys, versioned schema migrations.

### Open source

| Project | Contribution | Status |
|---|---|---|
| [miurla/morphic](https://github.com/miurla/morphic) | [#671](https://github.com/miurla/morphic/pull/671): fix for issue #546 | Merged |
<!-- Add a row for each merged PR: | [org/repo](link) | [#123](pr-link): what it changed | Merged | -->

### Toolbox

- **Languages:** Java · TypeScript · Python · SQL
- **Systems:** Spring Boot · Vert.x · Kafka · RabbitMQ · GraphQL · gRPC · PostgreSQL · Elasticsearch · AWS · Kubernetes
- **Exploring:** real-time voice AI ([Pipecat](https://github.com/pipecat-ai/pipecat)) · LLM agent tooling (MCP)
