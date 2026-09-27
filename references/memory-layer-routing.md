# Memory Layer Routing

Use this reference when external provider recall, local agent memory, historical notes, or a memory conflict is relevant to a knowledge-record assignment.

## Roles

- **Active memory provider:** fast working recall and cross-session continuity.
- **Local agent memory:** agent-specific daily notes, curated context, and other workspace memory artifacts supported by the active platform.
- **Reviewed knowledge layer:** durable agent-facing knowledge with provenance and maintenance rules.
- **Technical source of truth:** version-controlled code, configuration, skill definitions, and technical history.
- **Operational knowledge system:** approved human-facing business records, decisions, plans, and summaries.
- **Operating instructions:** concise durable behavior rules that change future agent conduct.
- **Source archive:** approved storage for raw source captures, transcripts, and large research evidence when preservation is authorized.

The same subject may appear in more than one layer when each copy has a distinct job. Make the authoritative location clear and retain concise substantive facts with source links without copying the full record.

## Functional Routing

- Put durable execution rules in operating instructions only when the rule must guide future agent behavior.
- Put durable facts, decisions, preferences, principles, and source links in compact long-term memory.
- Put structured tool, workflow, API, UI, and troubleshooting knowledge in the reviewed wiki or knowledge base.
- Put tactical lessons, runtime friction, recent surprises, and next actions in episodic or working memory.
- Put code, configuration, skill source, validation evidence, package records, and technical history in the technical source repository.
- Put business decisions, plans, summaries, SOPs, and human-facing operating records in the operational knowledge system.

## Recall And Verification

- Use the active provider and local memory when prior context may materially improve the assignment.
- Follow the current implementation profile for provider choice, bank or collection, sharing, privacy, write method, and verification.
- Treat recalled material as a lead. Find the originating source when practical.
- Verify time-sensitive, important, disputed, or actionable claims against the live system or the source that owns that type of fact.
- Separate verified facts from recollection, inference, uncertainty, and open questions.
- If memory conflicts with a live or reviewed source, follow the owning source and report the mismatch.

## Promotion To Durable Knowledge

- Apply the capture gates before promoting memory into a durable record.
- Raw provider dumps, full transcripts, secrets, duplicated chatter, disposable calculations, and unsupported speculation are not suitable durable records.
- Raw harvested documentation belongs in approved source records, wiki pages, or source archives when preservation is authorized, not in compact memory files.
- Summarize and sanitize useful context. Preserve provenance when it helps a future reader verify the record.
- Route by the owning subject and requested deliverable. The provider or source format does not select the destination.
- Respect the work boundary. Recall does not authorize a durable write.

## Write Back

Keep the active provider's approved automatic capture or retain and automatic recall enabled when supported. Useful context from reviews, research, audits, diagnosis, planning, and ordinary questions may be remembered when it can help future work.

When an explicit memory update will improve continuity, save substantive useful context containing what will help future work:

- subject;
- material decision, change, or result;
- current status;
- authoritative location;
- source or responsible agent when useful;
- next action and date when relevant.

Use the active provider's real write and verification procedure. Automatic capture may skip useful facts. Explicitly save important instructions, corrections, decisions, blockers, verified results, and handoffs. Read the saved content back through the provider before claiming it is remembered; an accepted asynchronous operation is not completed retention. Preserve the operation ID and check completion or retrieval. Before retrying an uncertain write, check whether it already succeeded.

Memory capture does not authorize publishing, modifying, moving, or deleting records in Notion, Memory Wiki, GitHub, Asana, production systems, or any other authoritative destination. Those actions remain controlled by the assignment's work boundary.

## Corrections, Continuity, And Handoffs

- Include the actual fact or decision, its reason when known, project, responsible agent, event date, status, next action, and exact source URL or identifier. A topic list or source title alone fails retention.
- Distinguish user decisions from suggestions, approved facts from review-pending material, and verified results from reported claims. Never invent missing metadata.
- Use the source identifier and subject to find an existing record. Update it when supported. Otherwise save a dated correction that identifies which prior claim is superseded; do not silently erase historical evidence.
- Keep one coherent record per subject and event. Use a stable document identifier and replace/update semantics when supported; check completion before retrying. Do not repeatedly ingest a full conversation.
- In the existing daily note, update the active assignment after meaningful changes and before handoff: objective, latest decision, completed work, next action, owner, waiting on, source, last updated. This is a section of the platform's existing daily file, not a new memory store.
- On resumption, read that daily entry directly and recall related provider history. Check date, ownership, source, and later corrections before acting. Promote lasting facts to existing curated memory; preserve daily history under the existing retention policy, without introducing deletion schedules.
- Workers return substantive results and their evidence to the main agent. The main agent saves and reads back the handoff within its own authorized scope. Do not assume worker, scheduled-job, channel, or main scopes share recall. Never widen private-memory access to make a test pass.
- If external recall or capture fails, write and read back the existing local daily entry, report the provider as degraded, and use authoritative sources when safe. Local success does not prove external success. Reconcile when the provider is restored, avoiding duplicates.
- Use provider-specific tools when generic native and external tools have ambiguous names. Identify which store returned the result; an empty native search does not prove the external bank is empty.

## Platform Variations

Do not hard-code an organization's agent assignments, endpoints, bank names, collection names, or version-specific commands into this universal skill. Keep them in the organization's provider inventory or platform implementation profile and verify the deployed runtime before using maintenance commands.

