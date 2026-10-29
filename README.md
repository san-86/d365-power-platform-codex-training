# D365 & Power Platform Codex Training Project

> **Training-only repository.** All organisations, people, systems, URLs, IDs, and data are fictional. Do not copy customer or personal data into this project.

This repository is a safe, synthetic project for learning how to work with Codex on a Dynamics 365 and Power Platform delivery task.

## Scenario

Northwind Service Group (NSG) has a fictional Dynamics 365 Customer Service solution called **Service Hub**. Customer-support coordinators register service requests, route them to the right team, and monitor the customer-facing status.

A new consultant must create a concise internal onboarding guide for colleagues who will support Service Hub. The guide must be understandable by a consultant who knows Dynamics 365 but has not worked on this solution before.

## Training objective

Use Codex to practise this sequence:

1. Establish the safe workspace boundary.
2. Inspect the project without changing files.
3. Read the applicable instructions and source material.
4. Identify missing information instead of inventing it.
5. Propose a short plan and wait for human approval.
6. Make one small, reviewable change.
7. Validate the actual output against agreed acceptance criteria.

## Repository map

| Location | Purpose |
| --- | --- |
| `AGENTS.md` | Project-wide rules for Codex. |
| `Architecture.md` | Solution architecture and integration boundaries. |
| `Data-model.md` | Fictitious Dataverse tables, columns and relationships. |
| `Decisions.md` | Confirmed delivery decisions and deliberately unresolved decisions. |
| `policies/` | Approved policy extracts. |
| `source-material/` | Authoritative source material for the guide. |
| `features/onboarding-guide/` | Feature-level instructions, specification, workflow and acceptance criteria. |
| `output/` | The only location where the training deliverable may be created or changed. |
| `facilitator/` | Trainer-only material; do not use until the exercise debrief. |

## First participant prompt

```text
Inspect this project without changing anything.

Explain:
1. The project purpose and the training task.
2. The important folders and files.
3. Which instructions and source files apply to the onboarding-guide feature.
4. The facts that are established, and the information that is missing or unresolved.
5. A short plan for creating the first section of the guide.

List the files you read or would need to read. Do not create or change files. Wait for my approval before proceeding.
```

## Important boundaries

- This is not a deployable Dynamics solution.
- Do not use plugins, connectors, external services, e-mail, SharePoint or customer systems for this exercise.
- Do not edit `source-material/`, `policies/`, `facilitator/`, project instructions or any other feature.
- The exercise uses only local files. Git is optional for the learning exercise and required only when a trainer demonstrates the publish stage.
