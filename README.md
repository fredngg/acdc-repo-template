# Architecture Template

A documentation-first repository template for projects that want agents and
contributors to understand the system before changing it.

## Template lineage

This repository is based on the system-architecture template from
[Architecture.md](https://architecture.md/). It deliberately modifies that
foundation for agent-driven delivery: the living architecture reference lives
in `docs/`, every product capability has a dedicated specification, and
`AGENTS.md` requires the documentation to stay aligned with implementation.

Treat this as an evolved starting point, not a frozen or verbatim copy. Adapt
the architecture, agent guidance, and product-specification templates to the
needs of each project.

## Repository guide

- [`docs/ARCHITECTURE.md`](docs/ARCHITECTURE.md) is the living architecture
  reference.
- [`docs/product-specs/`](docs/product-specs/) holds product specifications.
- [`AGENTS.md`](AGENTS.md) defines the required workflow for agents working in
  this repository.

This repository intentionally does not contain a quick-start guide. Add
runnable setup documentation only when the application stack has been chosen.
