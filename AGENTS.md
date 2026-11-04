# Workspace instructions

This repository owns Compallm documentation, product issues, and decisions. Application code and implementation PRs live in `Midwess/compallm`.

Read `README.md`, `CONTRIBUTING.md`, and the relevant feature ADR and focused pages in full before changing documentation. Preserve unrelated edits. Documentation-only work does not authorize application implementation.

Organize documentation under `docs/content/<feature>/adr.md` with focused sibling pages. Describe the current solution directly and keep unresolved requirements explicit. Do not add decision dates, superseded alternatives, review histories, implementation diaries, visual specifications, central ADR folders, or development/data-privacy sections. Keep shared engineering instructions here.

Keep feature ADRs below six minutes: estimate prose at 200 words per minute plus at least 30 seconds per diagram; aim for 500–800 words or fewer. Distinguish accepted decisions, planned behavior, and implemented behavior.

Generated API pages under `docs/content/api/` are sourced from Rust/OpenAPI in the application repository. Preserve generated output and TypeScript JSDoc; do not hand-edit API pages.

File product tasks in this repository and track them in the Compallm Project. Link application PRs with `Closes Midwess/wiki-compallm#NUMBER` only when they complete that issue. Keep delivery updates in issues and durable decisions in feature documentation.
