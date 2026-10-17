# Model audit: an edge that came from a quality field

Internal audit, 8 October 2026. Retrospective reconstruction.

## Background

An earlier gradient-boosted model scored well on three three-year tasks: A doubling, B contraction to 70% or less, C reversal after at least 50% prior expansion. Before using it, we audited what it was actually learning. Development cohorts 2012 and 2013, validation 2014. The original scores reproduced exactly.

## What the audit found

| Task | Arm | Validation AUC | Top-20% lift vs momentum |
|---|---|---:|---:|
| B contraction | Original model | 0.849 | 1.62 |
| B contraction | Momentum only | 0.613 | 1.00 |
| B contraction | Without quality fields | 0.728 | 0.94 |
| C reversal | Original model | 0.777 | 1.61 |
| C reversal | Momentum only | 0.574 | 1.00 |
| C reversal | Without quality fields | 0.687 | 1.37 |
| C reversal | Minimal allowlisted core | 0.598 | 0.82 |

The single most important feature in both B and C was `has_dates_pct`, the share of profiles that carry dates. That is a property of how the data was collected, not of the company. Removing the quality fields cut AUC by 0.12 on B (paired company bootstrap interval -0.158 to -0.087) and by 0.09 on C (-0.130 to -0.047), which triggered our pre-registered warning.

After also removing tenure, industry and country, reversal lift fell to 0.99 (interval 0.72 to 1.34). The minimal allowlisted core reached 0.82. No robust commercial advantage remained.

## Decision

The original model was not promoted and no target was marked validated. Quality fields are now quality-only, tenure and collection metadata are quarantined, and any new numerical test needs a fresh pre-registration and an unexposed cohort.

## Why publish this

Leakage like this is common and usually goes unreported. A model that looked like a 1.6x edge was mostly reading the data's own fingerprints. Catching that before a client saw it is the method working.
