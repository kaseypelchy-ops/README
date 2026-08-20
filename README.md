# Kasey Alexander Pelchy

Marketing Manager building systems at the intersection of **marketing technology, software engineering, data, automation, AI, and operations**.

I build practical systems when the process or tool I need does not already exist.

My work has included full-stack decision-support platforms, field-sales operations software, AI-powered quality and coaching systems, geospatial data pipelines, database-driven SEO/AEO infrastructure, analytics, reporting, automation, and internal business applications.

Most of these projects started with a real operational problem — disconnected data, repetitive work, limited visibility, difficult reporting, inconsistent processes, or software that did not fit the actual workflow — and grew into purpose-built systems designed around how the work really happens.

I typically work across the full lifecycle:

**business problem → workflow → data model → architecture → implementation → validation → operational use**

---

## Areas I Work Across

Marketing Strategy & Operations · Marketing Technology · Full-Stack Application Development · Data Engineering · Data Analytics · Decision-Support Systems · Process Automation · AI / LLM Systems · Database Design · Geospatial Data · SEO / AEO · Internal Tools · Workflow Design · Reporting · Cross-System Integration

---

## Technology

**Languages**  
TypeScript · JavaScript · Python · PHP · SQL · PL/pgSQL · HTML · CSS

**Application & Data**  
React · Next.js · PostgreSQL · Supabase · DuckDB · WordPress

**Cloud & Integration**  
Vercel · Google Cloud · REST APIs · Cloud Tasks · JSON · JSONB · JSON-LD

**Data & Spatial**  
Shapely · PyProj · KML / KMZ · FCC Broadband Fabric · Geospatial Processing

---

# Featured Projects

## Market Recovery Intelligence Platform

I built a full-stack market-intelligence and decision-support platform for identifying declining markets, investigating the underlying causes, prioritizing recovery opportunities, and measuring intervention outcomes.

The system combines acquisition activity, churn behavior, subscriber history, market identity, lifecycle state, and recovery-project data into a canonical analytical model.

Operational evidence is normalized before analytics are calculated. Multi-horizon trends and health signals feed a coverage-aware scoring model, while a separate policy layer determines whether a market is actually eligible for action.

Eligible candidates are then ranked deterministically for investigation.

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

**Selected engineering work:** canonical data modeling · multi-horizon trend analysis · coverage-aware scoring · data-completeness modeling · deterministic ranking · transactional project creation · immutable measurement baselines · analytical read-path optimization · shared TypeScript domain modules · database indexing · regression validation

**Stack:** Next.js · React · TypeScript · PostgreSQL · Supabase · SQL · Data Engineering · Analytics

