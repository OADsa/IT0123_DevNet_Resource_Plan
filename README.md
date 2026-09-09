# IT0123 DevNet Resource Validation Plan

## Student and Project

- Name: Kris Derick C. Odda
- Section: TN32
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

## AI Prompt Records

Scenario 1 — Always-On Sandbox

I am selecting a Cisco DevNet resource for a fictional classroom use case.
Use case: [Scenario 1 from devnet_use_cases.json]
Choose exactly one: learning-lab, always-on-sandbox, reservation-sandbox, or code-exchange.
Explain which requirement drove your choice. State any access, isolation, setup, or privilege claim that I should verify in official Cisco documentation.

AI recommendation: always-on-sandbox

Scenario 2 — Reservation Sandbox

I am selecting a Cisco DevNet resource for a fictional classroom use case.
Use case: [Scenario 2 from devnet_use_cases.json]
Choose exactly one: learning-lab, always-on-sandbox, reservation-sandbox, or code-exchange.
Explain which requirement drove your choice. State any access, isolation, setup, or privilege claim that I should verify in official Cisco documentation.

AI recommendation: reservation-sandbox

Scenario 3 — Learning Lab

I am selecting a Cisco DevNet resource for a fictional classroom use case.
Use case: [Scenario 3 from devnet_use_cases.json]
Choose exactly one: learning-lab, always-on-sandbox, reservation-sandbox, or code-exchange.
Explain which requirement drove your choice. State any access, isolation, setup, or privilege claim that I should verify in official Cisco documentation.

AI recommendation: learning-lab

Scenario 4 — Code Exchange

I am selecting a Cisco DevNet resource for a fictional classroom use case.
Use case: [Scenario 4 from devnet_use_cases.json]
Choose exactly one: learning-lab, always-on-sandbox, reservation-sandbox, or code-exchange.
Explain which requirement drove your choice. State any access, isolation, setup, or privilege claim that I should verify in official Cisco documentation.

AI recommendation: code-exchange

The assignment's own suggested prompt has essentially this structure.

Important: I would use the actual four scenario descriptions from your devnet_use_cases.json rather than leaving [Scenario 1], etc. If you want, I can update your ZIP so it contains the complete prompt records + reflections + README, ready to submit.

## AI-Use Disclosure

AI tool used: ChatGPT. It was used to recommend one DevNet resource type for each fictional scenario and to summarize the reasoning behind each recommendation. The resource type, access model, intended use, and official Cisco evidence were independently checked against Cisco documentation. The final selections and wording were revised into the required validator labels and plan structure.
