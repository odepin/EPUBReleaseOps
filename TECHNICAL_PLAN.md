# EPUBReleaseOps - technical plan

**Planning document, not an implementation report.**

## Product objective

An orchestration and release-evidence workflow built around established validators, not another EPUB syntax validator.

## Intended system boundary

- **Input:** Original or freely licensed EPUB demonstration content only.
- **Processing stages:** EPUB metadata reader; External validator adapters with version capture; Release manifest/status model; CLI and report writer.
- **Output:** A local sample release produces versioned, reproducible validation evidence.
- **Runtime / build stack (tentative):** Python 3.12+, Typer, lxml, subprocess adapters, pytest
- **Explicitly excluded:** Redistribution of copyrighted book text, claims of complete accessibility certification, or uploading customer manuscripts.

## Functional modules

- Validate EPUB packaging structure before invoking external tools
- Run installed EPUBCheck and optionally Ace by DAISY where configured
- Compare metadata and language settings across local variants
- Track manual QA checkpoints and issue remediation status
- Generate release manifests and deterministic check summaries

## Demonstration and acceptance cases

**Test 1:** Check a public-domain sample ebook and capture validator version

**Test 2:** Compare two synthetic publication variants

**Test 3:** Generate a release checklist with unresolved manual checks

## Safety, privacy, and provenance

1. Keep example datasets fictional, self-created, or appropriately licensed.
2. Run locally for the initial prototype; do not collect data on actual third parties.
3. Document origin and versions of external specifications and dependencies.
4. Exclude production credentials; put environment variable *names* only in `.env.example` if required later.
5. Do not make certification, legal compliance, professional safety, or performance guarantees without independent validation.

## Engineering unknowns and constraints

Respect third-party validator licenses and avoid bundling proprietary publications.

## Release definition

A first release requires a runnable prototype, verified README instructions, automated tests tied to the three demonstrations, the full LICENSE file, and an honest public GitHub development history. The roadmap estimates are hypotheses until reviewed during implementation.
