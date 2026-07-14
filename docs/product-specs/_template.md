# [Capability Name]

## Status

Draft | In discovery | Approved | In development | Released | Superseded

## Target goal

State one measurable outcome. Name the target user, the metric and baseline (if
known), the target value, the measurement window, and the core constraints.

- Target user:
- Outcome metric and baseline:
- Target and measurement window:
- Core constraints (time, cost, performance, compatibility, policy):

## User scenario

Anchor the work in one specific, contextual scenario. Describe who the user is,
what they are trying to accomplish, what triggers the need, and the context
that should guide product and engineering trade-offs.

## Problem

State the evidence, likely cause, and user impact. Link to research, support
data, analytics, or incident evidence. Do not substitute vague diagnostics or
unsupported speculation for evidence.

- Evidence:
- Cause or contributing conditions:
- User impact:

## Scope

List exactly what this change includes: affected surfaces, components, APIs,
data, and user groups. These boundaries constrain implementation; do not expand
them without updating this specification.

## Boundaries and non-goals

List tempting but strictly forbidden changes. Be explicit about adjacent
modules, redesigns, migrations, integrations, or policy changes that are not
part of this work.

- Not in scope:
- Do not change:

## Functional requirements

Number the required behaviors. Each requirement should be precise enough to
trace to one or more acceptance criteria and tests.

1.

## Data model and source assumptions

Name the fields, entities, ownership, lifecycle, and source-of-truth
assumptions. Include validation rules, defaults, transformations, retention,
and migration needs where relevant. Do not invent fields or sources that are
not listed here.

| Entity or event | Field | Type / format | Source of truth | Rules and assumptions |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |

## UX and interaction contract

Describe the expected flow, states, timing expectations, accessibility needs,
and error behavior as observable outcomes.

- Primary flow:
- Loading and pending states (including timing expectations):
- Empty states:
- Error and recovery behavior:
- Permission-denied behavior:
- Accessibility and responsive requirements:

## Acceptance criteria

Write observable, measurable scenarios. Prefer Given/When/Then statements with
specific data, outcomes, and time bounds.

- [ ] Given ..., when ..., then ... within ...

## Failure and edge cases

List known boundary failures before implementation so agents do not hallucinate
assumptions. Include invalid input, missing or stale data, concurrent changes,
timeouts, partial failures, retries, and unsupported permissions where they
apply.

| Condition | Expected behavior | User-facing message or recovery | Test coverage |
| --- | --- | --- | --- |
|  |  |  |  |

## Security and privacy

Name sensitive data, trust boundaries, authentication and authorization rules,
retention requirements, and forbidden behaviors. State concrete constraints,
such as data that must not be logged, exposed, stored, or sent to third-party
services.

- Sensitive data and classification:
- Required access controls:
- Encryption, retention, and audit requirements:
- Forbidden behaviors:

## Observability

Specify privacy-safe telemetry needed to evaluate behavior after release. Name
events, metrics, dimensions, alert thresholds, dashboards, and owners. Do not
collect unnecessary personal or sensitive data.

| Signal | Type | Trigger / definition | Dimensions | Privacy constraint | Owner |
| --- | --- | --- | --- | --- | --- |
|  | Event / metric / log / trace |  |  |  |  |

## Test plan

Mandate the exact tests, scenarios, fixtures, and evidence needed to prove the
change. Cover each acceptance criterion and relevant failure or edge case.

| Behavior or scenario | Test level | Fixture or setup | Expected evidence |
| --- | --- | --- | --- |
|  | Unit / integration / E2E / manual |  |  |

## Technical and architectural impact

Describe the affected components, interfaces, data stores, operations, and
tests. Link to the relevant sections of `docs/ARCHITECTURE.md`, and update that
document in the same change when architecture is affected.

## Rollout and controlled delivery

Define how the feature is exposed: flags, cohorts, migration sequencing,
backward compatibility, rollback, owners, and communication. Set explicit
success triggers and expansion rules before increasing exposure.

- Initial exposure:
- Entry and expansion criteria:
- Success metrics and thresholds:
- Rollback trigger and procedure:

## Risks and mitigations

Identify plausible failure modes introduced by this change and give each a
concrete mitigation, owner, and contingency.

| Risk | Likelihood | Impact | Mitigation | Owner | Contingency |
| --- | --- | --- | --- | --- | --- |
|  | Low / Medium / High | Low / Medium / High |  |  |  |

## Open questions and decisions

| Question or decision | Owner | Status | Due date |
| --- | --- | --- | --- |
|  |  | Open |  |

## Definition of done

List definitive, non-subjective conditions that combine quality gates,
evidence, and review outcomes. The work is not done until every applicable item
is complete.

- [ ] Scope and non-goals were respected; no unapproved adjacent changes were made.
- [ ] Every acceptance criterion and required edge case has passing test evidence.
- [ ] Security, privacy, and observability requirements are implemented and reviewed.
- [ ] Rollout, monitoring, and rollback plans are ready and owned.
- [ ] Relevant `docs/ARCHITECTURE.md` updates are included, if architecture changed.
- [ ] Required code review and product approval are recorded.
