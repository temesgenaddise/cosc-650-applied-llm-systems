# Week-3 Prompt Engineering Artifact: Security Code-Review Triage

- This project evaluates two versions of a structured prompt for classifying code-review findings as `LOW`, `MEDIUM`, `HIGH`, or `CRITICAL`.

## What is included

- `prompts/v1.txt` and `prompts/v2.txt`: system messages, four few-shot examples, and concise rationale scaffolding.
  
- `data/test_case: 12 input/expected-output pairs.
  
- The only prompt edit in v2 is an added authentication-bypass rule.

- The recorded evaluation uses a deterministic prompt-conditioned fixture backend so the experiment can be rerun without an API key.

- This backend is appropriate for testing the evaluation pipeline, but it is not evidence of a language model's quality.
  
- To evaluate an actual model, replace `FixtureBackend.generate()` with a local or API model call; all scoring and report code remains unchanged.

