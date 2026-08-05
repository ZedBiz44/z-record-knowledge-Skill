# Memory Layer Routing

Use this reference when external provider recall, local agent memory, historical notes, or a memory conflict is relevant to a knowledge-record assignment.

## Roles

- **Active memory provider:** fast working recall and cross-session continuity.
- **Local agent memory:** agent-specific daily notes, curated context, and other workspace memory artifacts supported by the active platform.
- **Reviewed knowledge layer:** durable agent-facing knowledge with provenance and maintenance rules.
- **Technical source of truth:** version-controlled code, configuration, prompts, skill definitions, and technical history.
- **Operational knowledge system:** approved human-facing business records, decisions, plans, and summaries.

The same subject may appear in more than one layer when each copy has a distinct job. Make the authoritative location clear and use links or compact pointers instead of copying the full record.

## Recall And Verification

- Use the active provider and local memory when prior context may materially improve the assignment.
- Follow the current implementation profile for provider choice, bank or collection, sharing, privacy, write method, and verification.
- Treat recalled material as a lead. Find the originating source when practical.
- Verify time-sensitive, important, disputed, or actionable claims against the live system or the source that owns that type of fact.
- Separate verified facts from recollection, inference, uncertainty, and open questions.
- If memory conflicts with a live or reviewed source, follow the owning source and report the mismatch.

## Promotion To Durable Knowledge

- Apply the capture gates before promoting memory into a durable record.
- Do not publish raw provider dumps, full transcripts, secrets, duplicated chatter, disposable calculations, or unsupported speculation.
- Summarize and sanitize useful context. Preserve provenance when it helps a future reader verify the record.
- Route by the owning subject and requested deliverable. The provider or source format does not select the destination.
- Respect the work boundary. Recall does not authorize a durable write.

## Write Back

When the work boundary authorizes a memory write and the implementation profile requires it, store a compact continuity pointer containing only what will help future work:

- subject;
- material decision, change, or result;
- current status;
- authoritative location;
- source or responsible agent when useful;
- next action and date when relevant.

Use the active provider's real write and verification procedure. Automatic capture, configured capture, or a successful response is not proof that the memory was stored.

For review-only, investigation-only, draft-only, or equivalent work, do not write to the provider or local durable memory unless the user separately authorizes that write.

## Platform Variations

Do not hard-code an organization's agent assignments, endpoints, bank names, collection names, or version-specific commands into this universal skill. Keep them in the organization's provider inventory or platform implementation profile and verify the deployed runtime before using maintenance commands.
