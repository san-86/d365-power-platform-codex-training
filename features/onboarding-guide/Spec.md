# Specification: Service Hub onboarding guide

## Audience

A consultant who understands the basics of Dynamics 365 and Dataverse but is new to the fictional Service Hub solution.

## Intended outcome

The reader can explain what Service Hub is for, identify the coordinator's responsibility, and understand what must be known before a Service Request moves from registration to active work.

## In scope

The first version of the guide will contain only **Section 1: Getting started with Service Hub**.

Section 1 should cover:

1. The purpose of Service Hub.
2. The coordinator's role at a high level.
3. The distinction between registering a request and starting work.
4. The information required or optional when registering a request.
5. A clearly marked escalation/support gap where approved information is missing.

## Out of scope

- Detailed flow configuration.
- D365 deployment, solution import/export or environment setup.
- Azure Function implementation.
- Service-level commitments.
- A named escalation contact.
- Sections 2+ of the guide.

## Required output

Create `output/Onboarding-guide.md`.

## Open question

The guide must explain what to do when ownership is unclear, but the named service owner and escalation route are unresolved. The guide must flag this instead of inventing a contact.
