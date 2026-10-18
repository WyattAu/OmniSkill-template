---
name: omni-skill-example
description: Canonical example skill validated by skillkit; copy this structure, keep the frontmatter fields exactly as documented.
allowed-tools: read, bash
license: Apache-2.0
---

## When to use

Load this skill when you need a working skeleton for a new agent skill: the
frontmatter below passes `skillkit lint` with zero findings, and the layout
(`scripts/` for executable steps, `references/` for long-form notes) is the
one the toolchain packages and verifies.

## Steps

1. Copy this directory and rename the `name` field (lowercase-hyphen, <= 64 chars).
2. Rewrite `description` — agents read it to decide when to load the skill, so
   say what it does and when, in under 1024 characters.
3. Put executable steps in `scripts/`, keep prose in `references/`.
4. Run `skillkit lint .` until it exits zero, then `skillkit pack .` and record
   the hash in your release notes.

See [references/patterns.md](references/patterns.md) for frontmatter patterns.
