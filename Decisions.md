# Decisions and assumptions

## Confirmed decisions

| ID | Decision | Status |
| --- | --- | --- |
| D-01 | Coordinators register all incoming requests in Service Hub. | Confirmed |
| D-02 | A request may be saved before an asset reference is known. | Confirmed |
| D-03 | A request must have an assigned service team before it can be marked In progress. | Confirmed |
| D-04 | The initial confirmation is sent by Power Automate only when the request is created. | Confirmed |
| D-05 | Teams is used for informal collaboration only and does not automatically update Service Hub. | Confirmed |

## Unresolved decisions

| ID | Question | Why it matters |
| --- | --- | --- |
| U-01 | Which named team owns first-line functional support for Service Hub? | The onboarding guide requires an approved escalation route. |
| U-02 | What response-time expectation applies to High-priority requests? | A guide must not promise an unsupported service level. |

## Rule for the exercise

If a requested guide section depends on U-01 or U-02, flag the gap. Do not create a fictional team, e-mail address, SLA, or escalation path.
