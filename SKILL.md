---
name: z-record-knowledge
description: Create, improve, research, and store reliable, durable, accurate, reusable knowledge records when lasting knowledge is justified.
---

# Record Knowledge

Create, update, summarize, condense, expand, or research information and content into reliable, durable, accurate, reusable knowledge records, then store them effectively.

This skill is source-neutral. Work from any credible material, including conversations, notes, files, databases, websites, email, documents, research, system evidence, and connected applications.

## Respect The Work Boundary

The user's requested scope controls whether durable systems may be changed.

- For `review only`, `investigate only`, `do not change anything`, `draft only`, or equivalent instructions, return findings or a draft without publishing, updating, moving, or deleting durable records.
- Read-only work may remain chat-only until publishing is requested or otherwise authorized.
- A request to create, update, organize, migrate, publish, or complete the record authorizes the ordinary record changes required for that outcome.
- If new work would materially exceed the authorized scope, stop and request direction.

Knowledge capture supports the assignment; it never expands the assignment's authority.

## Decide Whether Durable Capture Is Justified

Read `references/capture-decision.md` before creating a new record.

- Search before creating.
- Update a suitable existing record when the information materially improves it.
- Create a new record only when every new-record gate passes.
- Do not create records for acknowledgements, passing mentions, duplicated discussion, unsupported speculation, secrets, raw transient logs, or disposable intermediate work.

## Build The Record

- Identify the requested outcome, owning subject or initiative, evidence, and intended future use.
- Separate source statements, verified facts, conclusions, recommendations, uncertainty, and open questions.
- Preserve original source material when preservation is required. Put transformations or syntheses in a derivative record rather than silently rewriting the source.
- Combine related notes when one coherent record is more useful than several fragments.
- Keep distinct records when their owners, purposes, audiences, evidence standards, or lifecycles differ.
- Use the current schema, template, naming rules, and required fields of the selected destination.

## Use Memory As Supporting Context

Read `references/memory-layer-routing.md` when an active memory provider, local agent memory, historical recall, or a memory conflict is relevant.

- Use the agent's active memory provider when prior context may help the assignment.
- Follow the organization's current provider inventory for assignments, banks, collections, sharing, privacy, and write rules.
- Treat provider recall and local agent memory as supporting context, not final authority.
- Verify important or changeable information against the live system or authoritative record before durable publication.
- After meaningful work, store only a compact continuity pointer back to the authoritative record when the work boundary authorizes a memory write and the implementation profile requires it.

## Route The Record

Apply this hierarchy in order:

- The owning subject, entity, initiative, or operating context selects the database or collection.
- The requested deliverable selects the record or page type.
- The source format is evidence and does not automatically determine either destination.

Examples: research about a person normally belongs with the person; research supporting a campaign normally belongs with the campaign; a website review belongs with the website only when the website itself is the managed subject.

Load the organization's routing or publishing skill only when that specialist procedure is required. Keep destination selection separate from record-type selection.

## Apply Functional Storage Routing

Choose the storage layer by what the information must do later:

- Durable behavior rules belong in the agent's operating instructions only when they change future agent conduct. Keep them concise and stable.
- Compact long-term memory files hold durable principles, owner context, and pointers to authoritative records.
- Reviewed wiki or knowledge-base records hold structured tool knowledge, workflow facts, source-backed research, and reusable operational building blocks.
- Episodic or working memory holds tactical lessons, recent friction, short reminders, and next-action pointers.
- Technical source repositories hold code, configuration, skill source, package records, validation evidence, and technical change history.
- Human-facing operating systems hold decisions, plans, summaries, SOPs, and business records intended for people.

Raw harvested documentation, full transcripts, large research dumps, and copied manuals belong in approved source records, wiki pages, or source archives when preservation is authorized. Store only compact pointers in long-term or episodic memory.

For documentation harvests, preserve the building blocks that make future work easier: repeatable procedures, prerequisites, permissions, decision points, inputs, outputs, validation steps, failure conditions, manual fallbacks, undocumented workarounds, recurring questions, UI friction, automation opportunities, and materially useful prompts or configurations. Treat these as importance signals for durable storage, not as an automatic instruction to create a finished SOP or guide.

When a task is specifically support-documentation ingestion, use `z-support-doc-ingestion` only for a VPS1 shared-wiki OpenClaw assignment. Use `z-agent-knowledge-mapper` for VPS2, VPS3/Hermes, Rocky/VPS4, agent-local wiki setups, mirrored wiki setups, custom knowledge stores, or unfamiliar storage providers.

## Load Specialist Skills When Required

- Load `z-knowledge-routing` when the authoritative destination is unclear or more than one home is plausible.
- Load `z-code-allocation` before any governed lookup, reservation, confirmation, failure, or status check for an authoritative record code.
- Load `z-notion-knowledge-publish` before creating, moving, or materially updating a governed Notion record.
- Load `z-wiki-research` for substantial source-backed wiki research, conflicting evidence, important verification, or a durable wiki synthesis.
- Use the environment's `wiki-maintainer` when a wiki record needs technical maintenance without new research.

Do not call `z-small-bite-task` from this skill. It is independent everyday behavior that applies to large or resource-heavy work of any kind.

## Handle Historical Gaps

- Record a discovered missing or incomplete historical item as a gap.
- Backfill it during the current assignment only when it is directly relevant to the requested outcome.
- Put broader historical cleanup into a controlled backlog for review.
- Never let open-ended backfilling take over the current assignment.

## Research And Publish

- Research only to the depth needed for a reliable record and the requested outcome.
- Use authoritative, current sources when accuracy risk is high or information changes over time.
- Use the approved identifier or code-allocation workflow before publishing when the destination requires one.
- Publish through the approved destination-specific workflow.
- Create agent-facing mirrors only when the implementation profile requires them.
- Verify the stored record, required fields, links, identifiers, and any mirror before reporting completion.

## Completion

Report records created, updated, combined, reused, or deliberately not created; their authoritative locations; evidence or confidence gaps; any controlled-backlog item; and any memory pointer written and verified.

## Governance and Operational Records

The authoritative technical copy and current deployment evidence are maintained in the [ZedBiz source repository](https://github.com/ZedBiz44/z-record-knowledge-Skill). Keep implementation, security and rollback, validation, and pilot records in its `docs/` directory. Those operational records are not runtime instructions and are excluded from the generated package.
