# Architecture

A map of how this project fits together: the Expound entity and its two arms,
this repository's structure, and the website's information architecture. Diagrams
are written in [Mermaid](https://mermaid.js.org/) and render directly on GitHub.

---

## 1. Conceptual architecture — Expound

One entity, two arms, both grounded in the FLCA framework.

```mermaid
graph TD
    EXPOUND["Expound<br/>From AI Ambition to AI Reality"]

    EXPOUND --> COMM["Commercial arm<br/>(four service pillars)"]
    EXPOUND --> LAB["Engineering & open-source lab<br/>this repo · website 'Open Labs' section"]

    COMM --> BOOST["Boost — AI strategy consulting"]
    COMM --> BUILD["Build — AI agent development"]
    COMM --> GROW["Grow — incubation & acceleration"]
    COMM --> BACK["Back — venture investment"]

    LAB --> WF["Workflows<br/>verification-first playbooks"]
    LAB --> FM["Failure modes<br/>where LLMs are confidently wrong"]
    LAB --> AP["Audience personas"]
    LAB --> HH["Hallucination hedging patterns"]

    FLCA["FLCA framework<br/>Four-Layer Cognitive Architecture<br/>repo: EskilXu/FLCA"]

    COMM -. grounded in .-> FLCA
    LAB  -. grounded in .-> FLCA
```

---

## 2. Repository structure

`workflows/` is the core deliverable; it cites `failure_modes/` and targets the
people described in `audience_personas/`. `index.html` is the public website,
bound to `expoundlabs.io` via `CNAME`.

```mermaid
graph TD
    ROOT["Expound/ (repo root)"]

    ROOT --> SITE["index.html + CNAME<br/>→ expoundlabs.io"]
    ROOT --> DOCS["README.md · manifesto.md<br/>CONTRIBUTING.md · LICENSE"]
    ROOT --> WF["workflows/"]
    ROOT --> FM["failure_modes/"]
    ROOT --> AP["audience_personas/"]

    WF --> WF1["01_reading_long_documents/<br/>README · prompts · verification_checklist · examples"]
    WF --> WF2["02_legal_adjacent_memo/ — in development"]
    WF --> WF3["03_market_research/ — in development"]

    FM --> FM1["citation_fabrication.md"]
    FM --> FM2["numerical_precision.md"]
    FM --> FM3["time_sensitivity.md"]

    AP --> AP1["lawyer.md"]
    AP --> AP2["operator.md"]
    AP --> AP3["researcher.md"]

    WF -. each workflow cites .-> FM
    WF -. written for .-> AP
```

---

## 3. Website information architecture

Sections of `index.html`, top to bottom. The **Open Labs** section is the public
front door to this repository.

```mermaid
graph TD
    NAV["index.html / expoundlabs.io"]

    NAV --> S1["Hero — From AI Ambition to AI Reality"]
    NAV --> S2["The Problem — capability vs reliability gap"]
    NAV --> S3["Services — Boost / Build / Grow / Back"]
    NAV --> S4["FLCA — Theoretical Foundation"]
    NAV --> S5["Open Labs — open-source lab front door"]
    NAV --> S6["About the Founder"]
    NAV --> S7["AI Thesis Series"]
    NAV --> S8["Get Started — Contact"]
```

---

## Key relationships

- **One entity, two arms** — commercial services (four pillars) and the
  open-source lab (this repo); the website surfaces the latter as its
  **Open Labs** section.
- **Theory foundation** — both arms build on **FLCA**, which lives in its own
  repository, [`EskilXu/FLCA`](https://github.com/EskilXu/FLCA).
- **Repo = lab output** — `workflows/` (main deliverable), `failure_modes/`
  (cross-cutting knowledge), `audience_personas/` (who it's for), and
  `manifesto.md` (mission), all cross-referencing one another.
- **Website = unified public face** — `index.html` is hosted from this repo and
  pointed at expoundlabs.io via `CNAME`.
