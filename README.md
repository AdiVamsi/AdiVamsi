<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=Adi%20Vamsi&fontSize=52&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=AI%20Systems%20%C2%B7%20LLM%20Pipelines%20%C2%B7%20Python%20Backend&descAlignY=55&descAlign=50&descColor=a0aec0" width="100%"/>

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=15&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=AI+that+does+real+work%2C+not+demos.;LLM+pipelines+%C2%B7+Agent+systems+%C2%B7+Python+backends;Building+systems+that+stay+up+under+real+load.;San+Antonio%2C+TX+%C2%B7+Open+to+relocate+anywhere+in+the+U.S." alt="Typing SVG" />

</div>

<br/>

AI engineer building **production LLM systems, agent platforms, and the Python backends that hold them up** — software designed to eliminate manual work, not to win demos.

Currently at DATARA (May 2025–present) shipping async Python services and LLM classification pipelines — **99.9% uptime, 35% reduction in manual data extraction** across core workflows. Side builds: a grounded RAG service for insurance claim adjudication, a portfolio of 5 applied AI apps, an LLM-powered CRM for Indian SMBs, and a self-improving agent research platform.

---

## What I Build

**AI Workflows & LLM Pipelines** — Production LLM API integration, prompt-engineered classification, RAG systems, and agentic orchestration. Built to eliminate manual work from core business processes, not to pass benchmarks.

**Agent Systems** — Self-improving platforms where agents run optimization loops autonomously: program → artifact → metric → commit. Multi-agent coordination with pluggable LLM providers.

**Async Backend Services** — Python and Java/Spring Boot services behind the AI layer. Clean API contracts, observable, debuggable under real load.

**Operator Products** — CRMs, lead engines, and real-time dashboards for operators running daily workflows. WhatsApp capture, AI scoring, live updates over WebSockets.

---

## Systems

<table>
<tr>
<td width="50%">
<a href="https://github.com/AdiVamsi/insurance-claim-rag">
<img src="images/card-insurance-rag.svg" width="100%" alt="Insurance Claims RAG"/>
</a>
</td>
<td width="50%">
<a href="https://github.com/AdiVamsi/ai-apps-portfolio">
<img src="images/card-ai-apps.svg" width="100%" alt="AI Apps Portfolio"/>
</a>
</td>
</tr>
<tr>
<td width="50%">
<a href="https://github.com/AdiVamsi/indian-sme-engine">
<img src="images/card-sme-engine.svg" width="100%" alt="Indian SME Engine"/>
</a>
</td>
<td width="50%">
<a href="https://github.com/AdiVamsi/agent-hub">
<img src="images/card-agent-hub.svg" width="100%" alt="Agent Hub"/>
</a>
</td>
</tr>
</table>

<details>
<summary><b>Insurance Claims RAG</b> — Grounded retrieval for claim adjudication &nbsp; <sub><code>latest</code></sub></summary>

&nbsp;

Every answer is backed by a verbatim policy clause and a JSON audit trail an adjuster can hand to compliance. When the corpus doesn't support an answer, the service **refuses instead of guessing**.

```
POST /ask → classify → retrieve → ground → verify → ClaimAnswer JSON
                │          │         │         │
                ▼ low conf ▼ low sim │         ▼ quote not in context
                └──────────────── refuse ──────┘
```

LangGraph state machine with **3 independent refusal gates** (classifier confidence, retrieval similarity, verifier quote-match). Ingest: PDFs → pypdf per-page → heading-aware split → MiniLM embeddings → ChromaDB filtered by `policy_type`. FastAPI, Python 3.11, ~2 minutes from clone to first response.

</details>

<details>
<summary><b>AI Apps Portfolio</b> — 5 applied AI patterns in one structured codebase</summary>

&nbsp;

Chat · Prompt Chaining · Content Summarization · Natural-Language-to-SQL · Multi-Document RAG — all built on a shared, **provider-agnostic** foundation that works with both OpenAI and local Ollama models. Not five random demos — one system with consistent architecture, shared utilities, clean UIs, and honest limitations.

</details>

<details>
<summary><b>Indian SME Engine</b> — LLM-powered multi-tenant CRM for Indian SMBs</summary>

&nbsp;

Captures leads from web forms and WhatsApp, auto-classifies and scores them via AI, surfaces prioritized follow-ups through a real-time operator dashboard. Node.js/Express + Prisma/PostgreSQL, JWT auth with tenant-isolated data layer, WebSocket live updates, AI scoring engine. **100+ commits, actively developed.**

</details>

<details>
<summary><b>Agent Hub</b> — Self-improving agent platform</summary>

&nbsp;

Each agent optimizes a real-world problem overnight via an automated loop: `program.md → artifact → scalar metric → git commit or reset`. Running **~12 experiments/hr**. Meta-agent coordination layer for hands-off overnight optimization with clean version history — pluggable into Claude, Codex, or any LLM provider.

</details>

---

## Proof of Work

Numbers from production, not a portfolio site.

