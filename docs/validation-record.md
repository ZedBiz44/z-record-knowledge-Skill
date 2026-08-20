# z-record-knowledge Validation Record

**Status:** Source and static package validation passed. Target-platform pilot remains required before broader deployment.

## Tested Artifact

| Field | Value |
|---|---|
| Tested source commit | `5ac3b776fae538a811845b84a2baad120967915f` |
| Runtime artifact | `dist/z-record-knowledge/` generated from the tested source commit |
| Test date | 2026-08-17 MDT |
| Result | Passed |

## Commands and Results

- `bash -n scripts/build_package.sh scripts/test_default_package_build.sh` passed.
- `python3 -m py_compile scripts/validate_skill.py` passed.
- `bash scripts/test_default_package_build.sh` built `dist/z-record-knowledge/` and passed structural validation.
- `python3 scripts/validate_skill.py dist/z-record-knowledge` passed.
- `git diff --check` passed before commit.

## Remaining Deployment Evidence

- Run the target-platform validator when the pilot environment provides one.
- Install only the generated package on one approved pilot target.
- Record fresh-session discovery plus positive, paraphrased-positive, boundary, and negative trigger outcomes in the pilot record.
- Confirm the installed package matches the tested source commit and that the rollback procedure is executable.

## 2026-08-20 Storage-Routing Update Validation

**Status:** Source and package validation passed. Target-platform pilot remains required before broader deployment.

- Functional storage routing added to `SKILL.md`: pass
- Raw harvested documentation routed to approved source/wiki/source-archive locations rather than compact memory: pass
- Operational reuse signals added as capture-importance criteria: pass
- Support-documentation ingestion routed to `z-support-doc-ingestion` only for VPS1 shared-wiki OpenClaw assignments: pass
- VPS2, VPS3/Hermes, Rocky/VPS4, agent-local, mirrored, custom, and unfamiliar storage providers routed to `z-agent-knowledge-mapper`: pass
- `dist/z-record-knowledge/` refreshed from source: pass
- `python scripts/validate_skill.py dist/z-record-knowledge` passed using the bundled Codex Python: pass
- `git diff --check` passed: pass
- Local note: Windows desktop has no installed WSL distribution, so the Linux shell build script could not run here. The generated package was refreshed with the equivalent local copy operation and then validated.
