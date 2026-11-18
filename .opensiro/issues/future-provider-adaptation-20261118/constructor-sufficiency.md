# Gas City — conditional S4 constructor sufficiency and native validation contract

**PLAN_ONLY · NEEDS_EVIDENCE · NOT IMPLEMENTED · INDEX_BASELINE_MISSING.**  
[Human Issue](https://github.com/opensiro-contributions/gascity/blob/opensiro/meta/.opensiro/issues/future-provider-adaptation-20261118/issue.md) · [source receipt](https://github.com/opensiro-contributions/gascity/blob/opensiro/meta/.opensiro/issues/future-provider-adaptation-20261118/roadmap.md) · original [Gas City @ `208a43158ccd33a8f1e066d80daf65c9f3bea713`](https://github.com/gastownhall/gascity/commit/208a43158ccd33a8f1e066d80daf65c9f3bea713).

## Functional ownership boundary (NO accepted grades)

The canonical Index at `5f6ea0c777733813ca42e3f210390a719488dcfb` has no accepted Gas City assessment file. **S1/S2/S3/S3*/S4/S5 = NOT_ASSESSED**, not Gas Town's distinct historical `A/A/A/A/—/—`. No promotion to C, P or A occurs in this case.

**System-in-focus:** one configured, first-party Gas City deployment, its city pack, installed agents, bead store, orchestrator, orders, event bus, runtime registry, reconciliation and protected session lifecycle. External provider vendor announcements, future model availability and vendor identity systems are the *environment*, not Gas City-owned S4 actors. Third-party packs/agents are only counted when reachable through the supported first-party distribution and authorization boundary.

**S1:** configured workers execute local task steps; **S2:** orchestrator routes/serializes dependencies; **S3:** controller/reconciler manages present session status and capacity; **S3***: review gates do not automatically imply a separately proven independent audit owner; **S4:** future changes need separate perception, option selection, lawful future effect, return; **S5:** human/organizational provider and policy rights remain reserved. These are mapping hypotheses, **not classifications**.

## 1. User task, disturbance, choice and native baseline

**Actor:** a city operator maintaining multiple agents on allowed provider/model versions and a developer adding an opt-in adaptation policy pack.  
**Future disturbance:** credible upcoming deprecation or compatibility restriction, with source, effective date, model/provider, affected agents and verified compatible substitutes (not a presently failed launch).  
**Choices:** retain pending confirmation; migrate *future starts only* to an explicitly approved provider/model; hold and request operator decision.  
**Observable user outcome:** a later real session launches with the selected compatible runtime, while in-flight leased work is protected and receipts record why/how that choice was made.

**Baseline without new code:**
- [Root/rig patches](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/guides/gastown-config-recipes.md) support explicit provider overrides; `gc config` is predominantly explanatory, and durable config is file-first (see [command map](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/reference/gastown-command-map.md)).
- [Orders](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/tutorials/07-orders.md) run shell commands or model-driven formulas on events, conditions and schedules.
- [Pack-declared runtime providers](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/internal/config/pack_runtimes.go) are resolved into a city-scoped [runtime registry](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/cmd/gc/runtime_registry.go).
- [Config/reload machinery](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/cmd/gc/cmd_reload.go) and the session reconciler mediate the effect of config changes; **not** an automatic proof that a model-generated proposed edit is safe.
- [Primary maintainer roadmap](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/ROADMAP.md) does not promise this feature; prefer narrow comparison first.

**Key negative:** a manually edited provider patch + auto reload is a useful product path, but not proof a developer-composed autonomous S4 actor exists. A generic order that merely calls a hard-coded switch is also not proof of an independently constructed future S4 choice.

## 2. Shipped vs proposals / dedup

| First-party location or work | Verified position as of 2026-11-18 | What may be reused / not claimed |
| --- | --- | --- |
| [packs, formulas, orders, events](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/getting-started/how-gas-city-works.md) | SHIPPED documented primitives | Possible S4 construction substrate; no accepted classification |
| [order conditional/event/exec](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/tutorials/07-orders.md) | SHIPPED in first-party tutorial | Candidate future signal/scheduled check + actor invocation; avoid reinventing scheduler |
| [config patches](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/guides/gastown-config-recipes.md), [reload](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/cmd/gc/cmd_reload.go) | SHIPPED source/config surface | Authorized later effect must be checked with real first-party session outcome |
| [runtime registry](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/cmd/gc/runtime_registry.go), [pack runtime resolver](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/internal/config/pack_runtimes.go) | SHIPPED source code | No new provider framework absent proven demand |
| [#8419](https://github.com/gastownhall/gascity/issues/8419) and [#8367](https://github.com/gastownhall/gascity/issues/8367) | OPEN original Issues | Concrete outdated model aliases/pricing; fix natively, not VSM controller |
| [#19](https://github.com/gastownhall/gascity/issues/19) | OPEN original Issue | Rate-limit/account rotation = chiefly current recovery, not prospective S4 closure |
| [#2075](https://github.com/gastownhall/gascity/issues/2075), [#9006](https://github.com/gastownhall/gascity/issues/9006) | OPEN original Issues, some primitives have landed | Provider/runtime contracts; do not reimplement or claim all design shipped |
| [PR #8693](https://github.com/gastownhall/gascity/pull/8693) | OPEN / UNMERGED @ `8dbcddac9fc710430aef7362f7e53f9da4eee5f7` | Reactive `standby_provider`; independent future S4 difference must be shown |
| [PR #2718](https://github.com/gastownhall/gascity/pull/2718) | OPEN / UNMERGED @ `12d2f286e537495b7f3798f32b738afca3fe5c70` | K8s provider identity; only integrate if required |
| [#8370](https://github.com/gastownhall/gascity/issues/8370) | OPEN / maintainer DEFERRED pending eligible case | Conversation preservation constraints; no broad automatic resumption |
| [Gas City ROADMAP](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/ROADMAP.md) | 1.6 reliability/performance/onboarding priorities | Big new SDK abstraction risks low maintainer priority |

**No installed S4 capability is assumed absent simply because its assessment is missing.** Confirm whether an existing custom pack already constructs A→E before a new SDK API is proposed. An OPEN PR is not shipped.

## 3. Minimal S4-specific ports — only if native first pass proves a gap

| Port | Proposed first-party binding and data | Owner / enforcement / feedback |
| --- | --- | --- |
| **A · ProspectiveSignal** | Signed/trusted vendor release-change evidence, affected provider family/models, effective date, expiry, source link. Could enter via order check or event, not a new global poller | Only verified prospective events qualify |
| **B · LawfulOptions** | Current allowed catalog & configured agents → versioned `retain`/`migrate`/`hold` alternatives, compatibility and policy constraints | No fabricated compatible provider, no unapproved credentials |
| **C · DeveloperDecisionActor** | A real developer-composed, bounded Gas City agent/formula receives A+B and emits option ID, reason, expected future-state revision | Developer composes decision strategy; hardcoded fallback and prompt alone are not C |
| **D · FutureOnlyApply** | Approved decision is mapped into a supported pack/city configuration edit and reload with compare-and-swap or equivalent staleness protection | Existing active sessions/leases protected; S3/reconciler retains current operational authority |
| **E · LaterOperationReceipt** | Durable causal choice ID → later agent session's effective provider/model ID and actual start/task success/failure → returned to current S3 and future decision memory | Never mark success merely because config parse/reload succeeded |

**Conditional sufficiency:** Only a supported original-native end-to-end A+B+C+D+E (including independently different lawful decisions, a negative missing-actor case and later session feedback) might support a proposed Gas City `S4=C` claim for later Index assessment. None of these ports is asserted newly needed or currently shipped as a complete pipeline.

The S4 actor is *not* authorized to alter S5-level policy (which providers/credentials are allowed, budgets, external posting) and does not override the reconciler S3 owner. A prospective change is different from S3 crash/retry/quota rotation.

## 4. P0/P1/P2 sequencing and stop thresholds

**P1-A / first:** select a real, bounded future provider change with two accepted compatible alternatives. Check if original issues or recent PRs already close it. Obtain an independently accepted Gas City assessment (no claim of grades until then).  
**P1-B / experiment:** build *only an isolated native pack/order/formula prototype* (after separate permission); compare manual config override vs actor-selected alternative on the same frozen city scenario. No SDK code without fail evidence.  
**P1-C / rights and receipt:** prove future-only config apply, session-state protection, stale decision refusal, correct provider identity on later actual session and feedback to S3.  
**P0 / conditionally:** if the developer-composed S4 witness is materially useful and not doable with shipped primitives, propose precisely the missing smallest supported first-party port. Prefer a pack-level solution when sufficient.  
**P2: NONE** — no generic extra manager, no S5 takeover.

**Stop `NO_USEFUL_CHANGE`:** native manual config or a pack/formula covers the same useful change at equal/lower whole-life cost, or upstream accepted overlapping work resolves it.  
**Retain `NEEDS_EVIDENCE`:** no real compatible future event, unclear gap, no trustworthy authorized apply, no actual later session witness, or unknown need.  
**`DECISION_READY`** only as a future engineering disposition when a specific bounded native deficiency, non-duplicative implementation path and falsifiable user outcome are established. An Index grade and maintainer adoption remain distinct.

## 5. Source-native proposed test cases (NOT RUN)

| Test | Setup / stimulus | Expected observable outcome or falsifier |
| --- | --- | --- |
| T01 positive migration | Frozen scratch city with two *approved* providers and real future-change notice; developer-composed S4 actor selects one | Later Gas City session's effective provider/model matches selected approved config, task output/receipt returned to controller |
| T02 lawful hold | Same facts, actor returns `hold` | Durable hold reason, no config mutation, later session remains on prior provider |
| T03 no developer actor | Remove composed S4 actor, retain ordinary order/config infrastructure | No fake autonomous S4 selection; operator/manual control still works |
| T04 unauthorized option | Candidate provider lacks operator approval or requires secret rights | No config effect or secret exposure; explicit denied receipt |
| T05 stale revision | Decision prepared before a different config/release update | Application rejects obsolete decision, no lost operator change |
| T06 active session | A worker holds a live lease when future-only migration is chosen | Existing agent/work not forcibly restarted; only eligible later session changes |
| T07 launch failure | New provider cannot launch or resume | Actual failure attached to decision; S3 observes failure; no fabricated success |
| T08 unmerged conflict | Candidate assumes capabilities only in PR #8693 or #2718 | Test fails/capability labeled unshipped; no hidden dependency on PR branches |
| T09 native benchmark | Equivalent manual provider patch + reload and later session run | If same useful outcome at equal/lower cost, no new SDK constructor |
| T10 unsupported runtime | Pack-declared runtime unavailable or invalid | Fail closed in supported first-party distribution; no silent fallback as claimed S4 success |

**Native test command guidance, future implementation only:** `make check` (Bazel unit/policy), `make test-acceptance` for CLI end-to-end, `make test-integration` for config/controller/session outcomes. Run scratch city only; never alter a live operator deployment. **No commands executed in this study.**

## 6. Independent alternatives, ownership and economic question

- Product-native: use Gas City pack/order/formula/agent configuration and the established provider/reconciler contracts first; no provider-specific manager embedded in the SDK.
- Profile/Skills: use the independent Index process to classify the real actor/control/return boundary, without copying Gas Town's vector.
- Domain pack/fork: compare alternative future-provider decision policies independently in a permitted experimental configuration.
- Cost: same prospective provider change, baseline vs adaptation. Measure build, review, tests, compatibility, prevented failed sessions, human interventions and operational maintenance. **NOT_MEASURED**.

**Final narrative status: NEEDS_EVIDENCE.** This contract is a falsifiable construction target, not proof that a new SDK port is required or that `S4=C` exists.
