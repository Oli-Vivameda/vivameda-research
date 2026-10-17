# Capability turnover

Development result, 17 September 2026.

## Definition

Of a company's ten most-listed capabilities in year T, how many are still in its top ten at T+3. Retaining five or fewer is high turnover. This is only computable from a longitudinal panel; a current snapshot cannot show it.

## Design

77,589 US companies. Base 2013, midpoint 2016, outcome 2019. Conditioned on each company's own 2013 to 2016 momentum and an age control.

## Results

Turnover widens the distribution of outcomes rather than pointing one way. High-turnover companies had a higher scaling probability in 6 of 6 momentum and age cells (sign test p=0.016). What that means depends on where the company starts:

| Starting state | Outcome | High turnover | Low turnover | Effect |
|---|---|---:|---:|---|
| Younger, shrinking (n=2,600) | Further contraction | 55.8% | 67.0% | p=5.7e-09 |
| Established, mid momentum | Scaling | 4.2% | 2.0% | OR 2.14, p=2.8e-10 |
| Fast growers | Contraction | 25.3% | 20.2% | OR 1.34, p=0.0004 |

For a shrinking company, turnover reads as repositioning. For a fast grower, it is a caution.

## Limits

- Development result on one base year. Not yet transferred to the current layer, which needs employee-level skill data.
- A widener, not a direction: it must be read inside the momentum cell.
- The obvious counter-example is real. Aldevron retained only 5 of 10 twice during its build-out and was then acquired by Danaher for USD 9.6bn. High turnover is not a distress label.

## The qualitative side

What turns over matters more than how much. Between 2015 and 2020 Synthego lost MATLAB, C++, engineering, genomics and R&D from its top ten and gained cell culture, PCR, biochemistry and office capabilities: a sideways move within discovery, away from the automation thesis it was founded on.
