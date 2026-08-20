# Kasey Alexander Pelchy

Marketing Manager building systems at the intersection of **marketing, operations, data, automation, AI, and software engineering**.

I build practical tools when the process I need does not already exist.

My work has included field-sales operations platforms, market-intelligence and recovery systems, AI-powered quality and coaching platforms, geospatial data pipelines, SEO/AEO infrastructure, analytics, reporting, automation, and internal business applications.

Most of these projects started with an operational problem — disconnected data, manual work, limited visibility, inconsistent processes, or systems that were difficult to scale — and grew into purpose-built platforms designed around the actual workflow.

I typically work across the full lifecycle: **understanding the business problem, modeling the process and data, building the system, validating it, and turning the output into something people can use to make better decisions.**

---

## Areas I Work Across

Marketing Strategy & Operations · Marketing Technology · Full-Stack Application Development · Data Analytics · Data Engineering · Process Automation · AI / LLM Systems · Database Design · Decision-Support Systems · Geospatial Data · SEO / AEO · Internal Tools · Workflow Design · Reporting · Cross-System Integration

---

## Technology

TypeScript · JavaScript · Python · PHP · SQL · PostgreSQL · PL/pgSQL · React · Next.js · DuckDB · Supabase · Vercel · Google Cloud · WordPress · REST APIs · HTML / CSS · JSONB · JSON-LD

---

# Featured Projects

## Field Sales Operations Platform

I built a field-sales operations platform that connects territory management, address-level canvassing, sales submission, installation scheduling, invoicing, reporting, and management oversight.

The system gives field representatives a mobile workflow while operations and leadership receive centralized visibility into sales activity, installation capacity, territory performance, representative activity, customer lifecycle events, and operational trends.

The platform also connects field activity to downstream data systems so submitted sales can be followed beyond the initial transaction and measured against installation, cancellation, disconnect, and other lifecycle outcomes.

**Selected engineering work:** transactional sales workflows, offline synchronization, real-time schedule updates, duplicate-safe customer notifications, lifecycle tracking, PostgreSQL functions, role-based workflows, data-quality controls, reporting, and cross-system integration.

**Stack:** TypeScript · JavaScript · PostgreSQL · PL/pgSQL · Supabase · Vercel

