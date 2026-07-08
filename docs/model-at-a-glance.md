# The Model at a Glance

> **One page that ties every piece together — the reframe, the roles, the flow, the funding, and how they reinforce each other.**

---

## The whole model in one diagram

```mermaid
flowchart TB
    subgraph CAUSE["The trigger"]
        AI["AI compresses build<br/>(~20–30% of lead time)"]
        AI --> BN["Bottleneck relocates<br/>upstream to requirements"]
    end

    subgraph RESPONSE["The operating-model response"]
        direction TB
        PO["<b>PO runs a requirements<br/>supply chain</b><br/>discovery → spec → ready buffer"]
        SPEC["<b>Executable specs</b><br/>human- and agent-ready<br/>(Definition of Ready)"]
        TEAM["<b>Durable Outcome Teams</b><br/>engineers orchestrate agents,<br/>QA writes evals, design stewards system"]
        FLOW["<b>Continuous flow</b><br/>WIP limits replace big-batch<br/>sprints & PI planning"]
        PO --> SPEC --> TEAM --> FLOW
        FLOW -. "pull signals starvation risk" .-> PO
    end

    subgraph ENABLERS["What makes it run"]
        PLAT["Platform / agentic catalog<br/>(the multiplier)"]
        AGENTS["PO agents<br/>(discovery, spec, edge-case,<br/>consistency, readiness)"]
        FUND["Outcome funding<br/>(rebalanced envelope)"]
    end

    BN --> PO
    PLAT -.-> TEAM
    AGENTS -.-> SPEC
    FUND -.-> TEAM

    style AI fill:#40916c,color:#fff
    style BN fill:#9b2226,color:#fff
    style PO fill:#2d6a4f,color:#fff
    style SPEC fill:#2d6a4f,color:#fff
    style TEAM fill:#2d6a4f,color:#fff
    style FLOW fill:#2d6a4f,color:#fff
    style PLAT fill:#1b4332,color:#fff
    style AGENTS fill:#1b4332,color:#fff
    style FUND fill:#1b4332,color:#fff
```

---

## How the pieces reinforce each other

| Piece | Solves | Depends on | Detailed in |
|---|---|---|---|
| **Requirements supply chain** | Team starvation as build speeds up | Executable specs + PO agents | [Operating Model](future-delivery-operating-model.md) |
| **Upstream blockers cleared** | The real waits that starve a fast team | Decisions, context, clarity owned upstream | [Upstream Blockers](upstream-blockers.md) |
| **Executable specs** | Ambiguity that stalls humans and agents | Definition of Ready | [PO Spec Template](po-spec-template.md) |
| **Durable Outcome Teams** | Context tax of re-forming project teams | Outcome funding | [Team Shape & Roles](team-shape-and-roles.md) |
| **Continuous flow** | Batch delay from sprints / PI planning | WIP limits + ready buffer | [Governance & Cadence](governance-and-cadence.md) |
| **Outcome funding** | Spend stuck where value is not constrained | Flow metrics as evidence | [Funding & Operating Budget](funding-and-operating-budget.md) |
| **Platform / agentic catalog** | Every team reinventing tooling | Funded as an internal product | [Team Shape & Roles](team-shape-and-roles.md#the-supporting-teams) |

The system is **self-reinforcing**: better specs feed the supply chain → the supply chain keeps durable teams busy → durable teams compound context → context makes agents more effective → agents make specs cheaper to produce. Break any link and the team starves or the speed is wasted.

---

## The flow of value, end to end

```mermaid
flowchart LR
    D["Discovery<br/><i>PO + Designer, one horizon ahead</i>"] --> S["Specification<br/><i>PO + agents, build-ready</i>"]
    S --> RB[(Ready Buffer)]
    RB --> B["Build<br/><i>Engineers + agents</i>"]
    B --> R["Run<br/><i>whole team owns production</i>"]
    R -. "outcome data" .-> D

    style D fill:#40916c,color:#fff
    style S fill:#2d6a4f,color:#fff
    style RB fill:#1b4332,color:#fff
    style B fill:#2d6a4f,color:#fff
    style R fill:#40916c,color:#fff
```

The center of gravity sits **upstream**: discovery and specification are the new constraint, so that is where the team's effort — and the budget — concentrate.

---

## Where to go next

- **Two-minute leadership version** → [Executive Summary](executive-summary.md)
- **The full argument** → [The Operating Model](future-delivery-operating-model.md)
- **What actually blocks us upstream** → [Upstream Blockers](upstream-blockers.md)
- **How teams are shaped** → [Team Shape & Roles](team-shape-and-roles.md)
- **How work is governed** → [Governance & Cadence](governance-and-cadence.md)
- **How it is funded** → [Funding & Operating Budget](funding-and-operating-budget.md)
- **The keystone artifact** → [PO Spec Template](po-spec-template.md)
