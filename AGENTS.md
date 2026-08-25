# RateDue Website — Agent Instructions

## Scope and fail-closed rule

This repository is the local static source for the RateDue product website. It
is not evidence that any GitHub, hosting, DNS, certificate, redirect,
public-content, Apple, account, submission, or release state changed.

Nothing is committed, pushed, deployed, published, or represented as current
public evidence unless every applicable gate has current `PASS` evidence.
Missing, stale, conflicting, or `UNKNOWN` evidence keeps the action `BLOCKED`.

## Governing identity contract

- `RateDue` is the product name; the D-016 migration is not a product rename.
- Ashraya Studio is not approved as provider, operator, seller, or owner.
- The exact privacy-policy controller sentence is an approved, required
  exception to the default omission of the founder's legal name. It may appear
  once in `privacy/index.html` and nowhere else in the website source.
- The `ashrayastudio` GitHub owner, repository URL, `ashraya.ai` contact-domain,
  and other established identifiers are technical/contact infrastructure, not
  public legal-operator evidence.
- Prefer product-led or role-based wording and omit personal-name copyright
  footers.

The central governing source is
`/Users/hermes/Developer/personal-digital-products-ops`, especially D-016,
D-035, D-040, and D-041 in `docs/DECISION-LOG.md`,
`docs/COMMIT-EXECUTION-PLAN.md`, `docs/CURRENT-STATE.md`, and
`docs/PUBLIC-SURFACE-CORRECTION-PLAN.md`.

## Responsibility routing

- Codex owns exactly authorized local source/docs edits, local validators,
  diffs, and read-only local Git inspection.
- Hermes is the designated and exclusive operator for every GitHub network
  operation for `ashrayastudio/ratedue` at
  `https://github.com/ashrayastudio/ratedue`.
- For ordinary Git data, Hermes must use the existing authenticated Git HTTPS
  path through `/Users/hermes/.local/bin/hermes -z`; Codex must not fall back
  to direct `gh`, API, browser, SSH, or networked Git.
- Every Hermes request must name the exact repository/URL, Git HTTPS transport,
  read-only or mutation class, exact permitted operation, prohibited
  operations, and required sanitized before/after evidence.
- The founder alone authorizes commits, GitHub mutations, deployment,
  publication, DNS/hosting/certificate/redirect changes, Apple/account work,
  legal attestations, submission, and release. Hermes supplies operation, not
  authorization.

## Local validation and mutation boundaries

Run both before proposing a commit:

```text
python3 -B scripts/validate_site.py
python3 -B scripts/validate_site.py --self-test
```

Also require a reviewed exact diff, `git diff --check HEAD`, a clean index, a
scoped sensitive-pattern scan, and preservation of unrelated owner work. Local
source, a Git commit, a Hermes push, hosting configuration, and the published
result are separate states and require separate evidence and authority. Never
access protected credential/configuration paths or place credentials,
protected contact values, financial records, or account secrets here.