**[View the FieldOS showcase →](https://github.com/kaseypelchy-ops/fieldos-project-showcase)**

---

## Market Recovery Intelligence Platform

I built a market-intelligence and decision-support platform for identifying declining markets, investigating the underlying causes, prioritizing recovery opportunities, and measuring the results of intervention.

The system combines acquisition activity, churn behavior, subscriber history, market identity, lifecycle state, and recovery-project data into a canonical analytical model.

Rather than treating a score as the final decision, the platform separates **evidence, identity, analytics, severity, eligibility, ranking, and measurement** into distinct layers.

Operational data is normalized and mapped to canonical market identities before analytical metrics are calculated. Multi-horizon trends and health signals feed a coverage-aware scoring model that accounts for incomplete evidence without treating missing data as healthy.

A separate policy layer determines whether a market is actionable, after which eligible candidates are ranked deterministically for investigation.

Recovery projects preserve immutable measurement baselines so performance can be compared over time without rewriting the historical starting point.

```mermaid
flowchart LR
    A[Operational Data] --> B[Validation + Normalization]
    B --> C[Canonical Market Identity]
    C --> D[Derived Metrics]
    D --> E[Health Signals]
    E --> F[Recovery Score]
    F --> G[Eligibility Policy]
    G --> H[Deterministic Ranking]
    H --> I[Market Investigation]
    I --> J[Recovery Project]
    J --> K[Outcome Measurement]
```

**Selected engineering work:** canonical data modeling, multi-horizon trend analysis, coverage-aware weighted scoring, data-completeness modeling, deterministic ranking, transactional project creation, immutable baseline snapshots, analytical read-path optimization, shared TypeScript domain modules, database indexing, and regression validation.

**Stack:** Next.js · React · TypeScript · PostgreSQL · Supabase · SQL · Data Engineering · Analytics

**[View the Market Recovery Intelligence showcase →](https://github.com/kaseypelchy-ops/market-recovery-platform-showcase)**

---

## AI Call Quality & Coaching Platform

I built an AI-powered quality assurance and coaching platform for customer-service calls.

Completed call recordings move through a queue-based processing pipeline that validates eligibility, prevents duplicate analysis, performs structured AI evaluation, applies deterministic scoring, stores the results, and routes them into coaching and management workflows.

The platform supports one-on-one coaching, automated notifications, follow-up tracking, coaching-effectiveness measurement, processing-health monitoring, management analytics, and real-time dashboard updates.

The architecture separates ingestion, analysis, scoring, persistence, notification, and coaching workflows so failures in one stage do not silently compromise the rest of the process.

**Selected engineering work:** queue-based processing, idempotent analysis, deterministic scoring, AI evaluation pipelines, asynchronous workers, error handling, processing-health monitoring, coaching workflows, automated notifications, and management analytics.

**Stack:** Python · TypeScript · PostgreSQL · PL/pgSQL · Supabase · Google Cloud · Vercel · AI / LLMs · Cloud Tasks

**[View the AI Call Quality showcase →](https://github.com/kaseypelchy-ops/ai-call-quality-platform-showcase)**

---

## SEO & AEO Content Platform

I built a database-driven SEO and Answer Engine Optimization platform for managing hierarchical, localized website content through PostgreSQL, Supabase, and reusable WordPress templates.

Instead of managing every localized page independently, the platform models pages, geographic hierarchy, keywords, FAQs, content sections, internal links, services, markets, promotions, and redirects as structured data.

PL/pgSQL functions generate repeatable local SEO/AEO defaults, while PostgreSQL JSONB aggregation assembles related records into page-level documents that can be consumed by WordPress.

WordPress resolves the requested route, retrieves the published page bundle through Supabase REST, applies safe fallback behavior, and renders localized content, metadata, canonical and robots directives, Open Graph data, and JSON-LD.

**Selected engineering work:** relational content modeling, hierarchical geography, JSONB document assembly, dynamic metadata, structured data generation, route resolution, reusable templates, database-generated content defaults, and REST-based publishing.

**Stack:** PHP · WordPress · PostgreSQL · PL/pgSQL · Supabase · REST APIs · JSONB · JSON-LD · SEO / AEO

**[View the SEO & AEO Platform showcase →](https://github.com/kaseypelchy-ops/seo-aeo-content-platform-showcase)**

---

## Fiber Service Area Mapping Pipeline

I built a geospatial data pipeline that converts KML/KMZ service-area boundaries into structured broadband-location datasets.

The pipeline parses and repairs source geometry, calculates a service-area bounding box, queries FCC Broadband Fabric records stored in DuckDB to reduce the candidate universe, and then performs exact point-in-polygon matching with Shapely.

Matched locations are deduplicated, normalized, enriched with selected Census and Fabric attributes, and exported as structured JSON and CSV.

The cloud workflow also includes generation-aware duplicate protection, processing locks, stale-lock recovery, data-lineage tracking, and an optional cost-controlled geocoding fallback.

```mermaid
flowchart LR
    A[KML / KMZ] --> B[Geometry Parsing]
    B --> C[Bounding Box]
    C --> D[DuckDB Candidate Query]
    D --> E[Point-in-Polygon]
    E --> F[Normalize + Deduplicate]
    F --> G[Enrich Attributes]
    G --> H[JSON / CSV Output]
```

**Selected engineering work:** geometry repair, spatial filtering, point-in-polygon analysis, DuckDB query optimization, data normalization, deduplication, processing locks, stale-lock recovery, lineage tracking, and cloud processing.

**Stack:** Python · DuckDB · SQL · Shapely · PyProj · Google Cloud · KML / KMZ · FCC Broadband Fabric

**[View the Fiber Mapping showcase →](https://github.com/kaseypelchy-ops/fiber-service-area-mapping-showcase)**

---

# How I Approach Problems

I usually start with the process rather than the technology.

I look for places where:

- work is repetitive
- information is disconnected
- important decisions depend on manual analysis
- reporting is difficult
- multiple systems need to communicate
- existing software does not match the real workflow
- a process works at small scale but becomes difficult to manage as it grows

From there, I map the workflow, identify the entities and rules involved, define the data model, and determine the smallest architecture that can solve the problem reliably.

That might become a full application.

It might also become a database workflow, API integration, automation, analytical model, reporting layer, geospatial pipeline, or a better way to connect systems that already exist.

The technology is a means to solve the business problem, not the starting point.

---

# Engineering Principles

A few ideas consistently shape the systems I build:

### Model the process before building the interface

The workflow, data relationships, state transitions, and business rules should be understood before UI decisions dictate the architecture.

### Preserve one source of truth

When multiple applications need the same business logic, I try to centralize that logic rather than allowing each screen or service to develop its own interpretation.

### Separate evidence from decisions

Raw data, analytical conclusions, and operational policy are different things. Keeping those layers separate makes systems easier to explain, test, and change.

### Design for failure and retries

Imports can be repeated. Workers can fail. Networks disconnect. Users double-click buttons. Systems should expect those conditions instead of assuming perfect execution.

### Make the output useful to the person making the decision

A technically correct system still fails if the person using it cannot understand what happened or what they should do next.

---

# What I Bring

I am comfortable moving between the business and technical sides of a problem — from defining the objective and workflow to designing the data model, building the system, testing it, and using the resulting information to support operational decisions.

My background in marketing and operations means I tend to approach software differently than someone starting only from the engineering side.

I care about:

**What problem are we solving?**

**Who needs the answer?**

**What information do they need to make the decision?**

**Where does that information come from?**

**How do we make the process repeatable?**

And then:

**What should we build to make that happen?**

My work increasingly sits at the intersection of **marketing, software engineering, data, automation, AI, and operations**.

---

## About the Public Showcases

The repositories linked above are sanitized portfolio representations of privately maintained production systems and engineering work.

Production source code, credentials, customer or employee information, proprietary company data, internal infrastructure, confidential pricing, private operational metrics, and company-specific business rules are intentionally excluded.

The public repositories use synthetic data, generalized code samples, neutral schema names, technical documentation, architecture diagrams, and interactive reconstructions to demonstrate the engineering approach without exposing private systems.

---

## Connect

[LinkedIn](https://www.linkedin.com/in/kaseypelchy19/)
