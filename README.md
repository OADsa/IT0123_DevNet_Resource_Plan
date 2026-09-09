# IT0123 DevNet Resource Validation Plan

## Student and Project

- Name: Kris Derick C. Odda
- Section: TN24
- Repository name: `it0123-devnet-resource-plan`

## Purpose

Selecting the correct DevNet resource prevents using an environment that does not match the task's access, isolation, setup, or learning requirements. It also makes the development plan more reproducible because the selection is supported by official Cisco documentation and preserved through Git.

## Validated Resource Decisions

- **UC1 — Quick read-only API exploration:** `always-on-sandbox`. The key requirement is immediate shared access for safe read-only API exploration without administrative changes or provisioning time. Official evidence: https://developer.cisco.com/docs/sandbox/
- **UC2 — Private configuration testing:** `reservation-sandbox`. The key requirements are private access, administrative control, and configuration testing, with time available for reservation and setup. Official evidence: https://developer.cisco.com/docs/sandbox/
- **UC3 — Guided API concept practice:** `learning-lab`. The key requirement is structured, step-by-step learning content before independent API work. Official evidence: https://developer.cisco.com/learning/
- **UC4 — Reusable automation example:** `code-exchange`. The key requirement is examining existing Cisco and community code repositories for network-automation examples. Official evidence: https://developer.cisco.com/codeexchange/

## AI Evaluation

The AI recommendations were accepted because each recommendation matched the decisive requirement in the supplied scenario and the resource descriptions in the activity guide. The selections were independently checked against official Cisco DevNet pages. The AI output was treated as provisional rather than as the evidence itself.

## Validation Evidence

- Validator result: `VALIDATION COMPLETE: 9/9 checks passed.`
- Command used: `python validate_plan.py`
- Official Cisco pages reviewed:
  - https://developer.cisco.com/docs/sandbox/
  - https://developer.cisco.com/learning/
  - https://developer.cisco.com/codeexchange/

## Git Evidence

- Initial commit message: `Initialize DevNet resource validation plan`
- Validation commit message: `Validate DevNet resource decisions`
- Output of `git log --oneline`:

```text
2a35363 Validate DevNet resource decisions
4e806be Initialize DevNet resource validation plan
```

Replace the two placeholder log lines above with the actual hashes/output after running Git locally.

## AI-Use Disclosure

AI tool used: ChatGPT. It was used to recommend one DevNet resource type for each fictional scenario and to summarize the reasoning behind each recommendation. The resource type, access model, intended use, and official Cisco evidence were independently checked against Cisco documentation. The final selections and wording were revised into the required validator labels and plan structure.
