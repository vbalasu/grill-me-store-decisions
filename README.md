# grill-me-store-decisions

A Claude Code skill that interviews you relentlessly about a plan or design — and *persists* the full decision tree (selected + rejected options, recommendations, and cost tradeoffs at v1 / alpha / growth scales) to `decision-tree.md` in the current repo, so you can revisit any branch weeks later without re-running the whole interview.

## What it does

For each question:
- Records the question, every option presented, the one you selected, the rationale, and a cost tradeoff (SaaS vs self-host, $/month at three scales, crossover points, engineer-time).
- Tracks dependencies between decisions and surfaces guiding principles (e.g. "minimize paid 3rd parties") prominently.
- Updates `decision-tree.md` incrementally — not just at the end.

## Install

Drop `SKILL.md` into `~/.claude/skills/grill-me-store-decisions/` and invoke with `/grill-me-store-decisions` (or let Claude pick it up from the description).

## Credit

Built on top of [`grill-me`](https://github.com/mattpocock/skills/blob/main/skills/productivity/grill-me/SKILL.md) by [Matt Pocock](https://github.com/mattpocock) — shout out for the core "interview me until we reach shared understanding" idea. This variant adds the persistence + cost-tradeoff layer.
