# Vivameda research

Vivameda builds company intelligence from a longitudinal workforce panel: how organisations were staffed, structured and skilled, year by year, from 1950 to 2020, joined to a current observation layer for 2018 onward. This repository publishes what we have tested with it, what held up, and what did not.

Every result below is an aggregate from a dated study with its sample size and test status. Several are negative. We publish those too, because a reader who can see where the panel fails has a reason to believe where it works.

## The panel in one paragraph

4M+ companies, 48M observed company-year records, 1.88B skill rows, 46.5M capability buckets, 100+ countries. The historical layer (1950 to 2020) is frozen and reconstructed retrospectively from professional profiles; the current layer refreshes every three to four weeks. Counts are observed profiles, not payroll employees, and missing is never treated as zero. More in [PANEL.md](PANEL.md).

## Results register

| Finding | Status | Study |
|---|---|---|
| Functional breadth in 2019 predicts acquisition by 2026: growing companies with 8+ functions were acquired at 17.8% vs 2.6% for the rest (p=0.0011) | Pre-registered, one cohort, few events | [Acquisition and attrition](studies/acquisition-and-attrition.md) |
| 35% of a 2019 target list was no longer an independent business by 2026 | Pre-registered base rate | [Acquisition and attrition](studies/acquisition-and-attrition.md) |
| Workforce growth does not predict survival (65.3% vs 65.3% still independent, p=1.000) | Pre-registered null | [Acquisition and attrition](studies/acquisition-and-attrition.md) |
| A "scale fast, broad, engineering-heavy" configuration gives back more than half its expansion more often: held-out cohort 18.4% vs 7.9%, RR 2.33, p=7.4e-06 | Held-out confirmed, one blind cohort | [Scale then give back](studies/scale-then-give-back.md) |
| Capability turnover widens outcomes rather than setting direction; higher scaling probability in 6 of 6 momentum and age cells | Development result, 77,589 companies | [Capability turnover](studies/capability-turnover.md) |
| Generic next-year growth forecasting does not beat simple persistence (log error 0.0597 to 0.0676 vs 0.0488) | Negative, published | [Growth forecasting null](studies/growth-forecasting-null.md) |
| A model's apparent edge came mostly from a data-quality field; with it removed, no robust advantage remained | Negative, internal audit | [Model audit](studies/model-audit-quality-artifact.md) |
| Does pre-2021 workforce structure rank later winners among US listed companies? | Frozen before outcomes opened; running | [Blind forward test](studies/software-blind-test.md) |

Falsified along the way: that an outside operator arrives 12 to 24 months before a sale (none of four known deals showed it), and that quality or regulatory capability, or a falling operations share, predicts three-year headcount outcomes.

## What we take from it

The panel is weak at the question most people ask first, "will this company grow next year?" Recent momentum answers that better, and we say so. Where it earns its keep is in structure and long horizons: how broad an organisation is, how its capabilities turn over, which configurations reverse. Those signals are invisible in a headcount line, and on the tests so far some of them carry real information about acquisition and reversal. One blind cohort is not a law; replication is the next job.

## Read further

- [PANEL.md](PANEL.md): coverage, layers, and what an observed profile is and is not
- [METHODS.md](METHODS.md): how studies are frozen, scored and reported
- [TOOLS.md](TOOLS.md): the research tool surface an agent calls, with an illustrative request
- [Exelixis case study](case-studies/exelixis.md): one real company, read through the panel next to its filings
- [Synthetic samples](samples/): 15 fictional question and answer examples for agent builders
- [Publication policy](PUBLICATION_POLICY.md): what we publish and what we never do

Applied work using the same methods: [vivameda-prediction-markets](https://github.com/Oli-Vivameda/vivameda-prediction-markets) and [vivameda-blockchain](https://github.com/Oli-Vivameda/vivameda-blockchain).

Research findings, not investment advice. No licence is granted: published for review, all rights reserved. Vivameda Ltd, Cyprus, [vivameda.com](https://vivameda.com).
