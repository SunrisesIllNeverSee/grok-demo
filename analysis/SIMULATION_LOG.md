# Simulation Log

| Version / Area | Parameters | Reported Result |
| --- | --- | --- |
| v7 baseline | 20M tokens; no persona fusion; no storage hydration | Witness bandwidth ceiling 1.2 Gbps; 94% detection at 28% churn; tails avg 620ms, p99 <680ms; ghosts <3%. |
| v8 entropy gradients | 100 sync events at 20M scale | Entropy predicted failures in 1.8s avg at 94% accuracy; variance in 3.7s avg at 82%. |
| v11 drift baseline | Used as comparison baseline for v12+ poisoning | Recovery defined as drift returning within +0.2% of baseline and promotions resuming. |
| v12+ poisoning | Sweep poisoning at 5/10/15/20% churn | Metrics requested: FN <1%, FP <5%, blast radius, containment cycles, full-resume timing. |
| v17/v18+ governance | Provenance quorum, exception authority, legitimacy credits | Hardening shifts toward pruning exception authority and pricing recovery in legitimacy credits. |
| v19 capstone | Meaning, truth stagnation, future drift, refusal dominance, xAI federation | Invariant entropy baseline, truth-stagnation acceptance, predictive residue modeling, adaptive quorum scaling, reserve legitimacy credits. |

These values are preserved as claims made in the thread. They are not independently reproduced benchmark measurements.
