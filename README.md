<div align="center">

## 👋 Hi, I'm Andreas

I build developer tools for systems where small technical changes can create large operational consequences.

Right now, I’m focused on semantic data quality, resilient backend systems, and practical automation.

</div>

<br>

---

<br>

<div align="center">

## 🚀 Current flagship project

</div>

<div align="center">

### 📊 [Semantic Delta Detector](https://github.com/Ryukanchi/semantic-delta-detector)

**Catch metric drift before it becomes a dashboard problem.**

</div>

SQL changes can look harmless while changing what a KPI actually means. Semantic Delta compares changed SQL files between local Git refs and turns the technical diff into a reviewer-friendly explanation:

> **Changed SQL → Semantic Impact → Why it matters**

<div align="center">

<a href="https://github.com/Ryukanchi/semantic-delta-detector">
  <img src="https://raw.githubusercontent.com/Ryukanchi/semantic-delta-detector/main/docs/assets/decision-report.png" alt="Semantic Delta decision report" width="820">
</a>

</div>

**What already works:**

- Discovers modified and renamed SQL files between Git refs
- Detects changes in populations, filters, aggregations, joins, and time windows
- Explains risk, evidence, business impact, and the recommended reviewer action
- Produces readable text, simulated PR-style reports, and complete JSON output
- Supports optional severity gating for local and CI workflows
- Keeps every discovered file observable as either analyzed or explicitly skipped
- Runs locally without GitHub credentials or real PR posting

**Status:** Usable heuristic MVP. It is an early-warning system for semantic drift, not a SQL validator or truth engine.

<div align="center">

[Explore the repository and examples →](https://github.com/Ryukanchi/semantic-delta-detector)

</div>

<br>

---

<br>

<div align="center">

### 🛡️ [Rollback Engine](https://github.com/Ryukanchi/rollback-engine)

**An event-sourced reliability lab for commands that may have succeeded even when their response was lost.**

</div>

It explores how a backend can recover safely from ambiguous commits, partial execution, retries, stale workers, and corrupted read models without allowing caches or command records to become domain truth.

**What it demonstrates:**

- Event Store as retained domain history and replay as authoritative state
- saga compensation and idempotent command reconciliation
- lease, generation, and fencing-based command ownership
- repairable materialized views, safe event upcasting, and raw lost-ACK confirmation

<div align="center">

`Node.js` · `Express` · `SQLite` · **528 automated tests**

[Architecture, guarantees, and deliberate limits →](https://github.com/Ryukanchi/rollback-engine#why-this-exists)"

</div>

<br>

---

<br>

<div align="center">

### 💬 [Discord Bot “Archivist”](https://github.com/Ryukanchi/discord-bot-archivist)

</div>

A Discord bot designed to preserve **meaningful moments**, instead of storing everything.

It focuses on extracting highlights from conversations in a more selective, useful way.

**Focus areas:**
- community memory
- meaningful highlight detection
- automation inside chat systems
