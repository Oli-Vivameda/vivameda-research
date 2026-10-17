# Synthetic samples

15 fictional question and answer examples showing how a Vivameda-backed agent separates observation, hypothesis and limits. Every row is manually authored and synthetic: no panel or provider records were used, the companies are fictional, and `reference_sample_size` and `outcome_rate` are always null. These are illustrations of reasoning, not engine output or evidence of performance.

| Use case | Examples |
|---|---:|
| Strategy reasoning | 5 |
| Company comparison | 4 |
| Reference forecasting | 4 |
| Diligence | 2 |

File: [samples.jsonl](samples.jsonl). Filter on `use_case`. Fields: `sample_id`, `synthetic`, `company`, `use_case`, `question`, `answer`, `reference_sample_size`, `outcome_rate`, `limitations`.

The same set is published on Hugging Face as `Vivameda/synthetic-intelligence-samples`.
