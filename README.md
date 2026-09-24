# PRAHARI — Final Specification Package

## What This Is
This package is the final implementation specification for PRAHARI.

It converts the prior design discussion and Claude review into a coherent coding-agent contract.

## Files
- `AGENTS.md` — master instructions and locked decisions
- `rules.md` — binding product/privacy/safety rules
- `prd.md` — product requirements and role flows
- `architecture.md` — backend, database, security, analytics architecture
- `design.md` — UI/UX and role-specific screens
- `task.md` — implementation phases and test/demo checklist
- `MEMORY.md` — implementation history
- `README.md` — package overview

## Core Product
`DETECT → EXPLAIN → BALANCE → VERIFY`

## Roles
`PERSONNEL | WELFARE_OFFICER | COMMANDER | ADMIN | AUDITOR`

## Important Final Choice
The system is not intentionally reduced to a tiny prototype.

Instead, complexity is controlled through modular boundaries:
- API
- services
- repositories
- analytics
- security
- configuration
- tests

This means required functionality remains, while individual errors are easier to locate.

## Coding-Agent Instruction
Give the complete package to the coding agent and instruct it to:
1. read AGENTS.md first;
2. follow authority order;
3. implement in task.md order;
4. run tests after each phase;
5. never violate rules.md;
6. update MEMORY.md after meaningful work;
7. never silently remove required functionality;
8. report blockers rather than inventing requirements.

## Claude Review Incorporated
The supplied conversation highlighted:
- the strength of the operational/roster-driven framing;
- the importance of non-circular labels;
- the value of demonstrating the privacy firewall;
- Logistic Regression as the practical MVP model;
- greedy balancing as the practical MVP optimizer;
- the need to avoid over-claiming audit integrity or model validity;
- the need to separate core functionality from optional polish.

The market-positioning discussion from the conversation is retained only as positioning context in `prd.md`; it should be independently verified before being presented as a factual competitive claim.