```
┌─────────────────────────────────────────────────────────────────┐
│  DATARA · Python Developer · May 2025–present                   │
├─────────────────────────────────────────────────────────────────┤
│  5 production pipelines  │  99.9% uptime  │  35% less manual    │
│  async I/O: 10h → 8h    │  3 new sources │  150 hrs/mo saved   │
│  incidents: 48h → 12h   │  in <2 wks each │  post-deploy -15%  │
├─────────────────────────────────────────────────────────────────┤
│  XRG · Jr SWE (New Relic client) · Jun 2020–Dec 2022           │
├─────────────────────────────────────────────────────────────────┤
│  15+ microservices       │  85%+ coverage │  ~30% faster QA     │
│  millions daily queries  │  ~20% faster   │  ~40 hrs/sprint     │
│                          │  throughput    │  saved               │
└─────────────────────────────────────────────────────────────────┘
```

---

## Now Building

```
role:     Python Developer @ DATARA Pvt Ltd  ·  San Antonio, TX / Remote
focus:    LLM pipeline automation + async Python backend services
latest:   insurance-claim-rag — grounded RAG w/ refusal gates & audit trail
next:     ai-apps-portfolio — 5 applied AI apps, provider-agnostic
stack:    Python · FastAPI · LangChain · LangGraph · ChromaDB · PostgreSQL
```

---

## Stack

