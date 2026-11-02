# Security and evidence handling

This is a personal portfolio, not an employer system or an approved production tool.
Use an authorized lab and review changes before execution.

Never commit real company/customer data, ticket exports, passwords, tokens, API keys,
private keys, tenant/subscription IDs, internal hostnames/IPs, serial numbers, QR codes,
or screenshots containing names, notifications, account identifiers, or browser tabs.
Use fictional identities, example.invalid domains, and documentation-only addresses.
Private lab addressing can be explained abstractly; do not copy an employer's topology.

Before publishing: inspect git diff --cached, search for identifiers and secrets,
crop screenshots, replace identifying values with synthetic values, remove metadata,
and inspect the rendered files. Blurring alone can leave readable context; opaque
redaction or newly generated synthetic evidence is preferable.

.gitignore is not a security boundary and does not remove tracked files or history.
If a secret is exposed: revoke/rotate it first, remove it from current files and history
with the repository owner's approved process, and check downstream copies and logs.
Do not paste the secret into an issue while reporting it.

Report a suspected secret exposure privately through the owner's LinkedIn contact.
No vulnerability response SLA is promised for these learning projects.

Sanitization workflow:
1. Start from synthetic data instead of editing an employer export.
2. Parameterize host/domain/path/OU inputs; default to plan-only or read-only.
3. Never embed credentials; use approved runtime authentication in private labs.
4. Validate inputs, limit targets, use WhatIf/confirmation where mutations exist.
5. Test rejected inputs and failure behavior before a live lab run.
6. Review staged diffs and all rendered screenshots; run an approved secret scanner.
7. Keep command output local until it is reviewed; do not upload raw logs automatically.
8. Describe sample output as synthetic; preserve upstream code licenses and sources.
