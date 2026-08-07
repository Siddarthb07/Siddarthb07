<p align="center">
  <img src="assets/hero-issue-001.svg" alt="ISSUE 001 — Operator Dossier — Siddarth Boggarapu" width="1100" />
</p>

# Siddarth Boggarapu

Bangalore, India · [Portfolio](https://siddarthb07.github.io/siddarthb/) · [Email](mailto:siddarthb078@gmail.com) · [LinkedIn](https://www.linkedin.com/in/siddarth-boggarapu-12411339b/)

I build systems that operate under uncertainty across finance, healthcare, security, and physical simulation. My work combines machine learning, backend engineering, and physics-based modeling to create systems that are measurable, explainable, and grounded in real-world constraints.

*I build the part that catches it before it breaks. That's sort of the whole method.*

## What I work on

| Domain | What that looks like in practice |
| --- | --- |
| **LLM instrumentation** | Probe heads on Hugging Face models for valence / arousal / uncertainty — with a guard that can refuse when readouts look unreliable ([Anima](https://github.com/Siddarthb07/Anima)) |
| **Security research** | Multi-host campaign correlation from weak per-host signals; sealed synthetic eval; containment gated and dry-run only ([Corvex](https://github.com/Siddarthb07/corvex)) |
| **Quantitative finance** | Walk-forward trading research with costs in the optimizer, not assumed away ([GeoQuant](https://github.com/Siddarthb07/GeoQuant)) |
| **Healthcare** | Published clinical risk models (ACC/AHA, FINDRISC) with hard input gates ([Drift](https://github.com/Siddarthb07/Drift)) |
| **Aerospace / CFD** | Simulators I built to understand aircraft I physically assemble and fly ([vortex rings](https://github.com/Siddarthb07/Drone-Vortex-Ring-Simulation), [BEMT](https://github.com/Siddarthb07/Propeller-simulator), [NeuralVortex](https://github.com/Siddarthb07/NeuralVortex)) |

## How I think about systems

Three operating rules (same ones on the [Operator-Verse site](https://siddarthb07.github.io/siddarthb/)):

1. **Verify / look inside** — don't trust outputs alone. Hook internals, measure uncertainty, audit citations and claims.
2. **Simulate when reality costs** — walk failure modes in code or CFD before you pay for them in hardware, money, or patients.
3. **Refuse when uncertain** — a calibrated "I don't know" beats a confident hallucination. Refusal is a feature.

That pattern shows up from drones → simulators → model probes → campaign correlators → clinical gates → agent self-healing.

## Selected projects

### [Anima](https://github.com/Siddarthb07/Anima) — LLM emotion / uncertainty probes

Open-source tooling that attaches forward hooks to Hugging Face causal LMs and reads **valence**, **arousal**, and **uncertainty** from hidden states per token. Includes a guard policy, REST + WebSocket streaming, and a dashboard. Public demo on [HF Spaces](https://huggingface.co/spaces/sidb078/Anima). Useful for interpretability experiments — not a claim that models "feel" anything.

### [Corvex](https://github.com/Siddarthb07/corvex) — multi-host campaign correlator

Research correlator that fuses weak detectors (`lateral_auth`, `micro_exfil`, `recon_fanout`) into one attack timeline via HMAC-signed event envelopes. No LLM, no cloud API. **Standing claim:** holds up on synthetic ATT&CK-shaped fleets with sealed held-out eval; **not** validated on real enterprise telemetry or pure-benign baselines yet. Observe/correlate first; live OS quarantine is unimplemented and gated (`CORVEX_CONTAIN=0`). Windows + macOS observe-only sensors ship for lab use.

### [GeoQuant](https://github.com/Siddarthb07/GeoQuant) — quant trading platform

End-to-end FastAPI stack: MLP daily/intraday signals, news-sentiment scoring, self-learning retrain loop, Alpaca paper routing, walk-forward backtest harness. Designed so costs and slippage live inside the research loop.

### [Drift](https://github.com/Siddarthb07/Drift) — clinical risk + health tracking

Flask health platform whose runtime risk path uses **ACC/AHA Pooled Cohort Equations** and **FINDRISC** — published clinical models, not invented scores. Adds a 17-biomarker lab timeline, Fitbit / Google Fit OAuth, and safety gates that withhold risk when inputs are incomplete.

### Aerospace / scientific ML cluster

Self-driven CFD work (predates and continues independently of a short IISc internship):

| Repo | Role |
| --- | --- |
| [Drone-Vortex-Ring-Simulation](https://github.com/Siddarthb07/Drone-Vortex-Ring-Simulation) | Reduced-order vortex rings — Kelvin Γ scaling, Helmholtz thin-ring self-induction, viscous decay |
| [Propeller-simulator](https://github.com/Siddarthb07/Propeller-simulator) | Working BEMT propeller sweeps (GUI + CLI + CSV) |
| [vortex-tracker](https://github.com/Siddarthb07/vortex-tracker) | OpenCV measurement of ring diameter / speed (built during IISc, May 2025) |
| [NeuralVortex](https://github.com/Siddarthb07/NeuralVortex) | ML surrogate (TFNO / Conv3D path) trained on own CFD fields |

These aren't paper exercises — they're tools for designing and tuning quadcopters and hexcopters I build and fly.

### Other public work worth naming

- [text2sql-rag](https://github.com/Siddarthb07/text2sql-rag) — clean-room text-to-SQL RAG on the public Spider benchmark (portfolio proof after NDA-restricted internship work)
- [VidhiSethu](https://github.com/Siddarthb07/VidhiSethu) — public architecture docs for an Indian-legal RAG with citation audit (application is closed source)
- [homelab-rpi](https://github.com/Siddarthb07/homelab-rpi) — sanitized Raspberry Pi NAS / media / monitoring notes
- [cursor-llm-council](https://github.com/Siddarthb07/cursor-llm-council) — multi-model review council for Cursor that forces a devil's advocate

## Experience

**Summer Intern — Indian Institute of Science (IISc), Bangalore** · May 2025 · **10 days**  
Vortex-ring summer internship. Lab exposure to ring formation / instability; built the OpenCV [vortex-tracker](https://github.com/Siddarthb07/vortex-tracker). The CFD simulators on GitHub are **self-driven personal work**, not an IISc research fellowship extension.

**Engineering Intern — Vegam Solutions** · Q3 2025 – Q1 2026  
- Q3 2025: air-filtration / hardware-flavored engineering  
- Q1 2026: text-to-SQL RAG pipeline (**NDA** — no proprietary internals publicly). Portfolio proof: clean-room [text2sql-rag](https://github.com/Siddarthb07/text2sql-rag) on Spider

**Founder — [Athera](https://athera.digital)** · Ongoing  
AI automation, lead workflows, and websites for small businesses. One operator shipping live systems for clients.

**Co-founder — ORQIS AI** · Ongoing  
Agent monitoring and auto-remediation: detect silent failures (e.g. runaway tool-call loops), explain them, and open reviewable patches / PRs with a human in the loop before merge.

## Stack I use day to day

- **Languages:** Python, TypeScript, some C / GLSL  
- **ML:** PyTorch, Hugging Face, LangChain / local inference tooling  
- **Backend / web:** FastAPI, Next.js, Flask  
- **Data:** Postgres, Qdrant, Redis, DuckDB / SQLite where appropriate  
- **Infra:** Docker, Linux, GitHub Actions, Raspberry Pi homelab

## Outside the repos

Competitive skating, football (including CBSE / Goa Globe), badminton, swimming. Model UN (research + debate). 50+ hours community service, including helping NGOs get basic web presence.

## Links

- **Full interactive dossier (live sims + case UI):** [siddarthb07.github.io/siddarthb](https://siddarthb07.github.io/siddarthb/)  
- **Hero repos:** [Anima](https://github.com/Siddarthb07/Anima) · [Corvex](https://github.com/Siddarthb07/corvex) · [Drift](https://github.com/Siddarthb07/Drift) · [GeoQuant](https://github.com/Siddarthb07/GeoQuant)  
- **Contact:** [siddarthb078@gmail.com](mailto:siddarthb078@gmail.com)
