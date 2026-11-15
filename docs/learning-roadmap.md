# Learning roadmap

A 12-week plan, about one hour a day. Each week has one topic and one design exercise taken from systems I have already built, so the theory is tied to real code.

**Focus:** system design first, then SQL depth, with spoken English practised every day alongside.

## Weeks 1–8: system design

| Week | Topic | Design exercise |
|---|---|---|
| 1 | How to run a design discussion: requirements, load estimates, API, data model, bottlenecks, trade-offs | Write up the multi-store platform in that format, on one page |
| 2 | Scaling and load balancing: vertical vs horizontal, stateless services, autoscaling, cold starts | Size the order API for 10x the current stores |
| 3 | Caching: cache-aside, TTL, invalidation, CDN, Redis | Add a cache to the cross-store order list and define when it is invalidated |
| 4 | Queues and events: at-least-once delivery, idempotency, retries, dead-letter queues, ordering | Design webhook intake for 1,000 events per second |
| 5 | Databases at scale: replication, partitioning, sharding keys, hot partitions | Choose a partition key for orders across many stores and defend it |
| 6 | Consistency: CAP, transactions, sagas, outbox pattern, exactly-once myths | Keep an order and its refund consistent across two services |
| 7 | Reliability: timeouts, circuit breakers, rate limiting, backpressure, graceful degradation | Design a rate limiter for a third-party API with a shared quota |
| 8 | Observability and cost: metrics, logs, traces, SLOs, alerting, cost per request | Define SLOs and alerts for shipment tracking sync |

## Weeks 9–10: SQL depth

| Week | Topic | Exercise |
|---|---|---|
| 9 | Indexes and query plans: B-tree, composite and covering indexes, `EXPLAIN ANALYZE` | Take three slow PostgreSQL queries and make them fast, with before/after plans |
| 10 | Transactions: isolation levels, locks, deadlocks, MVCC; SQL vs NoSQL trade-offs | Model the order data in PostgreSQL and in Firestore, and compare both |

## Weeks 11–12: classic designs, end to end

| Week | Exercise |
|---|---|
| 11 | Notification system; URL shortener; news feed — 45 minutes each, written, then reviewed against a reference answer |
| 12 | Order and payment system; multi-tenant SaaS — presented out loud in English, recorded and reviewed |

## Every day, in parallel

- **English speaking, 20–30 minutes:** explain that day's topic out loud. Goal by week 12: present a system design for 10 minutes without notes.
- **Algorithms, 2–3 problems a week:** arrays, hash maps, trees, graphs, at easy and medium level.

## After week 12

- Google Cloud Associate Cloud Engineer certification.
- Leadership practice with numbers: estimates vs actuals, incident postmortems, release lead time.

## Sources

- Alex Xu, *System Design Interview*, volumes 1 and 2
- Martin Kleppmann, *Designing Data-Intensive Applications*
- `donnemartin/system-design-primer` on GitHub
- *Use The Index, Luke* (use-the-index-luke.com) for SQL indexing
- PostgreSQL documentation, chapters on indexes, `EXPLAIN` and concurrency control

## Progress

- [ ] Week 1
- [ ] Week 2
- [ ] Week 3
- [ ] Week 4
- [ ] Week 5
- [ ] Week 6
- [ ] Week 7
- [ ] Week 8
- [ ] Week 9
- [ ] Week 10
- [ ] Week 11
- [ ] Week 12
