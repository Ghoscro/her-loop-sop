# Her LOOP-SOP

A tiny operating loop for AI agents that need to keep long tasks aligned, verifiable, and safe.

Created by **Micker / Ghoscro** for **HerLove**, as part of the **Micker Method** for practical AI-agent workflows.

Origin product: **HerLove** ([herlove.ai](https://herlove.ai)).

**HER** means **Human intent / Evidence / Review**.

> Preserve the spark. Choose the smallest useful next action. Verify what can be verified. Let Strict-PM attack the claim, not the person.

This is a public-safe version. Examples use mock data; private memory, user data, credentials, deployment details, and full automation loops are intentionally excluded.

## Why

Long-running AI agent work often fails in the same boring ways:

- The agent starts with a good idea, then drifts.
- Progress reports get longer while evidence gets weaker.
- A dry run is accidentally described as a real result.
- The agent optimizes the visible checklist while forgetting the original goal.

Her LOOP-SOP is a one-page responsibility loop for avoiding that.

## Origin

Her LOOP-SOP comes from the Micker Method and the HerLove product lab: a practical approach to building AI-agent workflows that preserve the original spark, act in small verified slices, and use an independent critique pass before claiming completion.

The public version keeps the reusable method and templates from HerLove while excluding private memory, user data, credentials, deployment details, and full automation loops.

## The Minimal Loop

```text
Spark -> Goal -> Next Action -> Evidence -> Strict-PM -> Decision
```

| Step | Question |
| --- | --- |
| Spark | What original intent must be preserved? |
| Goal | What should this cycle actually deliver? |
| Next Action | What is the smallest useful move? |
| Evidence | What proves progress happened? |
| Strict-PM | What claim might be false, unsafe, or under-verified? |
| Decision | Stop, continue, retry, rollback, or ask? |

## Three Modes

### Spark Mode

Use for fuzzy ideas, product hunches, creative exploration, and early research.

Do not over-gate the idea. Capture the spark, name the cheapest experiment, and keep moving.

### Work Mode

Use when the direction is clear enough to produce an artifact.

Define the deliverable, create one useful slice, verify it, then decide whether another cycle is worth it.

### Guard Mode

Use for production, user data, secrets, money, public releases, irreversible actions, and external promises.

Run read-only first, prefer dry runs, define rollback, and do not claim completion without evidence.

## Copy-Paste Template

```markdown
## LOOP Cycle

Spark:
Goal:
Deliverable:
Next useful action:
Evidence:
Verification:
Strict-PM:
- Critical:
- Major:
- Minor:
Decision: stop / continue / retry / rollback / ask
Next checkpoint:
```

## Strict-PM Severity

| Level | Meaning | Action |
| --- | --- | --- |
| Critical | Completion is false, unsafe, unauthorized, or unverifiable | Block delivery |
| Major | Core goal is partially missed or evidence is weak | Continue or disclose risk |
| Minor | Clarity, polish, or reuse issue | Fix if cheap |
| Info | Useful observation | Do not block |

Strict-PM reviews the claim, not the person. Its job is to catch false green lights.

## Example

Task: prepare a public blog post from an internal workflow.

```markdown
Spark:
Share a useful agent workflow without leaking private context.

Goal:
Produce a public-safe draft.

Deliverable:
One Markdown article with a reusable template.

Next useful action:
Write the release boundary first, then draft the post.

Evidence:
Draft exists and includes a public-safe boundary sentence.

Verification:
No secrets, private memory, user data, deployment paths, or raw logs included.

Strict-PM:
- Critical: none
- Major: must replace internal names with neutral terms before publishing
- Minor: add a shorter social summary later

Decision:
Continue one polishing cycle.
```

## Public Release Guard

Before sharing any workflow, ask:

- Does this expose credentials, private memory, user data, or deployment details?
- Can someone reproduce the full private product from this?
- Are examples fake or safely abstracted?
- Does the release include a boundary sentence?
- Are only explicit files staged in Git?

Use the checklist in [`templates/public-release-checklist.md`](templates/public-release-checklist.md).

## What This Is Not

This is not a full project management framework, a prompt jailbreak, or a claim that process can replace judgment.

It is a small loop for keeping an AI agent honest across multiple turns.

## License

MIT
