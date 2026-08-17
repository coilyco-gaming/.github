---
ward:
  workflow: merge-remote-main
---
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

## Scope

The public organization profile and shared review metadata for `coilyco-gaming`.
Nothing else belongs here.

## Project shape

`profile/README.md` is the landing page both forges render.
`.github/CODEOWNERS` and `.forgejo/CODEOWNERS` carry equivalent review ownership.

## Repo boundaries

Organization presentation and review defaults only. Project work belongs in
the repository that owns it.

## Commands

No dev verbs, so this repo ships no justfile. [`.ward/ward.yaml`](.ward/ward.yaml)
is present so ward's repocfg loader recognizes the repo.

## Validation

Run `pre-commit run --all-files` before committing. The catalog suite is
consumed by upstream ref and never forked.

## Safety

Everything here is public. Keep opaque ids, host identifiers, and credentials
out of the tree.

## Cross-repo contracts

The catalog pre-commit hooks are authored in agentic-os and consumed here by
upstream rev. Canonical development happens on Forgejo.

## Release

Commit directly to `main` and push to canonical Forgejo.

## Agent rules

Use she/her for Kai. No em dashes, italics, or semicolons in prose. Name the
actor in every action sentence.

## See also

- [README.md](README.md) - what this repository is.
- [docs/FEATURES.md](docs/FEATURES.md) - what it provides.
- [.ward/ward.yaml](.ward/ward.yaml) - catalog metadata.
