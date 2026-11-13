# Agent instructions — Organization profile

Primary branch: `develop`. Preserve this branch policy.

## Engineering and language policy

- Communicate with the user in Portuguese unless they request another language. Write all code, identifiers, comments, commit messages, and repository documentation in English.
- Keep localized user-facing content in its locale resources; English technical naming must not remove Portuguese (Brazil) support. Preserve proper names, provider identifiers, and externally defined protocol fields.
- Read README.md, CHANGELOG.md, and applicable instructions before editing. Inspect actual code and installed versions; documentation is context, not proof of current runtime behavior.
- Apply KISS, DRY, and SOLID pragmatically. Reuse existing patterns and dependencies. Ask before introducing dependencies unless already authorized.
- Prefer Docker for development and verification. Test observable behavior and relevant failure/security boundaries. Never weaken assertions or security to make checks pass.
- Validate untrusted input and enforce authorization on the server. Never commit or print credentials, tokens, private keys, personal account data, or database backups.
- Preserve public contracts and persisted identifiers. Renaming a database, table, column, API field, or serialized identifier requires an explicit compatibility/migration plan and validation; never silently recreate or discard existing data.
- Preserve unrelated working-tree changes. Stage only task-owned files or hunks. Do not reset, force-push, rewrite shared history, or change production data without explicit authorization.
- Use Conventional Commits without unsolicited co-author attribution. Review the final diff and report checks actually performed, failures, limitations, and unfinished work.

## Documentation is part of every change

- Record every change in CHANGELOG.md under Unreleased, including fixes, documentation, operational changes, and verification/known limitations where relevant. Do not invent release dates or claim unfinished work is released.
- Update README.md whenever setup, configuration, behavior, public contracts, architecture, or operational guidance changes.
- Review and update AGENTS.md whenever agent instructions, repository conventions, tooling, constraints, or project context changes. Do not add meaningless edits when the instructions remain accurate.
- Keep all three files in English and consistent with each other and the code. Clearly separate implemented behavior from approved direction and future proposals.

## Project-specific requirements

- Keep the public profile concise and in English. Preserve existing brand assets and link destinations unless the task changes them.
- Use DynatriSoft Studios / DynatriSoft and the exact legal company name. Keep sensitive/private implementation details out of public profile content.
- Check relative/raw image links after branch changes. Validate static Markdown/SVG; do not introduce an application build or dependencies for this repository.
