# Architecture Overview

> This is a living reference. Update it whenever a change affects the
> structure, responsibilities, data flow, infrastructure, security posture, or
> roadmap of the system.

## 1. Project Structure

The repository is currently documentation-first. Application directories are
introduced only after product and technology decisions are approved.

```text
[Project Root]/
├── docs/
│   ├── ARCHITECTURE.md       # Living system architecture reference
│   └── product-specs/        # One product specification per capability
│       ├── README.md         # Product-specification index and conventions
│       └── _template.md      # Starting template for a new specification
├── AGENTS.md                 # Required operating instructions for agents
├── README.md                 # Repository index (not a quick-start guide)
└── .gitignore                # Intentionally untracked files
```

When implementation starts, add the selected application directories here and
describe their ownership and boundaries. A possible future shape is:

```text
backend/      # Server-side APIs, domain logic, persistence, and tests
frontend/     # Client application, UI components, API services, and tests
common/       # Shared types and utilities, when justified by the stack
scripts/      # Repeatable automation
.github/      # CI/CD workflows and repository automation
```

## 2. High-Level System Diagram

No runtime system exists yet. The expected direction, subject to an approved
product specification, is:

```text
[User] <--> [Frontend Application] <--> [Backend Service] <--> [Primary Data Store]
                                      |
                                      +--> [External Integrations]
```

Update this diagram with the real components and data flow before introducing
production infrastructure.

## 3. Core Components

No application components have been selected or implemented.

### 3.1. Frontend

- Name: Not selected.
- Description: To be defined in the relevant product specification.
- Technologies: Not selected.
- Deployment: Not selected.

### 3.2. Backend Services

No backend services exist yet. For each service introduced, document its name,
responsibility, technologies, deployment target, and owned interfaces here.

## 4. Data Stores

No persistent data store has been selected. Before adding one, record its
purpose, owner, data classification, key schemas or collections, backup plan,
and retention policy in this section.

## 5. External Integrations / APIs

No external integrations are configured. Document each integration's purpose,
authentication method, data exchanged, failure handling, and owning component.

## 6. Deployment & Infrastructure

- Cloud provider: Not selected.
- Key services: Not selected.
- CI/CD pipeline: Not selected.
- Monitoring and logging: Not selected.

## 7. Security Considerations

No authentication or authorization system has been selected. Before handling
user or production data, define the authentication model, authorization model,
encryption controls, secret management, and audit expectations here.

## 8. Development & Testing Environment

There is no runnable application yet. When implementation begins, document
local setup, test frameworks, code-quality tooling, and required checks here.

## 9. Future Considerations / Roadmap

- Create the first product specification from
  [`docs/product-specs/_template.md`](product-specs/_template.md).
- Select the application stack and update this document before implementation.
- Define deployment, observability, and security requirements before the first
  production release.

## 10. Project Identification

- Project name: ACDC Repository Template
- Repository URL: https://github.com/fredngg/acdc-repo-template
- Primary contact/team: fredngg
- Date of last update: 2026-07-14

## 11. Glossary / Acronyms

- **Product specification**: A document that defines a capability's user
  problem, scope, requirements, and acceptance criteria.
- **Architecture reference**: This document; the current record of system
  structure and technical boundaries.
