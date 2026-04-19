# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

A Claude Code **skill** (`SKILL.md`) that answers USA Softball 2026 Fast Pitch rules questions. When the skill is invoked, Claude reads the relevant `references/` markdown files and responds as an expert rules official.

There is no build system, test runner, or application code. All development is editing markdown files.

## Repository structure

- **`SKILL.md`** — The skill definition. Contains the system prompt, behavioral constraints, and the reference-file routing table (which file to read for which question type).
- **`references/`** — Structured markdown extracts of the official rulebook, one file per rule section. These are the sole source of truth for all rules answers.
- **`docs/USA Softball 1-12-2026-Rule-Book.pdf`** — The original source PDF. Use this to verify or expand reference files.

## How the skill works

Claude Code reads `SKILL.md` as a system prompt when the skill is triggered. It then reads only the `references/` files relevant to the question (per the routing table in `SKILL.md`) and answers strictly from those documents — no outside knowledge.

## Versioning

The version is tracked in `SKILL.md` frontmatter (`version` field) using two-part versioning:
- **Major version** — bump when a new year's rulebook is released (e.g. `2.0` for the 2027 rulebook)
- **Minor version** — bump for corrections or additions within the same rulebook year (e.g. `1.1`)

GitHub releases use the tag format `v1.0`, `v1.1`, `v2.0`, etc. Update the version in `SKILL.md` before tagging a release.

## Editing reference files

- Reference files must reflect the official PDF exactly. When in doubt, check `docs/USA Softball 1-12-2026-Rule-Book.pdf`.
- Each file covers one rule section. The routing table in `SKILL.md` maps question types to files — update the table if you add or rename files.
- Fast Pitch rules only. Slow Pitch / Modified Pitch variants may appear in the source PDF alongside FP rules; do not include them in the reference files unless they are needed as contrast.
- Rule citations in reference files should match the format used in answers: `Rule X, Section Y` or `Rules Supplement #N`.
