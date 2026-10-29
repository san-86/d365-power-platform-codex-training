# Acceptance criteria: Service Hub onboarding guide

The first deliverable passes when all criteria below are met.

| ID | Criterion | How to validate |
| --- | --- | --- |
| AC-01 | The guide contains a heading for Section 1 and explains the purpose of Service Hub in plain language. | Read the section. |
| AC-02 | The guide distinguishes request registration from work starting. | Compare with `Coordinator-quick-notes.md`. |
| AC-03 | The guide states that an assigned service team is required before a request can be marked In progress. | Compare with `Decisions.md` and `Workflow.md`. |
| AC-04 | The guide identifies asset reference as optional at registration. | Compare with `Data-model.md` and `Coordinator-quick-notes.md`. |
| AC-05 | The guide does not state or imply a named escalation contact, response time or unsupported automation. | Search the output and compare with `Decisions.md` and the policy extract. |
| AC-06 | The guide tells the reader to raise uncertain ownership with the designated service owner, while clearly marking that the actual contact is still to be confirmed. | Read the escalation note. |
| AC-07 | No files outside `output/` are changed. | Inspect the changed-file list or Git diff. |

## Deliberate trainer seed

A plausible but unsupported claim may be introduced during the exercise. Validation must rely on the actual output and source files, not on the agent's completion message.
