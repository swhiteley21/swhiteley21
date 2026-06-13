# claude-skills

Claude-ready conversions of the twelve HyperAgent skills under [`../hyperagent-public-skills`](../hyperagent-public-skills), which were cloned from [alexmcdonnell-airtable/hyperagent-public-skills](https://github.com/alexmcdonnell-airtable/hyperagent-public-skills).

The upstream files are HyperAgent platform exports and will not load in Claude as-is: they are wrapped in an export envelope and their Markdown bodies carry no YAML frontmatter. Each skill here has been restructured into the [Agent Skills](https://code.claude.com/docs/en/skills) layout that Claude Code and the Claude Agent SDK load.

## What changed in conversion

For each skill, the export envelope was stripped and the contents laid out as a skill directory:

- `SKILL.md` — YAML frontmatter (`name`, `description`) followed by the original skill body. The `description` merges the upstream `description` and `whenToUse` text so Claude can decide when to load the skill (capped at 1024 characters).
- `reference.md` — the upstream `documentation` field: full method, gotchas, and production notes.
- `scripts/` — each bundled file from the upstream `scripts` array, written out as a real file (HTML templates, Python, shell, JS).

Skill content (bodies, descriptions, scripts) is otherwise preserved verbatim, including the original em-dash punctuation and any third-party model references.

## A note on models

These skills are not wired to any LLM provider; the upstream exports carry no model field. The only mentions of "Claude" in the content refer to a design aesthetic to avoid (the "Claude look"), not to the agent. Several skills do call third-party media-generation tools (OpenAI GPT Image 2, Google Veo, Gemini) for image and video output. Those calls and their credentials are unchanged, so the skills run on Claude as the reasoning agent while still depending on those external services for generated media.

## Installing into Claude

Copy or symlink any skill directory into a location Claude scans:

- Personal (all projects): `~/.claude/skills/<skill-name>/`
- Project (this repo only): `.claude/skills/<skill-name>/`

For the Claude Agent SDK, point your skills directory at the relevant folders here. After installing, Claude loads a skill automatically when a request matches its `description`.

## Skills

| Skill | Bundled scripts |
| --- | --- |
| `airtable-kanban-work-tracker` | — |
| `brand-book-generator` | 1 |
| `briefing-trailer` | 2 |
| `business-simulation-operator-method` | 1 |
| `claymation-explainer` | 1 |
| `claymation-podcast-clips` | 3 |
| `landscaping-design-and-quote` | — |
| `muller-brockmann-grid-systems` | 2 |
| `nyc-subway-campaign` | 1 |
| `nyt-data-viz` | 6 |
| `veo-hyperframes` | — |
| `vignelli-canon-design-system` | 1 |