**Core** &nbsp;
![Python](https://img.shields.io/badge/Python-0d1117?style=flat-square&logo=python&logoColor=4584b6)
![Java](https://img.shields.io/badge/Java-0d1117?style=flat-square&logo=openjdk&logoColor=ed8b00)
![TypeScript](https://img.shields.io/badge/TypeScript-0d1117?style=flat-square&logo=typescript&logoColor=3178c6)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0d1117?style=flat-square&logo=postgresql&logoColor=4169e1)

**AI & Agents** &nbsp;
![LangChain](https://img.shields.io/badge/LangChain-0d1117?style=flat-square&logo=chainlink&logoColor=375bd2)
![LangGraph](https://img.shields.io/badge/LangGraph-0d1117?style=flat-square&logo=python&logoColor=58a6ff)
![OpenAI](https://img.shields.io/badge/OpenAI-0d1117?style=flat-square&logo=openai&logoColor=ffffff)
![ChromaDB](https://img.shields.io/badge/ChromaDB-0d1117?style=flat-square&logo=databricks&logoColor=ff6f00)

**Backend & Infra** &nbsp;
![FastAPI](https://img.shields.io/badge/FastAPI-0d1117?style=flat-square&logo=fastapi&logoColor=009688)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-0d1117?style=flat-square&logo=springboot&logoColor=6db33f)
![AWS](https://img.shields.io/badge/AWS-0d1117?style=flat-square&logo=amazonwebservices&logoColor=ff9900)
![Docker](https://img.shields.io/badge/Docker-0d1117?style=flat-square&logo=docker&logoColor=2496ed)

**Certified** &nbsp;
![AWS CCP](https://img.shields.io/badge/AWS%20Cloud%20Practitioner-0d1117?style=flat-square&logo=amazonwebservices&logoColor=ff9900)
![Oracle Java SE 17](https://img.shields.io/badge/Oracle%20Java%20SE%2017-0d1117?style=flat-square&logo=oracle&logoColor=f80000)

---

## Trace a Request

How a single query moves through [insurance-claim-rag](https://github.com/AdiVamsi/insurance-claim-rag). Expand each stage to see what happens — and *why* it's built that way.

<img src="images/trace-header.svg" width="100%" alt="Request trace through insurance-claim-rag pipeline"/>

```
curl -X POST /ask -d '{"query": "Does my auto policy cover flood damage?"}'
```

<details>
<summary><b>Stage 1 · classify</b> — What kind of claim is this?</summary>

&nbsp;

An LLM classifier reads the raw query and outputs a `policy_type` + confidence score. No retrieval yet — this is a cheap call that routes the rest of the pipeline.

```json
{
  "policy_type": "auto",
  "confidence": 0.95,
  "rationale": "Mentions auto coverage and a specific peril (flood)."
}
```

**Gate:** If confidence < 0.6, the service **refuses immediately** — no point retrieving documents against a misclassified query. The refusal reason is logged in `audit_trail.classify`.

**Why this matters:** Without classification, a homeowner's query could retrieve auto clauses and hallucinate a confident wrong answer. The gate costs ~200ms and prevents an entire class of errors downstream.

</details>

<details>
<summary><b>Stage 2 · retrieve</b> — Find the relevant policy clauses</summary>

&nbsp;

ChromaDB vector search over MiniLM embeddings, **filtered by `policy_type: "auto"`** from Stage 1. Returns top-k chunks with similarity scores.

```json
{
  "k": 5,
  "top_sim": 0.71,
  "best_chunk": "Section 3 · Comprehensive Coverage — pays for direct and accidental
    loss from perils other than collision, including fire, theft, vandalism,
    falling objects, hail, and impact with an animal. Flood damage is included
    only if specifically endorsed..."
}
```

**Gate:** If `top_sim` < 0.45, the corpus doesn't have relevant content — the service **refuses** rather than forcing the LLM to generate from weak context. Logged in `audit_trail.retrieve`.

**Why this matters:** Metadata-filtered search (not just vector similarity) prevents cross-policy contamination. A homeowner's flood clause and an auto flood endorsement say different things — the filter keeps them separate.

</details>

<details>
<summary><b>Stage 3 · ground</b> — Generate an answer anchored to the retrieved text</summary>

&nbsp;

The LLM receives the query + retrieved chunks and must produce a structured answer **that quotes directly from the context**. No synthesis from training data — if the clause doesn't say it, the answer can't say it.

```json
{
  "answer": "Flood damage is included only if specifically endorsed; absent
    that endorsement, flood loss is not covered under comprehensive.",
  "cited_index": 0,
  "cited_text": "Flood damage is included only if specifically endorsed...",
  "sufficient": true
}
```

**Design decision:** The prompt instructs the model to select a `cited_index` from the retrieved chunks and extract a verbatim quote. This makes the next stage (verify) possible — you can't verify a paraphrase, but you can verify a quote.

</details>

<details>
<summary><b>Stage 4 · verify</b> — Does the citation actually exist in the context?</summary>

&nbsp;

A deterministic check (no LLM) — does the quoted text from Stage 3 actually appear in the retrieved chunks from Stage 2? This catches hallucinated citations.

```json
{
  "verified": true,
  "quote_len": 89,
  "match_type": "substring"
}
```

**Gate:** If `verified: false`, the model cited text that doesn't exist in the context — a hallucinated citation. The service **refuses** and logs it. This is the gate that catches LLM confabulation.

**Why this matters:** Most RAG systems trust the model's citations. This one doesn't. A compliance officer can trace every answer back to a real page, section, and verbatim clause — or the system tells you it can't.

</details>

<details>
<summary><b>Stage 5 · respond</b> — Structured JSON, not chat</summary>

&nbsp;

All stages collapse into a single `ClaimAnswer` object. Every field is typed, every decision is auditable.

```json
{
  "query": "Does my auto policy cover flood damage?",
  "answer": "Flood damage is included only if specifically endorsed...",
  "decision": "answered",
  "confidence": "high",
  "citations": [{
    "text": "Flood damage is included only if specifically endorsed...",
    "source_file": "auto_personal_policy.pdf",
    "page_number": 1,
    "section_heading": "3. Comprehensive Coverage",
    "similarity": 0.71
  }],
  "audit_trail": {
    "classify": { "policy_type": "auto", "confidence": 0.95 },
    "retrieve": { "k": 5, "top_sim": 0.71 },
    "ground":   { "cited_index": 0, "sufficient": true },
    "verify":   { "verified": true, "quote_len": 89 }
  }
}
```

**The point:** An adjuster doesn't read chat. They need a decision, a cited clause, a page number, and an audit trail they can hand to compliance. That's what this returns — structured output designed for a downstream review queue, not a conversation.

</details>

&nbsp;

<sub>3 independent refusal gates. Every answer traceable to a verbatim clause. If the system can't prove it, it says so.<br/>— <a href="https://github.com/AdiVamsi/insurance-claim-rag"><i>View the full system</i></a></sub>

---

## Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=AdiVamsi&show_icons=true&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=e6edf3&icon_color=58a6ff&include_all_commits=true&count_private=true" height="165"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=AdiVamsi&layout=compact&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=e6edf3&langs_count=8" height="165"/>

<img src="https://github-readme-streak-stats.herokuapp.com?user=AdiVamsi&theme=transparent&hide_border=true&background=0D1117&ring=58A6FF&fire=58A6FF&currStreakLabel=58A6FF&sideLabels=E6EDF3&dates=8B949E&currStreakNum=E6EDF3&sideNums=E6EDF3" height="165"/>

</div>

---

## Find Me

[![Email](https://img.shields.io/badge/adivamsi1998%40gmail.com-0d1117?style=flat-square&logo=gmail&logoColor=ea4335)](mailto:adivamsi1998@gmail.com)
&nbsp;
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0d1117?style=flat-square&logo=linkedin&logoColor=0a66c2)](https://www.linkedin.com/in/adi-vamsi-sai-326667128/)
&nbsp;
[![Portfolio](https://img.shields.io/badge/Portfolio-0d1117?style=flat-square&logo=vercel&logoColor=ffffff)](https://portfolio-orpin-rho-13.vercel.app)
&nbsp;
[![Resume](https://img.shields.io/badge/Resume-0d1117?style=flat-square&logo=readdotcv&logoColor=ffffff)](https://portfolio-orpin-rho-13.vercel.app/resume.pdf)
&nbsp;
[![GitHub](https://img.shields.io/badge/%40AdiVamsi-0d1117?style=flat-square&logo=github&logoColor=ffffff)](https://github.com/AdiVamsi)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>
