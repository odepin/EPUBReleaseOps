# EPUBReleaseOps

> Reproducible release QA for openly licensed EPUB samples.

**Current state:** Documentation starter / proposed product. The presence of this README does **not** mean the software has been implemented, deployed, used. Update this status to reflect real work.

## What it is

EPUBReleaseOps is a proposed specialist software tool for Independent publishers and ebook production freelancers. Release teams must coordinate validation, metadata checks, manual QA, and reproducible results across multiple ebook variants. The intended differentiation is: An orchestration and release-evidence workflow built around established validators, not another EPUB syntax validator.

## Intended users and use cases

- Check a public-domain sample ebook and capture validator version
- Compare two synthetic publication variants
- Generate a release checklist with unresolved manual checks

## Planned features

- Validate EPUB packaging structure before invoking external tools
- Run installed EPUBCheck and optionally Ace by DAISY where configured
- Compare metadata and language settings across local variants
- Track manual QA checkpoints and issue remediation status
- Generate release manifests and deterministic check summaries

## Proposed technology

Python 3.12+, Typer, lxml, subprocess adapters, pytest

These technologies are *planned*, not a claim that dependencies have already been installed or code has been written. Revise this section when actual implementation decisions are made.

## Proposed architecture

- EPUB metadata reader
- External validator adapters with version capture
- Release manifest/status model
- CLI and report writer

See [TECHNICAL_PLAN.md](TECHNICAL_PLAN.md) for technical boundaries and acceptance tests.

## Running locally

**Not yet runnable.** This package contains documentation templates, not software. When a functioning implementation is available, replace this paragraph with tested prerequisites, install instructions, a verified executable command, and a reproducible example using `Original or freely licensed EPUB demonstration content only.`

## Data boundaries and exclusions

Redistribution of copyrighted book text, claims of complete accessibility certification, or uploading customer manuscripts. All public examples should use Original or freely licensed EPUB demonstration content only.

## Known limitations / validation risks

Respect third-party validator licenses and avoid bundling proprietary publications.

## Development roadmap

Work is broken into estimated, not-yet-completed milestones in [ROADMAP.md](ROADMAP.md). They are *planning estimates*, not an assertion that development has begun or that work will definitely be performed.

## Business direction

Potential commercial extensions: Studio batch workflow extensions and publishing integrations.

## Contributing and licensing

License: [Mozilla Public License 2.0](LICENSE) (`MPL-2.0`). The distribution contains the complete license text. Any future source files can include the SPDX identifier `MPL-2.0` and the Exhibit A notice where appropriate. Rights in contributions and project ownership must be verified before licensing.

