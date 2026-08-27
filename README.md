# Record Knowledge

This repository is the technical source of truth for `z-record-knowledge`, which determines whether lasting knowledge is justified, builds an accurate record, and routes it to an appropriate authoritative store.

## When to Use This Skill

- Create, improve, research, or store a reusable record whose value extends beyond the immediate task.
- Decide whether a fact, decision, workflow, source-backed finding, or reusable asset should be captured durably.
- Route a validated record to the right specialist skill or functional storage location.
- For Z-Knowledge work, improve or create the foundational Brief and use another Page-Type only for a different deliverable.

## When Not to Use It

- Do not use this skill for disposable chat notes, unverified claims, or a record that duplicates an existing canonical source.
- Turn raw model memory, transcripts, or private data into durable knowledge without review and sanitization.
- Publish research findings before source quality, confidence, and ownership are clear.

## Authoritative Source and Repository Contents

`SKILL.md` is the authoritative runtime guide. The repository root is the authoritative technical source, while operational SOPs or governed business records remain in their approved operational systems.

- `SKILL.md` is the authoritative runtime guide and defines the skill contract.
- `agents/openai.yaml` provides runtime discovery metadata for supported OpenAI-compatible environments.
- `references/` contains focused guidance that the runtime instructions may load when needed.
- `docs/` records implementation, pilot, validation, deployment, or operational context where applicable.
- `scripts/` contains deterministic validation and, where required, package-build helpers.

## Validation and Deployment

Run the repository validation before release or installation. Build a deployable package only when the target runtime or approved rollout requires one.

```bash
python3 <z-ai-skill-developer-root>/scripts/validate_skill.py --repository .
bash scripts/build_package.sh
python3 <z-ai-skill-developer-root>/scripts/validate_skill.py dist/z-record-knowledge
```

Validate on the actual target runtime after installation. Do not assume discovery paths, credentials, or platform behaviour without checking the live environment.

## Safety and Approval Boundaries

For Z-Knowledge work, search only approved Z-Knowledge Content databases, preserve imported or Jack-authored sources, and verify that a matching record represents the same subject and purpose. Keep secrets and private data out of inappropriate destinations, and follow required approval controls.

## Status and Contributions

Keep this README aligned with the actual skill contract and file structure. Make changes through version control, validate them before release, and document material deployment or governance decisions in the repository’s approved records.
