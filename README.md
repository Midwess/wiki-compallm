# Compallm workspace

Compallm helps individuals and teams use LLMs across providers, govern usage, and build shared knowledge.

This repository owns product documentation, architecture decisions, and product tasks. The [application repository](https://github.com/Midwess/compallm) owns source code and implementation pull requests.

## Documentation

- [Product overview](docs/content/overview.md)
- [Documentation index](docs/content/index.md)
- [Deployment guide](docs/content/setup-guideline.md)
- [Public API reference](docs/content/api/index.md)
- [Contribution and tracking guide](CONTRIBUTING.md)

## Work tracking

Create features, tasks, bugs, and actionable decisions in [Issues](https://github.com/Midwess/wiki-compallm/issues/new/choose). Use Discussions for open-ended exploration. The Compallm Project linked from this repository’s homepage is the shared dashboard.

Feature issues describe outcomes and link to specifications. Break implementation into sub-issues. Keep acceptance criteria and delivery updates in issues; maintain the accepted solution and unresolved business rules in the relevant feature ADR.

Application pull requests link to tasks in this repository using closing keywords in the PR description:

```text
Closes Midwess/wiki-compallm#TASK_NUMBER
```

Replace `TASK_NUMBER` with the actual issue number. GitHub establishes the closing link when the PR targets the application repository’s default branch and closes the issue when merged there. Reference a larger feature with `Related to Midwess/wiki-compallm#FEATURE_NUMBER` when the PR does not complete it.

## Documentation ownership

Maintain feature documentation under `docs/content/<feature>/`: `adr.md` owns architecture and open questions; sibling pages own focused behavior and configuration. Documentation publication does not establish feature completion.

Generated API pages remain sourced from Rust/OpenAPI in the application repository. Do not hand-edit them. Cross-repository generation and the existing documentation-site cutover are tracked as follow-up work; the application repository’s existing publication pipeline is still active.
