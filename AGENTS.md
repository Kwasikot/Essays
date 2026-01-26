# Repository Guidelines

## Project Structure & Module Organization
- `en/`: English papers grouped by topic (e.g., `postcapitalism/`, `sf/`).
- `ru/`: Russian papers/translations, mirroring `en/` where possible.
- `images/`: Shared assets referenced from documents via relative paths.
- File format: Markdown (`.md` or `.MD`), UTF-8. Prefer `.md` for new files.

## Build, Test, and Development Commands
- No build step required; open Markdown in your editor/preview.
- Helpful checks (optional, if installed):
  - `markdownlint "**/*.md"` — style and basic structure checks.
  - `prettier --write "**/*.md"` — consistent formatting.
  - `rg -n "\[(.*?)\]\((.*?)\)" en ru` — list inline links to verify.

## Coding Style & Naming Conventions
- Headings: ATX style (`#`, `##`, `###`); one `#` title per file.
- Tone: clear, neutral, and concise; avoid jargon where possible.
- Filenames: lowercase, hyphen- or snake-case (e.g., `seeders_of_resilience.md`). Avoid spaces in new files.
- Images: store in `images/`; use descriptive, lowercase names (e.g., `technetic-graph.png`).
- Links: use relative paths (e.g., `../images/technetic-graph.png`).
- Language layout: add English under `en/<topic>/...`, Russian under `ru/<topic>/...`; keep parallel structure when feasible.

## Testing Guidelines
- Verify that images render and links resolve in preview.
- Keep lines reasonably short (~100 chars) and use lists/tables for readability when needed.
- Run optional checks: `markdownlint` and/or `prettier` before submitting.

## Commit & Pull Request Guidelines
- Commits: short, imperative subject; mention scope when helpful.
  - Examples: `Update en/seeders_of_resilience/Time_capsule_ideas.md`, `Add ru/sf/Artefacts-of-the-ancients.md`
- Group related edits per topic/folder; avoid drive-by unrelated changes.
- Pull Requests: include a clear description, list of affected files, before/after notes or screenshots if layout is relevant, and link any related issues.

## Agent-Specific Instructions
- Do not rename or relocate existing files unless explicitly requested.
- Follow the structure above for any additions; prefer `.md`, lowercase filenames, and relative asset links.
- Avoid introducing new tooling or CI without prior discussion.
