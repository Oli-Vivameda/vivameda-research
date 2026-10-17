# Publication policy

Applies to Vivameda's public repositories (vivameda-research, vivameda-prediction-markets and vivameda-blockchain). Adopted 17 October 2026.

The goal is a verifiable public record: methods, pre-registrations, aggregate results and failures are public; anything that would expose people, clients, licensed data, the engine itself or live trading signals is not.

## Public

- Study questions, frozen designs, specification hashes and test status.
- Aggregate results: counts, rates, effect sizes, p-values, intervals, errors, including negative results and the reason a study failed.
- Coverage figures and the known limits of the panel.
- Case studies of real companies built from public filings plus approved descriptive panel aggregates.
- Synthetic examples and illustrative interface documentation.
- For the research services in the other two repositories: source code, tests and installers.

## Public after a delay

- Individual alerts and decisions in the trading research are published no earlier than 24 hours after the event, with a hash committed at event time (planned; not yet implemented for every lane).
- Results of a sealed study are published when the study closes, with the hashes committed at the start.

## Never public

- Row-level panel data, person-level records, raw provider responses and runtime databases.
- The research engine's source code, model weights and scoring internals.
- Names of upstream data providers and the terms of any data or partnership agreement.
- Client and prospect names, client work, mandates and personal data.
- Private keys, API keys, tokens, passwords and environment files.
- Server IP addresses, hostnames, endpoints, SSH users and key names.
- Trading wallet addresses and live positions.

## Wording

Results are research findings, not investment advice. Observed profiles are not employees. Retrospective reconstructions, backtests, paper results and peak multiples are labelled as such and never presented as forecasts or realized profit. No claim without the aggregate it rests on.

## Before every push

1. No secrets, hosts, endpoints, provider names, client names or row-level data in the diff.
2. Every number traces to a dated study record.
3. New results are aggregates, or delayed releases under the rules above.
4. Claims match the published numbers, including the unflattering ones.
