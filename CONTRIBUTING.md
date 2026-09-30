# Contributing to MoMo Guardian

## Branching
- `main` — always demo-ready. Protected. No direct pushes.
- `dev` — integration branch. Open PRs into `dev`; `dev` → `main` only at checkpoints.
- Feature branches: `feat/<area>-<short-desc>`, `fix/<short-desc>`, `docs/<short-desc>`, `chore/<short-desc>`
  (e.g. `feat/risk-new-recipient-signal`).

## Commits — Conventional Commits
`feat:`, `fix:`, `docs:`, `chore:`, `refactor:`, `test:`  — e.g. `feat(risk): add amount-deviation signal`.

## Pull requests
- One purpose per PR, small and reviewable (aim for < 400 changed lines).
- At least **1 approval** before merge. Author does not merge their own PR unless in emergency (note it in the PR).
- CI must pass. Link the issue (`Closes #12`).
- Squash-merge into `dev`.

## Contract-first rule
Frontend and API talk **only** through the contract in `momo-guardian-docs/02-architecture/api-contract.md`.
Need a change? Open a `docs:` PR to the contract first, tag both owners, then implement.

## Secrets
Never commit secrets, real phone numbers, or real customer data. The project uses **synthetic data only**.
