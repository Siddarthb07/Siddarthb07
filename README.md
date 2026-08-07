<p align="center">
  <img src="assets/hero-issue-001.png" alt="ISSUE 001 — Operator Dossier — Siddarth Boggarapu — applied ML, production systems, physical simulation" width="100%" />
</p>

# Siddarth Boggarapu

Builder · Bangalore, India  
[Portfolio](https://siddarthb07.github.io/siddarthb/) · [Email](mailto:siddarthb078@gmail.com) · [LinkedIn](https://www.linkedin.com/in/siddarth-boggarapu-12411339b/) · [GitHub](https://github.com/Siddarthb07)

I build systems that operate under uncertainty across finance, healthcare, security, and physical simulation. My work combines machine learning, backend engineering, and physics-based modeling to create systems that are measurable, explainable, and grounded in real-world constraints.

Operating principles: **verify** (look inside, not only at outputs), **simulate** (stress failure modes before reality costs), **refuse** (calibrated abstention when evidence is weak).

Domains I ship in: **LLM interpretability / emotion probes**, **multi-host threat hunting & campaign correlation**, **quantitative trading research**, **clinical risk scoring**, and **drone CFD / scientific ML**.

## Featured projects

### [Anima](https://github.com/Siddarthb07/Anima) — LLM emotion & uncertainty probes
Open-source instrumentation for Hugging Face causal LMs. Forward hooks + probe heads read **valence**, **arousal**, and **uncertainty** from hidden states per token, with a guard that can recommend abstaining. FastAPI / WebSocket streaming + dashboard. [HF Spaces demo](https://huggingface.co/spaces/sidb078/Anima).  
Keywords: LLM interpretability, emotion probing, Hugging Face, PyTorch, FastAPI.

### [Corvex](https://github.com/Siddarthb07/corvex) — multi-host campaign correlator
Research correlator that fuses weak per-host detectors (lateral auth, micro-exfil, recon fanout) into ATT&CK-shaped attack timelines via HMAC-signed event envelopes. No LLM, no cloud API. **Standing claim:** holds up on sealed synthetic fleets; **not** validated on real enterprise telemetry or pure-benign baselines yet. Observe-only Windows / macOS sensors; live containment gated / dry-run.  
Keywords: threat hunting, MITRE ATT&CK, lateral movement, SIEM-style correlation, cybersecurity, Python.

### [GeoQuant](https://github.com/Siddarthb07/GeoQuant) — quantitative trading platform
FastAPI + PyTorch stack for ML daily/intraday signals, news sentiment, walk-forward backtesting with costs in the loop, and Alpaca paper-trade routing.  
Keywords: algorithmic trading, quantitative finance, backtesting, sentiment analysis, Alpaca.

### [Drift](https://github.com/Siddarthb07/Drift) — clinical risk + health tracking
Flask health platform whose runtime path uses published **ACC/AHA Pooled Cohort** and **FINDRISC** models (not invented scores), plus a 17-biomarker timeline, wearables OAuth, and hard gates when data is incomplete.  
Keywords: clinical risk, health tracker, biomarkers, explainable ML, Flask.

### Aerospace / scientific ML
Self-driven CFD and simulators used to design aircraft I physically build and fly (plus a **10-day** IISc vortex-ring internship, May 2025 — the repos are personal work that predates and continues independently of IISc):

| Repo | What it is |
| --- | --- |
| [Drone-Vortex-Ring-Simulation](https://github.com/Siddarthb07/Drone-Vortex-Ring-Simulation) | Reduced-order vortex rings — Kelvin Γ, Helmholtz self-induction, viscous decay |
| [Propeller-simulator](https://github.com/Siddarthb07/Propeller-simulator) | BEMT propeller performance sweeps (GUI + CLI + CSV) |
| [vortex-tracker](https://github.com/Siddarthb07/vortex-tracker) | OpenCV ring diameter / propagation speed from high-speed imagery |
| [NeuralVortex](https://github.com/Siddarthb07/NeuralVortex) | ML surrogate (TFNO / Conv3D path) on own CFD volumetric fields |

Keywords: vortex ring, drone aerodynamics, CFD, fluid dynamics, Fourier Neural Operator, BEMT.

### Also public
[text2sql-rag](https://github.com/Siddarthb07/text2sql-rag) (clean-room Spider text-to-SQL RAG) · [VidhiSethu](https://github.com/Siddarthb07/VidhiSethu) (Indian-legal RAG architecture docs) · [homelab-rpi](https://github.com/Siddarthb07/homelab-rpi) · [cursor-llm-council](https://github.com/Siddarthb07/cursor-llm-council)

## Experience

**Summer Intern — Indian Institute of Science (IISc), Bangalore** · May 2025 · **10 days**  
Vortex-ring internship; built [vortex-tracker](https://github.com/Siddarthb07/vortex-tracker). CFD / simulation portfolio is self-driven, not an IISc research fellowship.

**Engineering Intern — Vegam Solutions** · Q3 2025 – Q1 2026  
Air-filtration engineering (Q3); text-to-SQL RAG pipeline (Q1, **NDA**). Portfolio proof: [text2sql-rag](https://github.com/Siddarthb07/text2sql-rag) on the public Spider benchmark.

**Founder — [Athera](https://athera.digital)** · Ongoing  
AI automation, lead workflows, and websites for small businesses.

**Co-founder — ORQIS AI** · Ongoing  
Detect silent agent failures (e.g. tool-call loops), explain them, and open reviewable patches with a human in the loop.

## Stack

Python · TypeScript · PyTorch · Hugging Face · FastAPI · Next.js · Flask · Postgres · Qdrant · Redis · Docker · Linux · Raspberry Pi

## Outside code

Competitive skating, football (CBSE / Goa Globe), badminton, swimming · Model UN · 50+ hrs community service (including NGO web presence).

---

[Open the full interactive dossier (live sims) →](https://siddarthb07.github.io/siddarthb/)
