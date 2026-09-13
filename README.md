# Rule.js — Serializable Business Rules

A modular exploration of **serializable conditions and business-rule evaluation**.

## The engineering problem

Business rules change independently of application code. A useful rule engine needs to make those rules explicit, composable, serializable and executable—while keeping the boundary between business intent and implementation understandable.

## Modules

- `@rule.js/core` — build and evaluate conditions
- `@rule.js/elasticsearch` — translate rules into Elasticsearch queries
- `@rule.js/knex` — use conditions with Knex
- `@rule.js/contextualize` — resolve rule keys from runtime data
- `@rule.js/access-mate` — attribute-based access control
- `@rule.js/constraint` — data constraints
- `@rule.js/expression` — express business rules in a compact language

## What to study

**rule definition → serialization → contextualization → execution → downstream representation**

The interesting engineering questions are around correctness, portability, evaluation boundaries and how rule changes affect consumers.

## Portfolio positioning

This is a reusable engineering building block rather than a polished product. It complements the MountainBridge case studies around configurable workflows, business rules and platform design.

When extending it, document the decision and failure modes—not only the API surface.
