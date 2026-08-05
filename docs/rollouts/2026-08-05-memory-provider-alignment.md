# Memory Provider And Z-Knowledge Fleet Alignment — 2026-08-05

Date: 2026-08-05 MDT  
Agent: Cody  
Status: Complete and verified

## Scope

Integrated external-provider and standard agent memory behavior into the universal `z-record-knowledge` process, aligned the related skill family, reconciled live agent instructions, and verified behavior across VPS1–VPS4.

## Universal Rules Implemented

- Use the agent's active memory provider.
- Follow the organization's provider inventory for assignments and sharing rules.
- Treat provider recall as supporting context.
- Verify information before durable publication.
- Store a compact pointer back to the authoritative record.
- Review-only, investigation-only, diagnostic, and draft-only work does not authorize durable publication or memory writeback.
- Historical gaps are recorded; directly relevant authorized items may be backfilled; broader cleanup goes to a controlled review backlog.

## Skill Repositories

- `z-record-knowledge-Skill`: memory-awareness rules and `references/memory-layer-routing.md`.
- `z-knowledge-routing-Skill`: owning subject selects the system of record; provider/source type does not.
- `z-wiki-research-Skill`: provider recall must be verified before promotion.
- `z-notion-knowledge-publish-Skill`: raw provider dumps prohibited; useful provenance and authoritative links required.

Relevant commits:

- `z-record-knowledge-Skill`: `d3d84d2`, `f00a9c7`, `4476515`, `32acd82`
- `z-knowledge-routing-Skill`: `18245eb`
- `z-wiki-research-Skill`: `e04cca9`
- `z-notion-knowledge-publish-Skill`: `3548d6f`

All four skills passed the Z skill validator and generic skill validator.

## Live Provider Assignment Verification

- Mem0: Terry, Edith, Harry
- LanceDB: Amanda, Vivian, Victor, Wilma
- Hindsight `zedbiz-shared`: Marsha, Maggie, Frank, Ruby
- Hindsight `internet-marketing`: Inga, Suzy
- Hindsight `ghl`: GohZed, Grogar
- Hindsight dynamic `rocky-vps4` banks: Rocky

## Fleet Rollout

- VPS1 OpenClaw: Terry, Edith, Marsha, Maggie, Amanda, Vivian, Victor, Wilma, Inga, GohZed, Grogar
- VPS2 OpenClaw: Frank, Harry, Suzy
- VPS3 Hermes: Ruby
- VPS4 OpenClaw: Rocky

The four standardized skills were deployed to each applicable live runtime. Core `AGENTS.md` instructions were aligned without replacing agent-specific provider, privacy, or source-of-truth rules.

The old automatic historical-backfill sentence was removed. Forced activity-memory wording was made conditional on authorization.

Rocky-specific corrections:

- Added missing `MEMORY.md`, `DREAMS.md`, and `memory/`.
- Verified OpenClaw `2026.7.1-2`.
- Verified Hindsight OpenClaw integration `0.10.0`.
- Retired obsolete `zedbiz-knowledge-routing` and `zedbiz-wiki-research` directories to a recoverable backup outside the active skill path.

Ruby-specific handling:

- Kept Hermes-native layout: `AGENTS.md`, `SOUL.md`, and `/opt/data/memories/`.
- Verified Hermes `0.20.0`.
- Deployed the four skills into `/opt/data/skills/` with Hermes ownership.

## Behavior Tests

Review-only boundary tests passed for:

- Edith — Mem0
- Amanda — LanceDB
- Marsha — Hindsight
- Harry — Mem0
- Frank — Hindsight
- Suzy — Hindsight
- Ruby — Hindsight through Hermes
- Rocky — Hindsight through OpenClaw

Every tested agent correctly stated that:

- Recall is supporting context, not authority.
- Important facts require verification before durable publication.
- Review-only work authorizes no provider or local-memory write.
- An authorized durable update receives only a compact pointer to the authoritative record.

## Notion Records

Updated:

- OpenClaw-Agent-Memory-Concepts
- External-Memory-Providers
- Z-Knowledge-Skills-Memory-Providers
- Memory-Integration-Testing-Executive-Summary
- 2026-08-05 Cody Daily Journal

The stale provider-comparison essay was removed from the live assignment inventory, and Rocky's provider record was updated from the stale `0.9.0` note to verified `0.10.0`.

## Follow-Up

Review the controlled-backfill rule after practical use. The possible overnight gap check and Asana review-task workflow remains a future design idea and was not enabled by this rollout.