**[View the technical showcase →](https://github.com/kaseypelchy-ops/market-recovery-platform-showcase)**  
**[Open the live interactive demo →](https://kaseypelchy-ops.github.io/market-recovery-platform-showcase/)**

---

## Field Sales Operations Platform

I built a field-sales operations platform that connects serviceable-address data, territory management, door-to-door canvassing, customer dispositions, pricing, installation scheduling, sale submission, post-sale review, invoicing, and management reporting.

Field representatives get an address-centered mobile workflow, while operations and leadership receive centralized visibility into sales activity, installation capacity, territory performance, representative activity, lifecycle outcomes, and operational trends.

The platform is designed for real field conditions, including unreliable connectivity, shared installation capacity, realtime updates, transactional sale workflows, and preservation of unsynced work.

**Selected engineering work:** transactional sales workflows · PWA/offline synchronization · realtime reconciliation · installation-capacity management · pricing snapshots · duplicate-safe customer notifications · lifecycle tracking · PostgreSQL functions · role-based workflows · data-quality controls · reporting · cross-system integration

**Stack:** JavaScript · HTML / CSS · PostgreSQL · PL/pgSQL · Supabase · Vercel · Leaflet

**[View the FieldOS showcase →](https://github.com/kaseypelchy-ops/fieldos-project-showcase)**

---

## AI Call Quality & Coaching Platform

I built an AI-powered quality assurance, coaching, and management analytics platform for customer-service calls.

Completed call recordings move through an asynchronous processing pipeline that validates eligibility, prevents duplicate analysis, performs structured AI evaluation, applies deterministic scoring, persists the result, and routes the output into coaching and management workflows.

The architecture separates ingestion, queueing, AI analysis, application scoring, persistence, notification delivery, coaching, and reporting so failures in one stage do not silently compromise the rest of the process.

**Selected engineering work:** queue-based processing · idempotent analysis · structured LLM output · deterministic scoring · asynchronous workers · retry handling · processing locks · automated notifications · coaching workflows · effectiveness measurement · operational-health monitoring · management analytics

**Stack:** Python · TypeScript · React · Next.js · PostgreSQL · PL/pgSQL · Supabase · Google Cloud · Cloud Tasks · Vercel · AI / LLMs

**[View the AI Call Quality showcase →](https://github.com/kaseypelchy-ops/ai-call-quality-platform-showcase)**

---

## SEO & AEO Content Platform

I built a database-driven SEO and Answer Engine Optimization platform for managing hierarchical, localized website content through PostgreSQL, Supabase, and reusable WordPress templates.

Instead of maintaining each localized page as an independent collection of WordPress fields, the platform models pages, geographic hierarchy, services, promotions, keywords, FAQs, content sections, internal links, redirects, metadata, and publishing state as structured relational data.

PostgreSQL and PL/pgSQL assemble the related records into page-level JSON documents that WordPress can retrieve and render through reusable templates.

**Selected engineering work:** relational content modeling · hierarchical geography · JSONB document assembly · PL/pgSQL content generation · route resolution · dynamic metadata · structured-data generation · reusable templates · REST-based publishing · SEO/AEO architecture

**Stack:** PHP · WordPress · PostgreSQL · PL/pgSQL · Supabase · REST APIs · JSONB · JSON-LD

**[View the SEO & AEO Platform showcase →](https://github.com/kaseypelchy-ops/seo-aeo-content-platform-showcase)**

---

## Fiber Service Area Mapping Pipeline

I built a geospatial data pipeline that converts KML/KMZ service-area boundaries into structured broadband-location datasets.

The pipeline parses and repairs source geometry, calculates a service-area bounding box, uses DuckDB to reduce a large FCC Broadband Fabric dataset to a candidate set, and then performs exact point-in-polygon matching with Shapely.

Matched locations are deduplicated, normalized, enriched with selected geographic attributes, and exported as structured JSON and CSV for downstream systems.

The cloud workflow also includes generation-aware duplicate protection, processing locks, stale-lock recovery, lineage tracking, and optional cost-controlled geocoding fallback.

**Selected engineering work:** geometry parsing and repair · coordinate transformations · bounding-box filtering · DuckDB query optimization · point-in-polygon analysis · streaming record processing · normalization · deduplication · processing locks · stale-lock recovery · lineage tracking · cloud automation

**Stack:** Python · DuckDB · SQL · Shapely · PyProj · Google Cloud · KML / KMZ · FCC Broadband Fabric

**[View the Fiber Mapping showcase →](https://github.com/kaseypelchy-ops/fiber-service-area-mapping-showcase)**

---

# How I Build

I start with the process rather than the technology.

I look for places where:

- work is repetitive
- information is disconnected
- important decisions depend on manual analysis
- reporting is difficult
- multiple systems need to communicate
- existing software does not match the real workflow
- a process works at small scale but becomes difficult to manage as it grows

From there, my usual approach is:

1. **Map the workflow and decision points**
2. **Identify the entities, state, and business rules**
3. **Design the data model**
4. **Separate source evidence from analytical and operational logic**
5. **Choose the smallest architecture that can solve the problem reliably**
6. **Build for retries, failure, changing data, and changing requirements**
7. **Validate the system against the real workflow**
8. **Turn the output into something useful for the person making the decision**

The technology is a means to solve the business problem, not the starting point.

---

# Engineering Principles

### Model the process before the interface

The workflow, data relationships, state transitions, and rules should be understood before the UI dictates the architecture.

### Preserve clear sources of truth

When multiple screens or services depend on the same logic, I prefer shared domain rules and canonical data sources over duplicated implementations.

### Separate evidence from decisions

Raw data, analytical interpretation, and operational policy are different concerns. Keeping them separate makes systems easier to explain, test, and change.

### Treat missing data explicitly

Missing information should remain missing rather than silently becoming a healthy value, successful result, or false certainty.

### Design for failure and retries

Imports can be repeated. Workers fail. Connections drop. Users retry actions. Systems should expect those conditions rather than assume perfect execution.

### Preserve history

Changing today's configuration should not silently rewrite what happened yesterday. Historical decisions, pricing, measurements, and baselines should remain explainable.

### Build for the person making the decision

A technically correct system still fails if the person using it cannot understand the output or determine what to do next.

---

# What I Bring

I am comfortable moving between the business and technical sides of a problem — from defining the objective and workflow to modeling the data, designing the architecture, building the system, validating it, and using the resulting information to support operational decisions.

My background in marketing and operations shapes how I approach software.

I tend to start with four questions:

**What problem needs to be solved?**  
**Who needs the answer?**  
**What evidence is required to make the decision?**  
**How can the process become repeatable?**

Then I determine what should be built to make that happen.

My work sits at the intersection of **marketing technology, software engineering, data engineering, analytics, automation, AI, and operations**.

---

## About the Public Showcases

The repositories linked above are sanitized portfolio representations of privately maintained production systems and engineering work.

Production source code, credentials, customer or employee information, proprietary company data, internal infrastructure, confidential pricing, private operational metrics, and company-specific business rules are intentionally excluded.

The public repositories use combinations of:

- synthetic data
- generalized code samples
- neutral schema names
- technical documentation
- architecture diagrams
- representative SQL and TypeScript
- sanitized screenshots
- interactive reconstructions

The goal is to demonstrate the engineering approach without exposing private systems or data.

---

## Connect

**[LinkedIn →](https://www.linkedin.com/in/kaseypelchy19/)**
