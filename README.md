# Delivery Operating Model

> **A future operating model for product and delivery teams reshaping around AI-accelerated development.**

This project defines how product and delivery teams change as development velocity increases through AI and agentic tooling. It focuses on the **Product Owner** role and the shift from managing a backlog to running a **requirements supply chain** — so developers (and their agents) are never starved for build-ready work.

It is intentionally kept **separate from any specific agent catalog or codebase** — it is an operating-model and process reference that can inform any team or program.

---

## Live site

Published via GitHub Pages: **Settings → Pages → Source: GitHub Actions**. Once enabled, the `deploy.yml` workflow builds and publishes on every push to `main`.

---

## Contents

| Document | Purpose |
| --- | --- |
| [docs/future-delivery-operating-model.md](docs/future-delivery-operating-model.md) | The full model: the bottleneck reframe, the requirements supply chain, what changes for the PO, how POs use agents/AI, the agile → continuous-flow shift, industry trends, transition path, and metrics. |
| [docs/po-spec-template.md](docs/po-spec-template.md) | The keystone artifact: the Definition of Ready, an executable spec template usable by both humans and agents, and a worked example. |

---

## The core idea

Development has been compressed by AI, but coding was never the constraint — it is ~20–30% of end-to-end lead time. Speeding up build without changing the surrounding process just **relocates the bottleneck upstream** to requirements and decision latency.

The response:

1. **The PO owns a continuous supply of validated, build-ready work** — measured by whether the team ever has to wait.
2. **Specs become executable** — complete enough that a human _or an agent_ can act without a follow-up meeting.
3. **Discovery runs continuously, one horizon ahead** of delivery.
4. **Agile principles stay; batch ceremonies give way to continuous flow** (Kanban-like), once the flow machinery exists.

---

## Local preview

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve   # http://127.0.0.1:8000
```

## Start here

- New to the model → read [docs/future-delivery-operating-model.md](docs/future-delivery-operating-model.md).
- Ready to change PO practice → adopt [docs/po-spec-template.md](docs/po-spec-template.md).
