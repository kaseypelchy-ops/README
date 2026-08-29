# Kasey Alexander Pelchy

Marketing Manager working at the intersection of **Marketing Operations, Revenue Operations, AI, automation, data, and business systems**.

I translate business and operational problems into repeatable workflows, structured data, decision-support tools, and working software.

My work includes customer acquisition and lifecycle strategy, full-stack decision-support platforms, field-sales operations software, AI-powered quality and coaching systems, geospatial data pipelines, SEO/AEO and search-intelligence infrastructure, analytics, reporting, automation, and internal business applications.

Most of these projects started with a real operational problem â€” disconnected data, repetitive work, limited visibility, difficult reporting, inconsistent processes, or software that did not fit the actual workflow â€” and grew into purpose-built systems designed around how the work really happens.

I often work across the full lifecycle:

**business problem â†’ process â†’ data â†’ technology â†’ outcome â†’ improvement**

**[View my interactive portfolio â†’](https://kaseys-portfolio.vercel.app)**

---

## Areas I Work Across

Marketing Operations Â· Revenue Operations Â· Sales Operations Â· Marketing Technology Â· Business Process Improvement Â· Customer Lifecycle Strategy Â· Full-Stack Application Development Â· Data Engineering Â· Data Analytics Â· Business Intelligence Â· Decision-Support Systems Â· Process Automation Â· AI / LLM Systems Â· Database Design Â· Geospatial Data Â· SEO / AEO Â· Search Intelligence Â· Internal Tools Â· Reporting Â· Cross-System Integration

---

## Technology

**Languages**  
TypeScript Â· JavaScript Â· Python Â· PHP Â· SQL Â· PL/pgSQL Â· HTML Â· CSS

**Application & Data**  
React Â· Next.js Â· PostgreSQL Â· Supabase Â· DuckDB Â· WordPress

**Cloud & Integration**  
Vercel Â· Google Cloud Â· GitHub Actions Â· REST APIs Â· Cloud Tasks Â· JSON Â· JSONB Â· JSON-LD

**Marketing, Search & Analytics**  
Google Search Console Â· Google Analytics 4 Â· Bing Webmaster Tools Â· Mautic Â· ACF Â· Schema.org

**Data & Spatial**  
Shapely Â· PyProj Â· KML / KMZ Â· FCC Broadband Fabric Â· Geospatial Processing

---

## Certifications

**HubSpot Revenue Operations Certified** Â· **HubSpot Inbound Certified**

---

# Featured Projects

## Market Recovery Intelligence Platform

I built a full-stack market-intelligence and decision-support platform for identifying declining markets, investigating the underlying causes, prioritizing recovery opportunities, and measuring intervention outcomes.

The system combines acquisition activity, churn behavior, subscriber history, market identity, lifecycle state, and recovery-project data into a canonical analytical model.

Operational evidence is normalized before analytics are calculated. Multi-horizon trends and health signals feed a coverage-aware scoring model, while a separate policy layer determines whether a market is actually eligible for action.

Eligible candidates are then ranked deterministically for investigation.

```mermaid
flowchart TD
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

**Selected engineering work:** canonical data modeling Â· multi-horizon trend analysis Â· coverage-aware scoring Â· data-completeness modeling Â· deterministic ranking Â· transactional project creation Â· immutable measurement baselines Â· analytical read-path optimization Â· shared TypeScript domain modules Â· database indexing Â· regression validation

**Stack:** Next.js Â· React Â· TypeScript Â· PostgreSQL Â· Supabase Â· SQL Â· Data Engineering Â· Analytics

**[View the technical showcase â†’](https://github.com/kaseypelchy-ops/market-recovery-platform-showcase)**  
**[Open the live interactive demo â†’](https://kaseypelchy-ops.github.io/market-recovery-platform-showcase/)**

---

## Field Sales Operations Platform

I built a field-sales operations platform that connects serviceable-address data, territory management, door-to-door canvassing, customer dispositions, pricing, installation scheduling, sale submission, post-sale review, invoicing, and management reporting.

Field representatives get an address-centered mobile workflow, while operations and leadership receive centralized visibility into sales activity, installation capacity, territory performance, representative activity, lifecycle outcomes, and operational trends.

The platform is designed for real field conditions, including unreliable connectivity, shared installation capacity, realtime updates, transactional sale workflows, and preservation of unsynced work.

**Selected engineering work:** transactional sales workflows Â· PWA/offline synchronization Â· realtime reconciliation Â· installation-capacity management Â· pricing snapshots Â· duplicate-safe customer notifications Â· lifecycle tracking Â· PostgreSQL functions Â· role-based workflows Â· data-quality controls Â· reporting Â· cross-system integration

**Stack:** JavaScript Â· HTML / CSS Â· PostgreSQL Â· PL/pgSQL Â· Supabase Â· Vercel Â· Leaflet

**[View the FieldOS showcase â†’](https://github.com/kaseypelchy-ops/fieldos-project-showcase)**

---

## AI Call Quality & Coaching Platform

I built an AI-powered quality assurance, coaching, and management analytics platform for customer-service calls.

Completed call recordings move through an asynchronous processing pipeline that validates eligibility, prevents duplicate analysis, performs structured AI evaluation, applies deterministic scoring, persists the result, and routes the output into coaching and management workflows.

The architecture separates ingestion, queueing, AI analysis, application scoring, persistence, notification delivery, coaching, and reporting so failures in one stage do not silently compromise the rest of the process.

**Selected engineering work:** queue-based processing Â· idempotent analysis Â· structured LLM output Â· deterministic scoring Â· asynchronous workers Â· retry handling Â· processing locks Â· automated notifications Â· coaching workflows Â· effectiveness measurement Â· operational-health monitoring Â· management analytics

**Stack:** Python Â· TypeScript Â· React Â· Next.js Â· PostgreSQL Â· PL/pgSQL Â· Supabase Â· Google Cloud Â· Cloud Tasks Â· Vercel Â· AI / LLMs

**[View the AI Call Quality showcase â†’](https://github.com/kaseypelchy-ops/ai-call-quality-platform-showcase)**

---

## SEO, AEO & Search Intelligence Platform

I built and continue to develop a production search-operations platform connecting structured website content, technical site health, organic-search performance, optimization workflows, and AI-visibility measurement.

The project began as a database-driven SEO and Answer Engine Optimization system. Pages, geographic relationships, services, promotions, keywords, FAQs, content sections, internal links, redirects, metadata, and publishing state are modeled in PostgreSQL and Supabase. Reusable WordPress templates retrieve page-level JSON bundles and dynamically render localized content, metadata, and structured data.

That foundation helped expand localized website coverage from approximately 25 manually maintained pages to more than 435 dynamic market and service-area pages.

The system has since expanded into a protected Next.js application combining managed page data, live rendered-site evidence, Google Search Console performance, GA4 AI referral data, Bing AI citation evidence, automated monitoring, prioritization models, internal-link workflows, and optimization experiments.

```mermaid
flowchart TD
    A[Structured Content] --> B[Publish + Render]
    B --> C[Collect Evidence]
    C --> D[Diagnose + Prioritize]
    D --> E[Implement + Verify]
    E --> F[Measure Outcomes]
    F --> C
```

The platform deliberately preserves source meaning: Search Console performance, rendered-site health, identifiable AI referrals, and AI citations can be compared operationally without being blended into fabricated metrics. It also distinguishes **not measured** from **measured zero** and retains import lineage for auditable results.

**Selected engineering work:** relational content modeling Â· reusable WordPress publishing Â· Search Console integration Â· intent and page-ownership intelligence Â· opportunity prioritization Â· content-gap and cannibalization analysis Â· rendered-site health monitoring Â· internal-link execution and verification Â· optimization experiments Â· GA4 AI-referral measurement Â· Bing AI citation intelligence Â· pipeline operations Â· explainable scoring and guardrails

**Stack:** Next.js Â· React Â· TypeScript Â· PostgreSQL Â· Supabase Â· WordPress Â· PHP Â· Google Search Console Â· Google Analytics 4 Â· Bing Webmaster Tools Â· REST APIs Â· JSONB Â· JSON-LD Â· Vercel

**[View the SEO, AEO & Search Intelligence showcase â†’](https://github.com/kaseypelchy-ops/seo-aeo-content-platform-showcase)**

---

## Fiber Service Area Mapping Pipeline

I built a geospatial data pipeline that converts KML/KMZ service-area boundaries into structured broadband-location datasets.

The pipeline parses and repairs source geometry, calculates a service-area bounding box, uses DuckDB to reduce a large FCC Broadband Fabric dataset to a candidate set, and then performs exact point-in-polygon matching with Shapely.

Matched locations are deduplicated, normalized, enriched with selected geographic attributes, and exported as structured JSON and CSV for downstream systems.

The cloud workflow also includes generation-aware duplicate protection, processing locks, stale-lock recovery, lineage tracking, and optional cost-controlled geocoding fallback.

**Selected engineering work:** geometry parsing and repair Â· coordinate transformations Â· bounding-box filtering Â· DuckDB query optimization Â· point-in-polygon analysis Â· streaming record processing Â· normalization Â· deduplication Â· processing locks Â· stale-lock recovery Â· lineage tracking Â· cloud automation

**Stack:** Python Â· DuckDB Â· SQL Â· Shapely Â· PyProj Â· Google Cloud Â· KML / KMZ Â· FCC Broadband Fabric

**[View the Fiber Mapping showcase â†’](https://github.com/kaseypelchy-ops/fiber-service-area-mapping-showcase)**

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

I am comfortable moving between the business and technical sides of a problem â€” from defining the objective and workflow to modeling the data, designing the architecture, building the system, validating it, and using the resulting information to support operational decisions.

My background in marketing and operations shapes how I approach software, data, and process design. I understand the customer-acquisition and lifecycle side of the work as well as the systems required to support it.

I tend to start with four questions:

**What problem needs to be solved?**  
**Who needs the answer?**  
**What evidence is required to make the decision?**  
**How can the process become repeatable?**

Then I determine what should be built to make that happen.

My work sits at the intersection of **Marketing Operations, Revenue Operations, marketing technology, business systems, software engineering, data, analytics, automation, and AI**.

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

**[Interactive Portfolio â†’](https://kaseys-portfolio.vercel.app)**  
**[GitHub â†’](https://github.com/kaseypelchy-ops)**  
**[LinkedIn â†’](https://www.linkedin.com/in/kaseypelchy19/)**
