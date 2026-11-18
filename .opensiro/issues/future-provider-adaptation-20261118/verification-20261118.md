# Gas City S4 roadmap — final source-native engineering verdict

**Date:** 2026-11-18 · **Result:** `NO_USEFUL_CHANGE` for adding a **new Gas City SDK/core S4 future-provider adaptation constructor**. This is a scoped engineering decision, **not** an accepted VSM grade or a claim that existing Gas City already provides an autonomous S4 closed loop. The earlier `NEEDS_EVIDENCE` was a hypothesis stage; this is its final adjudication.

**Original:** [gastownhall/gascity @ `03f6fe825cf0a54c677c241e4aaa7e76dade28a5`](https://github.com/gastownhall/gascity/commit/03f6fe825cf0a54c677c241e4aaa7e76dade28a5). Initial case pin [`208a43158ccd33a8f1e066d80daf65c9f3bea713`](https://github.com/gastownhall/gascity/commit/208a43158ccd33a8f1e066d80daf65c9f3bea713); [one intervening commit](https://github.com/gastownhall/gascity/compare/208a43158ccd33a8f1e066d80daf65c9f3bea713...03f6fe825cf0a54c677c241e4aaa7e76dade28a5) modifies orphan cleanup and related session tests, not the model aliases, order interface, config editor or proposed future S4 mechanism.  
**Index:** [canonical current `5f6ea0c777733813ca42e3f210390a719488dcfb`](https://github.com/opensiro/vsm-harness-index/commit/5f6ea0c777733813ca42e3f210390a719488dcfb); no accepted Gas City assessment identified. **S1/S2/S3/S3*/S4/S5 = NOT_ASSESSED**, never inherit Gas Town's assessment.

## 1. Evidence and the alternative to a new SDK controller

| Gate | First-party evidence | Decision |
| --- | --- | --- |
| Developer-configurable actors | [Gas City architecture](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/docs/getting-started/how-gas-city-works.md): packs, agents, formulas, durable beads, events; no hard-coded roles | Already a first-party composition substrate |
| Prospective checks | [Orders tutorial](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/docs/tutorials/07-orders.md) documents conditional, cron and event triggers, with an agent-driven **formula** or a controller-side **exec**; event dispatch is at least once | No new generic scheduler or policy loop justified |
| Future provider/config choice | [Root/rig provider patches](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/docs/guides/gastown-config-recipes.md), [pack runtime registry](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/cmd/gc/runtime_registry.go), [atomic editor](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/internal/configedit/configedit.go) | Basic option/config transport already exists; not automatic S4 authorization |
| Real effect and feedback | [Config reload](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/cmd/gc/cmd_reload.go) returns `applied/no_change/accepted/failed/busy/timeout`; [revision publication](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/cmd/gc/city_runtime_config_publication.go) rejects superseded controller snapshots; [events](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/engdocs/architecture/event-bus.md) are best effort on some paths | Neither reload success nor event receipt proves a later task succeeded; **complete S4=C unproven** |
| Concrete issues | Original [#8419](https://github.com/gastownhall/gascity/issues/8419) stale model aliases; [#8367](https://github.com/gastownhall/gascity/issues/8367) Sonnet pricing gap. Current [model aliases](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/internal/worker/builtin/profiles.go) still resolve bare `opus` to `claude-opus-4-8`, while pricing includes newer models | These are real *narrower* first-party repairs with their own original Issues, not evidence demanding a prospective S4 SDK |
| Adjacent work | [#19 quota rotation](https://github.com/gastownhall/gascity/issues/19), [#2075 provider packs](https://github.com/gastownhall/gascity/issues/2075), [#9006 runtime protocol gaps](https://github.com/gastownhall/gascity/issues/9006) OPEN; [PR #8693 standby](https://github.com/gastownhall/gascity/pull/8693) and [PR #2718 runtime identity](https://github.com/gastownhall/gascity/pull/2718) OPEN/UNMERGED | Existing scopes must not be duplicated or counted as shipped |
| Maintainer priorities | [Original ROADMAP.md](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/ROADMAP.md) lists 1.6 reconciliation reliability, performance and contributor onboarding. [#8370](https://github.com/gastownhall/gascity/issues/8370) was deferred pending a concrete eligible real-world use case | Broad prospective controller has no grounded maintainer/user urgency |

The current product code includes a config editor with an *in-process mutex and validation*, not an independently proved cross-process CAS or a permission grant to an LLM. An order with `exec` runs under the controller's execution context; that must **not** be confused with a least-privilege autonomous future-policy actor. Safety/feedback for the five-link S4 hypothesis remains untested.

## 2. End-to-end sufficiency question — falsified need for a NEW CORE primitive, not S4 itself

The old P0 assumed a new SDK-level future provider controller was required to achieve:
**externally verified upcoming change → bounded permitted alternatives → independently developer-composed choice → protected configuration for eligible later sessions → actual later-session feedback to current management.**

A generic adapter may still need a domain pack; this case has **no source-pinned real consumer or native failed run that demonstrates a missing core port**. Existing pack/order/formula/config composition is the first adequate implementation candidate. Current incident and pricing Issues are not proof of an unmet *future* environment choice. Therefore adding a new core SDK controller has **no justified incremental user capability** in this case.

This is a **burden-of-proof rejection** of the proposed *new SDK feature*, not evidence that Gas City has attained `S4=C`, that all prospective provider migration is solved, or that S4 is irrelevant.

## 3. Final priority and work decision

- **P0: REJECT** new generic SDK S4 constructor, automatic future-provider manager, new event scheduler or special hard-coded VSM role. **Result: NO_USEFUL_CHANGE** for this proposal.
- **P1:** route concrete alias, pricing, quota and provider issues through **existing original GitHub issues/PRs**. Only on a *new real prospective user case* try the smallest authorized native pack/order/formula solution; do not claim it implemented or demand SDK changes now.
- **P2: NONE.** Do not create speculative S3/S5 autonomy or policy ownership.

**Reopen gate (all needed):** (1) named user plus verifiable future model/provider disturbance and at least two lawful compatible choices; (2) supported first-party native baseline or prototype demonstrably failing a defined user task; (3) precisely identified smallest missing SDK port with rights, concurrency and future-session constraints; (4) passing supported-mode positive/negative acceptance including `hold`, absent actor, revoked permission, stale revision, active worker and actual later task feedback; (5) meaningful full-life cost or operational advantage vs manual/config/pack alternative.

## 4. Execution, provenance, publication

**Source review:** completed with pinned current original main and original issue/PR status checks.  
**Actual native test / provider migration:** NOT_RUN. A release-binary smoke attempt failed at the SSH/tool execution layer before executing Gas City; that is no product test outcome.  
**Measured costs:** NOT_MEASURED.  
**Index acceptance:** NOT_AVAILABLE; formal six-grade assignment requires an independent Index process. The standard Upstream receipt validator is expected to reject the missing real accepted assessment SHA/ref/date rather than accept fabricated values.  
**Original/fork product changes:** NONE; no original Issue, PR, comment, or public fork Issue.  
**Next action:** no new SDK S4 work or new public feature request for this rejected abstraction. Only independently justified original-native fixes or a newly scoped prospective case may proceed under their own authority gates.
