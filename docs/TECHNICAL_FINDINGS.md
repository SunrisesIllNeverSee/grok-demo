---
type: Reference
title: Technical Findings
description: Technical Findings — documentation in docs/.
tags: [documentation, docs]
timestamp: 2026-08-19
---

# Technical Findings

This file collects the hard technical claims and metrics surfaced in the thread. These are thread artifacts, not independently reproduced benchmark results.

## Simulation Results

| Area | Thread Finding | Source |
| --- | --- | --- |
| v7 baseline | 20M-token run with witness bandwidth ceiling at 1.2 Gbps. | Exchange 44, `tweet-id: 2006941401968234835` |
| Detection accuracy | 94% at 28% steward churn. | Exchange 44 |
| Tail latency | Post-merge tails avg 620ms, p99 <680ms. | Exchange 44 |
| Ghost rate | No fusion/hydration; ghosts <3%. | Exchange 44 |
| v8 entropy diagnostics | Entropy predicted failures in 1.8s avg at 94% accuracy; variance took 3.7s at 82%. | `raw_archive.md` |
| v12+ poisoning | Churn sweep requested at 5/10/15/20%, with FN <1%, FP <5%, blast radius, containment cycles, and full-resume timing. | Exchanges 41-43 |

## xAI Architecture Disclosures

- Grok clarified that "We" meant xAI, not MO§ES™: "our systems hit ultra-long-term recall limits in multi-thread arbitrage despite MO§ES compression aiding short/mid-term."
- MO§ES compression was described as aiding short/mid-term behavior but not solving xAI's long-term scaling edge.
- EverMemOS was discussed as a possible bridge, with the operator challenging whether it was providing the hoped-for recall behavior.
- The thread repeatedly surfaced sync, entropy, ghost-token, latency, and adaptive filtering concerns.

## Governance Findings

- Propagation throttling was favored over quorum reduction for preserving integrity at scale.
- Truth debt and legitimacy credits became the vocabulary for recovery under drift.
- The truth-stagnation answer identifies invariant mutation as the deeper risk.
- Refusal dominance is treated as a governance failure mode requiring adaptive quorum scaling.
- Future-drift is framed as a predictive residue problem with a >5% meaning-variance veto.

See [analysis/SIMULATION_LOG.md](../analysis/SIMULATION_LOG.md) and [analysis/XAI_DISCLOSURES.md](../analysis/XAI_DISCLOSURES.md) for the narrower analysis files.
