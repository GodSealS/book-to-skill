@AGENTS.md

# CodeBuddy

Use `AGENTS.md` as the canonical repository instruction file. Do not duplicate repository-wide rules here.

## CodeBuddy specifics

- This repository ships as an agent skill. CodeBuddy reads it from `~/.codebuddy/skills/book-to-skill/` (personal) or `.codebuddy/skills/book-to-skill/` (project) — invoke it as `/book-to-skill <path|folder|glob> [skill-name]`.
- CodeBuddy scans only the two roots above, so generated book skills default to `~/.codebuddy/skills/<slug>/` on this host; a skill written to `~/.agents/skills/` is invisible here.
- Local CodeBuddy state (`memory/`, `settings.local.json`, session data) is gitignored; `.codebuddy/skills/`, `agents/`, `rules/`, `commands/` and `settings.json` are shareable and tracked.
