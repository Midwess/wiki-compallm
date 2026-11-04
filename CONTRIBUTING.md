# Working on Compallm

## Documentation

Change specifications through pull requests in `Midwess/wiki-compallm`. Read the relevant ADR and focused pages before proposing a change. Keep unresolved business rules explicit and record accepted decisions in place. Application changes that alter behavior or architecture must reference the documentation change before implementation.

Use ordinary relative Markdown links. Keep architecture and focused pages organized directly by feature under `docs/content/`. Keep each ADR below six minutes: estimate prose at 200 words per minute and allow at least 30 seconds per diagram. Aim for 500–800 words or fewer. Document behavior, architecture, security, and configuration; keep visual specifications in design assets and component code.

The generated `docs/content/api/` pages must come from Rust/OpenAPI in `Midwess/compallm`. Until automated publication is configured, regenerate them there and submit the generated output here in a documentation PR. Do not manually change generated contracts.

## Issues and decisions

Use the issue forms for features, tasks, bugs, and decisions requiring an answer. Give each task a concrete outcome and acceptance criteria. Link its specification and relevant parent feature. Use GitHub sub-issues for independently assignable work and issue dependencies for blocking work. Use checkboxes for small steps within one task.

Use Discussions for open-ended questions. Once a discussion produces actionable work, create an issue and link back. Record accepted architecture and business rules in the feature documentation rather than leaving them only in comments.

## Project fields

The [Compallm Project](https://github.com/orgs/Midwess/projects/7) displays the same issues as this repository. Issue forms automatically select this Project when the author has write access to it. Issues created through other paths must be added through the Project selector until repository-wide auto-add is configured. Status belongs in the Project; labels classify work rather than duplicating status. Priority is P0 (urgent), P1 (high), P2 (normal), or P3 (low). Feature identifies the product area. Only assign target dates when agreed.

Move work through Backlog, Ready, In progress, In review, and Done. Use Needs decision for work awaiting a business or architectural answer. A feature is complete only when its acceptance criteria are met, not merely when one sub-issue is closed.

## Linking implementation PRs

In the application PR description, use `Closes Midwess/wiki-compallm#TASK_NUMBER` for a task that the PR completes. The PR must target the application repository’s default branch for keyword linking and automatic closure. A mention in a PR comment does not establish a closing link.

Use `Related to Midwess/wiki-compallm#FEATURE_NUMBER` for broader context without closing the feature. If linking manually across repositories, open the issue’s Development sidebar, select `Midwess/compallm`, and select the PR. Do not create a duplicate application issue merely to link a PR.

Repository permissions still apply: Project access alone does not grant access to a repository’s content.
