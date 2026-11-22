# Nikita Mikaev · Staff Engineer

Tbilisi, Georgia (GMT+4)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-nmikaev-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nmikaev)
[![CV](https://img.shields.io/badge/CV-PDF-B31B1B?logo=adobeacrobatreader&logoColor=white)](Nikita_Mikaev_CV_Staff.pdf)

## Summary

Staff Engineer with 10+ years of backend development in Java and distributed systems architecture across banking, healthtech, music distribution, e-commerce, and streaming.

Currently leading a monolith decomposition program at a streaming platform. Previously built a global music distribution platform from scratch at Warner Music Group, led the core team behind the most critical paths of a 1M+ DAU marketplace, delivered a remote pre-shift medical clearance system for a railway operator, and engineered the brokerage platform core and SME credit pipeline at one of Russia's largest banks.

Hands-on engineer with a deep focus on architecture and code quality. Strong proponent of AI-assisted development backed by strict TDD and Clean Architecture workflows, actively helping peers and teams around me with AI adoption.

## Experience

### Staff Engineer · [Dcloud.tech](https://dcloud.tech/)
<sub>Aug 2025 – Present</sub>


- Leading the monolith decomposition program for a 7M MAU streaming platform, owning the target architecture and domain boundaries.
- Moved playback and catalog out of the monolith's shared database and release cycle, cutting playback API p95 latency from 900 to 350 ms and release lead time from 6 to 2 weeks.
- Designed and shipped an internal AI hiring platform for internal purposes (resume scoring, RAG-based candidate search, resume-to-vacancy matching, personalized assessments, AI interview avatar) that halved time-to-hire.

*Java, Spring Boot, Hibernate, Kafka, PostgreSQL, Redis, Debezium, OpenSearch, Keycloak, OpenTelemetry, Kubernetes*

### Engineering Manager · [Uzum Market](https://uzum.uz)
<sub>Mar 2024 – Aug 2025</sub>


The largest marketplace in Uzbekistan: 1M+ DAU, 100k+ orders daily.
- Led the turnaround of a 9-engineer cross-functional team owning the marketplace's highest-traffic customer journeys (Main Page, Promotions) after severe leadership turnover.
- Drove +$1.45M incremental GMV, +1.7% order conversion and +10.1% registration conversion. Delivered a social project with $10.5M GMV that laid the foundation for a $17M ARR banking initiative.
- Raised sprint commitment rate from 20–30% to a consistent 85–100% through capacity-based planning, a clearly defined SDLC and a dedicated tech-debt quota.
- Architected the extraction of promo code and bonus logic scattered across the monolith into a dedicated service as the single source of truth. Authored the RFC and defended the target design before the Architecture Committee.
- Eliminated critical Main Page crashes caused by GraphQL null propagation by returning partial data with errors and rendering each widget independently.

*Java, Spring Boot, Hibernate, Kafka, PostgreSQL, Debezium, GraphQL, Kubernetes, GrowthBook, Grafana, Jaeger*

### Team Lead · [Warner Music Group](https://www.wmg.com/)
<sub>Sep 2021 – Mar 2024</sub>


Global music distribution platform used by WMG, labels and studios, covering the full cycle from release creation to delivery to Spotify and Apple Music.
- Hired and led a distributed cross-functional team (backend, frontend, QA) with near-zero attrition over 2.5 years.
- Architected and launched the cloud-native platform on AWS from scratch, delivering the end-to-end system within a strict 8-month timeline.
- Introduced compression for audio spectrograms, cutting AWS storage costs by a third.
- Designed and rolled out a granular permission model with access control at the department, role, release participation, stage and action levels.
- Designed royalty and pricing mechanics supporting per-country pricing and individual contract terms.

*Java, Node.js, Spring Boot, AWS (Lambda, SQS, Aurora, Step Functions, S3, CloudFront, EC2, API Gateway, CDK), Okta*

### Team Lead · National Railways
<sub>Jan 2021 – Sep 2021</sub>


Remote pre-shift medical checks for train drivers and depot staff.
- Hired and led a team of 8 as tech lead and architect.
- Architected the platform end to end (services, data flows, integrations, media server) and took it to production in 4 months, then rolled it out to thousands of depot terminals nationwide.
- Designed a custom WebRTC signalling protocol on top of the media server, with session recording and STUN/TURN connectivity for unstable depot networks.
- Built a pod-pinning mechanism for WebSocket sessions on Redis Streams, keeping each session bound to its pod as the service scaled horizontally.

*Java, Kotlin, Spring Boot, Hibernate, WebRTC, Redis Streams, Kafka, PostgreSQL, Keycloak, Kubernetes, ELK*

### Team Lead · VTB Bank
<sub>Feb 2019 – Jan 2021</sub>


Led three products in succession, each with a 12-person cross-functional team I hired.
- Architected and launched the brokerage core orchestrating client operations across ledger, reporting, tax and depository at 800 TPS peak. Used Kafka with transactional outbox, and Debezium CDC to stream ledger changes into reporting.
- Built an SME loan underwriting system on Camunda, replacing legacy email-based routing: applications are assigned to underwriters by a workflow and competence management mechanics. Cut review time from 3–4 days to half a day.
- Built a Camunda-based CRM for managers serving wealthy clients, cutting handling time by 40%.

*Java, Spring Boot, Hibernate, GraphQL, Camunda, Kafka, Debezium, ActiveMQ, PostgreSQL, Kubernetes, ELK*

### Senior Software Engineer · VTB Bank
<sub>Jan 2018 – Feb 2019</sub>


- Built the multi-channel notification subsystem (push, email, SMS) for corporate lending on RabbitMQ, with transactional outbox and deduplication for effectively-once delivery.

*Java, Spring Boot, Hibernate, RabbitMQ, MongoDB, Kubernetes, ELK*

### Senior Software Engineer · [Avaya](https://www.avaya.com/en/)
<sub>Oct 2016 – Jan 2018</sub>


- Designed and built from scratch a contact-center loyalty scoring system that rates callers by their social media mentions, as de facto tech lead of a team of 8.

*Java, Spring, Hibernate, Kafka, PostgreSQL, MongoDB, Redis*

### Software Engineer · [Kaspersky Lab](https://www.kaspersky.com/)
<sub>Jan 2016 – Oct 2016</sub>


- Built backend for a corporate email security gateway that checks attachments by hash and quarantines unknown ones.

*Java, Hibernate, RabbitMQ, MySQL*

## Skills

- **Languages & frameworks:** Java 21, Kotlin, Python, Spring Boot 3, Hibernate, FastAPI, Flask
- **Architecture:** distributed systems, microservices, monolith decomposition, event-driven architecture, Clean Architecture, saga orchestration, transactional outbox, CDC (Debezium), idempotency, BFF
- **Patterns & Principles:** GoF, GRASP, SOLID, EIP, Resilient patterns (Circuit Breaker, Retry, Rate Limiting, Throttling)
- **APIs & protocols:** REST, GraphQL, OpenAPI (API-first), WebSockets, WebRTC
- **Workflow engines:** Camunda, AWS Step Functions
- **Databases & search:** PostgreSQL, MongoDB, Redis, OpenSearch
- **Messaging:** Kafka, RabbitMQ, ActiveMQ
- **Cloud & infra:** AWS (Lambda, Aurora, SQS, S3, CloudFront, API Gateway, EC2, CDK), Kubernetes, Docker, Helm, Istio
- **Observability:** OpenTelemetry, Prometheus, Grafana, Jaeger, ELK, SLO/SLI
- **Security:** Keycloak, OAuth2/OIDC, Okta, RBAC/ABAC, HashiCorp Vault
- **Testing & delivery:** TDD, mutation testing, Testcontainers, WireMock, feature flags (GrowthBook), user-level A/B rollouts
- **AI:** RAG, LangChain, ChromaDB, Claude Code (agentic workflows)

## Education

- Master of Software Engineering, Moscow State Technological University "Stankin", 2020–2022
- Bachelor of Computer Science, Moscow State Technological University "Stankin", 2016–2020

## Achievements

- Two-time National Mathematics Champion (2017, 2018)
- Java Programming Course Instructor, Moscow State Technological University "Stankin" (2020–2022)
