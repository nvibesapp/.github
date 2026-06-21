# Contributing to nVibes

nVibes is developed with a strong focus on real human connection, privacy, trust, safety and long-term maintainability.

This guide defines the expected contribution workflow for the nVibes repositories.

---

## Core Principles

Contributions should support the nVibes mission:

- real-world human connection
- privacy and transparency
- digital sovereignty
- trust and safety
- simple, robust and maintainable architecture
- no engagement manipulation
- no needless complexity

---

## Repository Routing

Use the correct repository for the work:

```txt
nvibes-development/App             Frontend, React, Vite, PWA, UI, routing
nvibes-development/Api             Backend, NestJS, Prisma, PostgreSQL, services, controllers
nvibes-development/Feature-Request Roadmaps, sprints, backlog, completed docs, principles
nvibes-development/Infrastructure  Azure, deployment, Nginx, VMSS, operations, disaster recovery
nvibesapp/.github                  Organization profile, issue templates, PR templates, governance
```

---

## Branching

Recommended branch naming:

```txt
feature/<short-topic>
fix/<short-topic>
docs/<short-topic>
infra/<short-topic>
agent/docs/<short-topic>
agent/app/<short-topic>
agent/api/<short-topic>
```

Avoid broad mixed-purpose branches.

---

## Pull Requests

Every pull request should explain:

- goal
- affected areas
- changes
- tests and validation
- security impact
- privacy and trust-and-safety impact
- database or migration impact
- deployment impact
- documentation impact
- open follow-up tasks

Use the organization pull request template.

---

## Code Quality

Before review, check where applicable:

```txt
App:
  npm run lint
  npm run build

Api:
  npm run lint or future lint:check
  npm run test
  npm run build
  npx prisma validate / generate when schema-related
```

Do not rely on manual testing alone for security-sensitive flows.

---

## Security and Secrets

Never commit:

- production secrets
- `.env.production`
- real `.tfvars`
- private SSH keys
- local SSH-key paths
- Cloudflare origin private keys
- database passwords
- GitHub tokens
- raw personal data exports

Security-sensitive changes require explicit review.

---

## Database and Prisma

Database changes require special care.

Before merging a Prisma or database change, document:

- schema change
- migration name
- affected data
- indexes and constraints
- compatibility impact
- backup requirement
- rollback approach
- staging validation
- API and frontend impact

Production migrations must not run automatically without approval.

---

## Infrastructure

Infrastructure is production-adjacent.

Changes affecting Azure, Nginx, Cloudflare, VMSS, DB VM, API VM, AI VM, SSH, Key Vault or deployment scripts require:

- risk assessment
- rollback plan
- validation plan
- human approval
- documentation update

---

## Documentation

Feature planning documents belong in `nvibes-development/Feature-Request`:

```txt
roadmaps/   strategic feature roadmaps and target architecture
sprints/    operational sprint plans
completed/  completed implementation summaries
backlog/    early ideas, research and analysis notes
principles/ product, ethics and design principles
```

Do not create nested `docs/roadmaps/` or `docs/sprints/` paths in Feature-Request.

---

## nVibes Repository Steward

The nVibes Repository Steward may help with analysis, documentation, PR preparation and governance.

The Steward must not:

- push directly to main without explicit instruction
- perform production deployments alone
- perform production database migrations alone
- store or expose secrets
- make risky infrastructure changes without approval

---

## Review Expectations

A good PR is:

- small enough to review
- clearly scoped
- tested or manually validated
- documented where needed
- honest about risks
- aligned with nVibes product principles

Large changes should start with a roadmap or sprint plan before code.
