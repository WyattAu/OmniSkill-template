# Frontmatter patterns

- `name` — lowercase letters, digits, hyphens; 1-64 chars; no leading/trailing hyphen.
- `description` — agent-facing; <= 1024 chars; no placeholders (lint warns on TODO).
- `allowed-tools` — comma-separated tool ids the skill may use; keep it minimal.
- `license` — optional SPDX id.

Unknown fields are lint **errors**: the format accepts everything otherwise,
and a format that accepts everything validates nothing.
