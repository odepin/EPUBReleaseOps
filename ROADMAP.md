# EPUBReleaseOps - development roadmap

**Status:** Planned work only. None of the boxes are marked completed. Estimates are rough.

## Product-level acceptance criterion

A local sample release produces versioned, reproducible validation evidence.

## Estimated work breakdown

| Step | Milestone | Estimated hours | Observable outcome |
|---|---|---:|---|
| 1 | Implement EPUB metadata parsing | 8 | Tested package metadata extraction |
| 2 | Create subprocess validator adapters | 10 | Captured tool versions and failure handling |
| 3 | Build manifest and checkpoint engine | 9 | Machine and manual checks coexist |
| 4 | Add variant comparison | 8 | Clear metadata/asset differences |
| 5 | Implement CLI and reports | 8 | Repeatable batch release view |
| 6 | Tests and installation documentation | 10 | Sample workflow with openly licensed content |
| | **Total estimated** | **53** | |

## Detailed milestones

### 1. Implement EPUB metadata parsing (8 estimated hours)

- [ ] Deliverable: Tested package metadata extraction.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 2. Create subprocess validator adapters (10 estimated hours)

- [ ] Deliverable: Captured tool versions and failure handling.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 3. Build manifest and checkpoint engine (9 estimated hours)

- [ ] Deliverable: Machine and manual checks coexist.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 4. Add variant comparison (8 estimated hours)

- [ ] Deliverable: Clear metadata/asset differences.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 5. Implement CLI and reports (8 estimated hours)

- [ ] Deliverable: Repeatable batch release view.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 6. Tests and installation documentation (10 estimated hours)

- [ ] Deliverable: Sample workflow with openly licensed content.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

## QA and release gates

- [ ] A real runnable implementation exists, with verified setup commands in `README.md`.
- [ ] Automated tests pass in a clean environment and failures are actionable.
- [ ] Only fabricated, original, openly licensed, or otherwise authorized sample data is published.
- [ ] No passwords, API keys, secrets, customer records, or employer/client confidential artifacts appear in repository history.
- [ ] A source-linked change log and actual progress notes distinguish finished work from plans.
- [ ] The GitHub history preserves authentic work and authorship; do **not** manufacture or backdate commits.

## Parking lot and risks

- Technical: Respect third-party validator licenses and avoid bundling proprietary publications.
- Commercial hypothesis (not validated): Studio batch workflow extensions and publishing integrations.
- Beyond MVP: defer paid extensions and hosted features until the underlying product works.
