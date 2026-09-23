<h1 align="center">Rajprakash Sahoo</h1>
<p align="center"><b>AI engineer ~ I build LLM systems that prove their work. Prefers primitives >>> frameworks</b></p>
<p align="center">
  <img src="https://img.shields.io/badge/open_to-AI_%2F_LLM_Engineer_roles-2ea44f?style=flat-square" alt="Open to AI Engineer roles">
  <a href="https://drive.google.com/file/d/1yTFHRxneAWEVLSZs6O9z0b-zQH_AYL24/view?usp=drivesdk">
    <img src="https://img.shields.io/badge/resume-Raj_AI_Engineer_Resume-important?style=flat-square&logo=readme&logoColor=white" alt="Raj_AI_Engineer_Resume.pdf"/></a>
</p>
<p align="center">
  <a href="https://www.linkedin.com/in/rajprakash-sahoo/"><img src="https://img.shields.io/badge/LinkedIn-Rajprakash_Sahoo-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://twitter.com/RajprakashSahoo"><img src="https://img.shields.io/badge/@RajprakashSahoo-black?style=flat-square&logo=X&logoColor=white&color=black" alt="X(twitter)"></a>
  <a href="mailto:rajprakash1999@gmail.com"><img src="https://img.shields.io/badge/email-rajprakash1999@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://byraj.dev"><img src="https://img.shields.io/badge/byraj.dev-111111?style=flat-square&logo=vercel&logoColor=white" alt="byraj.dev"></a>
</p>

> 🟢 **status** — 2 AI systems shipped · 🚧 building a review-gated PR risk agent · writing at [byraj.dev](https://byraj.dev) · India, remote-friendly

## 🟢 Shipped

### [Contract Change-Impact Intelligence](https://github.com/rajprakash00/contract-change-intel) · [try it live](https://change-report.byraj.dev)

Upload an agreement and its amendments; get obligations extracted (owners, deadlines, penalties), an explained diff, and every change mapped to the clauses it touches. Each statement cites its source text, low-confidence items queue for human review, and every LLM call's cost is persisted per tenant.

<a href="https://github.com/rajprakash00/contract-change-intel/actions/workflows/ci.yml"><img src="https://github.com/rajprakash00/contract-change-intel/actions/workflows/ci.yml/badge.svg" alt="CI"></a>
<a href="https://github.com/rajprakash00/contract-change-intel/actions/workflows/deploy.yml"><img src="https://github.com/rajprakash00/contract-change-intel/actions/workflows/deploy.yml/badge.svg" alt="Deploy"></a>

`1.0 citation validity` · `0.90 extraction precision` · `0.96 recall@10`
`FastAPI` `pgvector + Postgres FTS (RRF)` `Postgres job queue (SKIP LOCKED)` `AWS ECS/Fargate` `Terraform` `Next.js`

### [shotgrep](https://github.com/rajprakash00/shotgrep) · [try it live](https://shotgrep-demo.vercel.app)

Search video like it's text: ask for a moment in plain language, get the exact frame back with jump-to-timestamp links. Stage-cached ingest (FFmpeg → shot detection → faster-whisper ASR → SigLIP embeddings), fused visual + transcript retrieval over LanceDB, served as REST and MCP tools for agents.

`Recall@5 0.688 vs 0.578 baseline` · `MRR 0.495` · `p50 189 ms / p95 234 ms`
`Python` `FFmpeg` `faster-whisper` `SigLIP + bge-small ONNX int8` `LanceDB` `FastAPI` `MCP` `Fly.io`

### [rn-otp-timer](https://github.com/rajprakash00/rn-otp-timer)

Standalone OTP timer for React Native.

<a href="https://www.npmjs.com/package/rn-otp-timer"><img src="https://img.shields.io/npm/dt/rn-otp-timer?style=flat-square&label=downloads&color=CB3837" alt="npm downloads"></a>

## 🧠 How I build

- **No citation, no claim.** LLM output must trace to source text; invalid items get one repair pass, then drop.
- **Evals before vibes.** Precision/recall on frozen sets; CI fails when quality regresses.
- **Budgets are product features.** Per-run caps, per-tenant limits, cost persisted per call.
- **Humans hold the write.** Agents draft; people approve.

## 📚 Currently exploring

- **Agent harnesses** — tool loops, checkpointing, interrupt/resume when the model misbehaves.
- **Multi-agent systems** — where committees beat one loop, and where they just multiply the bill.
- **Harder evals** — frozen query splits, Recall@5 / MRR, regression gates instead of vibes.
- **Local-first agent spend** — metering and capping coding agents across vendors with a SQLite ledger and hooks.

## 🧰 Stack

**AI/LLM** — RAG (pgvector + FTS, RRF) · multimodal retrieval (SigLIP + bge-small, ONNX int8) · evals · structured outputs · LangGraph agents · MCP · LanceDB · LLM cost tracking

**Backend** — Python · FastAPI · Pydantic v2 · SQLAlchemy · PostgreSQL · Node.js

**Frontend** — React · Next.js · TypeScript · Redux Toolkit · TanStack Query · Tailwind

**Infra** — AWS (ECS/Fargate, RDS, S3) · Terraform · Fly.io · Docker · GitHub Actions · Sentry · CloudWatch

## 🧭 Earlier

Full-stack at product startups (**Innovaccer**, **Geeks Invention**). Now building AI systems end to end.

`Off the clock`: singing and tactical shooters (Valorant, CS :video_game:)
