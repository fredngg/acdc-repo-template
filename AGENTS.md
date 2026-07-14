# Agent Operating Guide

## Purpose

This repository is documentation-first. Its primary source of truth for the
system's structure and technical decisions is `docs/ARCHITECTURE.md`.

## Required workflow

Before making a change, agents must:

1. Read `docs/ARCHITECTURE.md`.
2. Read the relevant file in `docs/product-specs/` when the change relates to
   a product capability.
3. Keep code, product specifications, and architecture documentation aligned.

After making a change, agents must update `docs/ARCHITECTURE.md` when it
affects any of the following:

- project structure or ownership boundaries;
- component responsibilities, interfaces, or data flow;
- data stores, external integrations, deployment, or security;
- notable technical decisions or the roadmap.

## Documentation conventions

- Keep `docs/ARCHITECTURE.md` concrete and current. Replace placeholders as
  soon as an implementation decision is made.
- Put one product capability or initiative in each file under
  `docs/product-specs/`, using `docs/product-specs/_template.md`.
- Use relative Markdown links between architecture and product specifications.
- Do not add a quick-start guide to the README. Add setup instructions later
  only when the project has runnable software, preferably in `docs/`.

## Change quality

- Prefer small, cohesive changes.
- Do not commit credentials, secrets, generated files, or local environment
  configuration.
- When implementation begins, add focused automated tests alongside the
  affected component.
