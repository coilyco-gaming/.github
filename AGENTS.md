# Agent instructions

This repository owns the `coilyco-gaming` organization profile.

## Boundaries

* Edit `profile/README.md` for the public organization landing page.
* Keep all profile and documentation content public-safe.
* Regenerate the repository pointer skill through agentic-os. Do not hand-edit
  its generated `SKILL.md`.

## Portfolio triage

* Treat every active repository in `coilyco-gaming` as one priority pool. Rank
  P0-P4 across the whole organization rather than forcing a target distribution
  inside each repository.
* Retrieve and reconcile each repository's complete open-issue set before
  ranking. Per-repository issue counts remain the coverage gate even though the
  final percentile cut is organization-wide.
* Keep executable work in the repository that owns the affected artifact.
  Labels, milestones, readiness, and dependency markers remain repo-local.
* Treat the organization-scoped P0-P4 and execution-mode labels as the live
  source of truth. Every open issue has exactly one label from each axis.
* Generate complete cross-repository views from Forgejo. Do not hand-maintain
  issue counts, issue-number inventories, priority queues, or point-in-time
  tracker snapshots in this repository.
* Use an issue in this organization-profile repository only for a time-bounded
  portfolio outcome that needs synthesis, ordering, and final closure across
  several member repositories. Link the repo-local issues instead of
  duplicating them. Do not use a standing issue as a portfolio index.

## Checkout residency

This repo is not in Agent Compose's `repository-plan.yaml`, so it has no
resident checkout under `~/projects/<owner>/`. That is intentional. Work it
from a task-scoped temporary clone, and remove that clone once the work lands.

A temporary root can be purged at any time, so commit and push before pausing,
switching tasks, or ending a session. The remote is the only durable artifact.
