# Research tool surface

Vivameda's research engine is exposed to agents as MCP tools. Today these run under owner access; client access is a separate release gate and is not announced here. The engine itself, its data and its endpoint are not public.

| Tool | What it answers |
|---|---|
| `company_search` | Resolve a company to its panel identity by domain or name, with match evidence |
| `company_intelligence` | Summary of one company: historical series, current state, coverage and caveats, each source kept separate |
| `historical_workforce` | Observed-profile series by year, with gaps named rather than filled |
| `role_analysis` | Functional composition over time, with the denominator stated |
| `skill_analysis` | Most-listed skills by period, descriptive only |
| `capability_analysis` | Capability buckets and how they turn over |
| `cohort_stats` | Aggregates for a defined population, with the default filters reported |
| `panel_screen` | Screens of the historical panel against stated criteria |
| `strategy_evidence` | Historical context for a strategy question, anchored to a resolved company |

## Illustrative request

The company ID below is fictional. This is documentation, not a live demonstration.

```json
{
  "jsonrpc": "2.0",
  "id": "demo-1",
  "method": "tools/call",
  "params": {
    "name": "strategy_evidence",
    "arguments": {
      "company_id": "synthetic-example-company",
      "base_year": 2019,
      "question": "Describe observed organizational development and alternative explanations.",
      "include_references": false
    }
  }
}
```

Illustrative shape of an interpretation, not an actual response contract:

```json
{
  "synthetic": true,
  "historical_observation": "Illustrative organizational expansion.",
  "hypothesis": "Expansion could be consistent with a changing operating model.",
  "reference_sample_size": null,
  "reference_outcome_rate": null,
  "next_evidence_needed": "Coverage, entity perimeter and dated corporate context.",
  "forecast_validated": false
}
```

## Rules the tools enforce on an agent

- Ground numbers in returned evidence and keep evidence and version identifiers.
- Separate observations, hypotheses and actions.
- Observed profiles are not employees. Missing is not zero.
- Peer context is not automatically a matched reference class.
- A refused or unavailable result stays unavailable; it is not estimated around.
- Historical outcomes do not by themselves establish transfer to current companies.
- No individual probability from a single named analogue.
- Bad queries are refused rather than answered: unknown keys, inverted year ranges and out-of-range options return an error with the correct form.

For an integration or data partnership discussion: [vivameda.com](https://vivameda.com).
