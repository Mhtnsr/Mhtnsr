Use MIT for personally authored code and documentation; include the full LICENSE in every repo. Do not license employer-owned work or third-party assets as your own.

Recommended structure:
README.md
LICENSE
SECURITY.md
.gitignore
scripts/          implementation
tests/            deterministic checks
examples/         synthetic inputs and clearly labeled sample output
docs/             design, decisions, and limitations
templates/        incident/change/lab records
evidence/         sanitized, real proof only
reports/          ignored local output
data/private/     ignored real input; preferably never place it in the repo

Commit convention:
feat: add disabled-account provisioning plan
fix: reject duplicate usernames before planning
test: cover failed DNS resolution
docs: record actual client-join verification
chore: update repository metadata

One meaningful change per commit. Explain the reason when it is not obvious. Never backdate, create empty commits, or split trivial lines just to inflate activity.

Topic strategy: 4–8 precise lowercase hyphenated topics. Include the domain (identity-management), implementation (powershell/python), and purpose (troubleshooting/sysadmin). Avoid irrelevant popular topics and certification claims. Topics describe contents, not mastery. See repo-metadata.json for all six sets.


# [Project title]

[One sentence: who it helps and what it does.]

## Problem
[Concrete trigger, affected task, and why existing manual work is difficult.]

## Solution
[Implemented behavior. Separate implemented, designed, and planned features.]

## Requirements
[OS, versions, modules, permissions, inputs, and authorized scope.]

## Usage
[Exact command from repository root, using synthetic input and dry-run first.]

## Validation
[Checks actually run, observed outcome, environment, and limitations.]

## Screenshots
[Add sanitized real screenshot and caption after running. No invented evidence.]

## Recovery / escalation
[Reversal steps, irreversible effects, and when to stop or hand off.]

## Security
[Data collected, outbound requests, privileges, and what must remain private.]

## License
MIT — see LICENSE. Include third-party attribution separately.
