# Public Release Checklist

Created by Micker / Ghoscro as part of the Micker Method.

Use this before publishing AI-agent workflows, demos, templates, or code.

## Layer

- [ ] Public: methods, templates, checklists, fake-data demos.
- [ ] Needs abstraction: remove private names, paths, data, and implementation depth.
- [ ] Internal only: too close to private operations.
- [ ] Blocked: contains high-risk material.

## High-Voltage Check

Block release if any item is present:

- [ ] API keys, tokens, cookies, passwords, SSH config, `.env`.
- [ ] Raw private memory, persona files, diaries, or internal relationship context.
- [ ] Real users, private chats, invite-code pools, orders, contact details.
- [ ] Server credentials, internal hostnames/IPs, live deployment scripts.
- [ ] Full unredacted logs, telemetry, or tool-history files.
- [ ] Anything that reproduces the complete private product loop.

## Moat Check

- [ ] The release teaches a method, not the whole business.
- [ ] Examples use fake or safely abstracted data.
- [ ] Core data, prompts, operations, and automation loops remain private.
- [ ] Publishing creates reputation, feedback, collaboration, or user trust.

## Git Check

- [ ] Use a clean export folder or clean public repo.
- [ ] Stage only explicit files.
- [ ] Inspect staged filenames and staged diff.
- [ ] Do not use `git add .` in a dirty private workspace.

## Boundary Sentence

Add this or an equivalent:

```text
This is a public-safe version. Examples use mock data; private memory, user data, credentials, deployment details, and full automation loops are intentionally excluded.
```
