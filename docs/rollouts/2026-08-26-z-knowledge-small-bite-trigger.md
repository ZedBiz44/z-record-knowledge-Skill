# Z-Knowledge Small Bite Trigger Rollout

Date: 2026-08-26 | Agent: Cody | Status: Partial Fleet Complete

## Change

Replaced the conflicting prohibition against calling `z-small-bite-task` with this exact rule:

> For Z-Knowledge research, load `z-small-bite-task`, but use only the minimum number of meaningful bites needed for safe completion.

The rule makes Small Bite explicit for Z-Knowledge research while preventing unnecessary fragmentation of ordinary work.

## Source And Validation

- Authoritative repository: `ZedBiz44/z-record-knowledge-Skill`
- Source pull request: `#2`
- Merged commit: `520643183e7c0f742ea6b4b3a8ede41bc4895620`
- Deployable package rebuilt successfully.
- Structural validation passed.
- Default package-build regression passed using the bundled Codex Python runtime.
- Source and generated package contain the exact same new sentence.
- The obsolete `Do not call z-small-bite-task` instruction is absent.

## Pilot

- Pilot agent: Inga on VPS1.
- Backed up the installed skill before modification.
- Patched only the conflicting sentence so unrelated live skill content was preserved.
- Restarted Inga through her private 1Password-aware wrapper.
- Verified gateway-ready, Discord and Telegram startup, zero restarts, and zero OOM state.
- Verified both `z-record-knowledge` and `z-small-bite-task` are eligible and ready.

## Completed Runtime Rollout

- VPS1: Amanda, Edith, Gohzed, Grogar, Inga, Maggie, Marsha, Terry, Victor, Vivian, and Wilma.
- VPS2: Frank, Harry, and Suzy.
- Every changed runtime file has a timestamped `SKILL.md.bak-small-bite-*` rollback copy.
- VPS1 agents were restarted sequentially and reached gateway-ready before the next agent was changed.
- VPS2 services were restarted sequentially and returned active with both skills eligible.
- Wilma used her protected `.env.resolved` startup fallback because her separate LightningWP vault item remains missing.

## Held Back By Dependency Boundary

- Ruby on VPS3/Hermes was not changed because `z-small-bite-task` is not installed or enabled there.
- Rocky on VPS4/OpenClaw was not changed because `z-small-bite-task` is not installed or eligible there.
- Installing a new skill on those platforms is a separate capability rollout and was not inferred from this wording change.

## Rollback

- Restore the newest `SKILL.md.bak-small-bite-*` file for the affected agent.
- Restart through the platform's normal protected startup path.
- Verify `z-record-knowledge` discovery, communication-channel startup, and service health.

## Remaining Behavioral Proof

- The installed instruction and skill discovery are verified.
- Confirm real Small Bite activation and the minimum-meaningful-bites behavior during the next natural Z-Knowledge research assignment; no artificial durable record was created solely for testing.
