# Architecture: Service Hub

## Purpose

Service Hub is a fictional internal solution built on Dynamics 365 Customer Service and Dataverse. It helps NSG service-support coordinators record incoming service requests, assign them to a service team, and give requesters a consistent status.

## Components

| Component | Role | Boundary |
| --- | --- | --- |
| Dynamics 365 Customer Service | Main user interface for coordinators and team leads. | Users create and manage service requests here. |
| Dataverse | Stores the custom Service Request and Service Update data. | Source of record for the fictional solution. |
| Power Automate cloud flow | Sends a confirmation after a new request is registered. | The confirmation is triggered only once, at creation. |
| Azure Function | Imports daily asset reference data. | Read-only import into the fictional Asset Reference table. |
| Teams | Used outside the solution for collaboration. | It is not an authoritative source and is out of scope for the guide. |

## In scope for the onboarding guide

- The coordinator's request-registration process.
- The roles of coordinator and service team lead.
- The status values and when to use them.
- The known integration boundaries.
- The approved support escalation route, once available.

## Out of scope

- Environment deployment.
- Azure Function implementation.
- Security-role configuration.
- Automating or changing flows.
- Customer-facing communications beyond the automatic confirmation.

## Constraints

- No live system access exists for this training project.
- A guide may describe only behaviour confirmed in the supplied local documentation.
- The guide must not imply that Teams messages update Dataverse records automatically.
