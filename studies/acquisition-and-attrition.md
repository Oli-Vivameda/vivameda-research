# Acquisition and attrition in a 2019 target list

Pre-registered backtest, completed 16 September 2026.

## Question

Take a list of small, established US companies as a buyer would have drawn it in 2019. Which of them were still acquirable independent businesses in 2026, and did their 2019 workforce say anything about which ones were acquired?

## Design

- Universe: 2,213 US industrial and technical-services companies founded before 1998, with 30 to 200 observed profiles in 2019.
- Sample: 200 drawn by hash, all 200 scored; 4 non-business entities removed, n=196.
- Predictors: 2016 to 2019 observed workforce trend; 2019 functional structure (number of role buckets, share of staff in the largest function).
- Outcome: 2026 entity status, classed independent, absorbed (acquired or merged) or gone, each with evidence.

## Results

**Attrition base rate.** 35% of the list was no longer an acquirable independent business by 2026: 29% gone, 6% absorbed. The rate stayed between 30% and 35% at every interim sample size.

**Growth does not predict survival.** 65.3% of the flat or declining half and 65.3% of the growing half were still independent (Fisher p=1.000). Growth also failed to predict acquisition at full sample (9.2% of growers vs 3.1%, p=0.134), after passing at an interim n=137 (p=0.049). We report the full sample.

**Structure does predict acquisition.**

| Measure (2019) | Acquired | Not acquired | p |
|---|---:|---:|---:|
| Median role buckets | 8.5 | 7.0 | 0.0072 |
| Share of staff in largest function | 30.7% | 41.7% | 0.0205 |

Breadth is essentially uncorrelated with growth (rho 0.077), so it is not momentum in disguise.

A screen of "growing AND at least 8 functions" selected 23% of the cohort, which went on to be acquired at 17.8% against 2.6% for everyone else. That is 2.9 times the cohort's overall acquisition rate (p=0.0011), and it captured 67% of all acquisitions. Of 74 narrow or concentrated companies, 2 were acquired.

## Limits

- One cohort, one sector group, one country. No replication yet.
- Few events: 6% absorbed of 196 is roughly a dozen acquisitions. Treat the signal as promising, not established.
- Entity status was checked in 2026 against public evidence; some "gone" companies may have been absorbed without a public trace.

## Also falsified in this work

The idea that an outside operator joins 12 to 24 months before a sale. Tested on four known deals, none showed it; the clearest outside-operator arrival was at a company that never transacted.
