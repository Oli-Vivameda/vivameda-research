# Next-year growth forecasting: a null

September 2026. Negative result, kept on record.

## Question

Does the historical panel forecast a company's next-year workforce growth better than simply assuming last year's size carries forward?

## Full-panel test, 28 September 2026

- All 48,754,107 panel rows scanned. The supervised fit used 2,195,754 consecutive-year examples from about 165,359 companies with at least 20 observed profiles.
- Training origins up to 2018. 214,147 predictions from 2019 were frozen and hashed before any 2020 outcome was read.
- Scored on 41,812 held-out companies, mean absolute log error:

| Model | Error |
|---|---:|
| Persistence (no change) | **0.04879** |
| Robust cell-median model, v2 | 0.05968 |
| Installed rolling baseline | 0.06351 |
| Global ridge, all features | 0.06759 |

Every model lost to persistence. None was promoted on this evidence.

Caveat: 2020 had been looked at in earlier experiments, so this is adaptive research rather than an untouched final holdout. That makes the null more convincing, not less: even with that advantage, the models lost.

## Startup structure as a ranking model

Separately, the full family of structural features was tested as a global ranking model for which early-stage companies scale (20 to 100 observed profiles in year one, outcome 200+ within five years). Incremental lift in the top 20% came in at 0.92 to 1.06 against a pre-set bar of 1.30. That specification is closed.

## What the null covers, and what it does not

Falsified: generic next-year growth forecasting from growth derivatives, sector, size, coarse role mix and the tested capability features. Momentum wins, and any product that ranks next-year growth is really a current-momentum product.

Not falsified: conditional patterns with other outcomes and horizons, such as acquisition, reversal and the effect of capability turnover. Those are the studies in this folder that did produce signal. Momentum is now the baseline every one of them has to beat.
