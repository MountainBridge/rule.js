# Rule.js — Business Rules Engine

> A historical JavaScript rules-engine repository with unusually strong potential as an engineering case study: serializable conditions, contextual data, query translation and access-control rules.

## 30-second read

The core problem is separating **business policy from application control flow** so rules can be represented, composed, serialized and evaluated consistently.

## Modules

- `@rule.js/core` — build and run conditions
- `@rule.js/elasticsearch` — translate rules into Elasticsearch queries
- `@rule.js/knex` — integrate conditions with Knex
- `@rule.js/contextualize` — substitute runtime context into conditions
- `@rule.js/access-mate` — attribute-based access control
- `@rule.js/constraint` — data constraints
- `@rule.js/expression` — business-rule expression language

## Run online

**[Open in StackBlitz](https://stackblitz.com/github/MountainBridge/rule.js)** — browser workspace for exploring the JavaScript packages.

**[Open in GitHub Codespaces](https://codespaces.new/MountainBridge/rule.js)** — recommended when working across the package workspace.

For isolated JavaScript experiments, use **[OneCompiler](https://onecompiler.com/javascript)**.

## Engineering questions

```text
Business policy
      ↓
Serializable rule
      ↓
Contextualization
      ↓
Evaluation / query translation
      ↓
Application decision
```

Key questions:

- How do we validate a rule before execution?
- How do we version serialized rules?
- Can a rule be translated consistently across storage/query engines?
- How do we prevent authorization rules from becoming ambiguous?
- What happens when context data is missing?
- How do we test rule equivalence during a migration?

## Modernization direction

This is a stronger candidate for deeper modernization than the tiny game repositories. The next step is deterministic fixtures, property-style tests, rule snapshots, failure cases and CI evidence around rule evaluation.
