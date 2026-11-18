# Gas City — composable future-provider adaptation roadmap (OpenSiro plan-only)

**FINAL FOLLOW-UP DECISION (2026-11-18): `NO_USEFUL_CHANGE` for a NEW Gas City SDK/core S4 constructor.** The initial `NEEDS_EVIDENCE` plan and conditional P0 below are superseded **as an implementation recommendation**. Verified native agents/packs/orders/formulas/configuration and the existing narrower original issues do not establish any missing SDK port or incremental user benefit. **This is not an accepted VSM grade or proof of complete S4=C.** [Full source-native verdict](verification-20261118.md). No public fork/original Issue is recommended or published for this rejected SDK proposal.


**OpenSiro architecture-first pilot · PLAN_ONLY · NEEDS_EVIDENCE · PUBLIC FORK ISSUE DRAFT — NOT PUBLISHED.**  
**Source:** [gastownhall/gascity @ `208a43158ccd`](https://github.com/gastownhall/gascity/commit/208a43158ccd33a8f1e066d80daf65c9f3bea713) (main observed 2026-11-18).  
**Companions:** [AI/developer sufficiency contract](https://github.com/opensiro-contributions/gascity/blob/opensiro/meta/.opensiro/issues/future-provider-adaptation-20261118/constructor-sufficiency.md) · [source-pinned receipt](https://github.com/opensiro-contributions/gascity/blob/opensiro/meta/.opensiro/issues/future-provider-adaptation-20261118/roadmap.md) · [case README](https://github.com/opensiro-contributions/gascity/blob/opensiro/meta/.opensiro/issues/future-provider-adaptation-20261118/README.md).

## 1. Why OpenSiro

OpenSiro tests whether mapping reusable organizational capabilities onto each harness's **existing first-party mechanisms** can standardize agent-harness development and reduce total engineering, integration, validation and maintenance effort. This is an evidence-seeking experiment, not a request to implement VSM terminology, add one controller per letter, or claim proven savings.

Gas City is the appropriate successor to study because the [maintainer migration guide](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/getting-started/coming-from-gastown.md) expressly moves Gas Town roles into configurable **packs**, agent behavior, **formulas**, **orders** and provider interfaces.

## 2. Canonical VSM starting point — NO ACCEPTED INDEX BASELINE

**Index coverage check (2026-11-18):** no `gascity` assessment file was found in [the canonical Index at `5f6ea0c77773`](https://github.com/opensiro/vsm-harness-index/tree/5f6ea0c777733813ca42e3f210390a719488dcfb). The earlier [Gas Town assessment](https://github.com/opensiro/vsm-harness-index/blob/03b3cd41621b85cb4c2418eab574db030493512c/assessments/ga/gastown.md) is for a **different repository and organizational boundary**; it is **not** Gas City's accepted assessment. There is no accepted review date/ref or Profile/Methodology pair for Gas City to carry over.

| Function | Canonical Gas City ownership | Source-native observation, not a grade |
| --- | --- | --- |
| S1 · Operations | NOT_ASSESSED | Configured agents perform work; formulas materialize durable work beads |
| S2 · Coordination | NOT_ASSESSED | Orchestrator dispatches bead dependencies, agent routing and fan-out |
| S3 · Current management | NOT_ASSESSED | Reconciler and health patrol regulate current sessions and capacity |
| S3* · Independent audit | NOT_ASSESSED | Review gates/formulas exist; function ownership and independent closure unassessed |
| S4 · Future adaptation | NOT_ASSESSED | Packs, orders and runtime providers could compose future adaptation; no confirmed full function-specific witness |
| S5 · Identity/policy | NOT_ASSESSED | Operator/provider authority and approval boundaries exist; not an accepted ultimate-policy state |

**No inference from the baseline:** `NOT_ASSESSED` is not `—`, `?`, `A`, `C` or `P`. No grade change or assessment is being published. An independent, source-pinned Index assessment is desirable before making a formal `S4=C` sufficiency claim.

## 3. User need and native baseline

**User counterfactual:** an operator runs a fleet of role-configured coding agents using a model/provider whose supported model IDs, versions or future availability change. They need to **decide in advance** whether to retain the provider, prepare an approved migration or hold, without silently replacing in-flight sessions, breaking credentials/compatibility, or relying on repeated operator hand-edits.

This is supported as a plausible problem by original [#8419 — stale model aliases](https://github.com/gastownhall/gascity/issues/8419) and [#8367 — unpriced newer model](https://github.com/gastownhall/gascity/issues/8367), but these are **specific defects**, not proof of demand for autonomous future adaptation. [#8370](https://github.com/gastownhall/gascity/issues/8370) additionally shows why launch-only configuration drift and session continuation require restrictive evidence.

**Closest shipped original-native alternative:** edit the root or rig [`[[patches.agent]]` provider setting](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/guides/gastown-config-recipes.md) or provider preset, let supported configuration reload reconcile future sessions, and use [existing orders/formulas](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/tutorials/07-orders.md) to collect signals or run an opt-in check. This may already solve the task better than a new constructor. A custom agent prompt without a first-party permitted apply/return path is not evidence of S4 closure.

**Do not duplicate:** [#19 account/quota rotation](https://github.com/gastownhall/gascity/issues/19) (reactive availability), [#2075 provider/runtime packs](https://github.com/gastownhall/gascity/issues/2075) (SDK extensibility), [#9006 runtime contract gaps](https://github.com/gastownhall/gascity/issues/9006), [PR #8693 standby_provider](https://github.com/gastownhall/gascity/pull/8693) (stall-triggered, unmerged), [PR #2718 runtime identity](https://github.com/gastownhall/gascity/pull/2718) (unmerged), or existing per-agent runtime routing. Treat proposed/open work as **not shipped**.

**Maintainer priority constraint:** the first-party [ROADMAP.md](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/ROADMAP.md) currently prioritizes 1.6 session/reconciler reliability, performance and contributor onboarding. This proposed adaptation is **not** an announced maintainer priority.

## 4. Capability priority

| Priority | Decision / measurable outcome |
| --- | --- |
| **P0 — conditional S4** | Test a **developer-composed prospective-provider adaptation** on supported Gas City primitives: future signal → two compatible lawful choices (`retain`, `migrate`, or `hold`) → independently composed decision actor → authorized future-only config/launch outcome → actual later session receipt and feedback. Only add an SDK port if the native pack/order/formula composition cannot close that path. |
| **P1 — evidence and prerequisites** | (a) perform independent Index baseline; (b) pin credible upcoming provider change and compatibility options; (c) run a native-first baseline comparison; (d) verify protected config revision/active-session constraints; (e) bind decision evidence to a real later operation and measure value. P1 evidence precedes product code. |
| **P2 — NONE** | No unrelated S3/S5 upgrade or autonomy escalation justified. |

**Minimum sufficient difference:** a developer can plug in a real bounded S4 decision actor and the supported first-party system executes a lawful different future-session behavior with observable feedback. Generic schedule/event hooks, provider alias fixes, a fixed fallback rule or static policy are **not by themselves** C witnesses.

## 5. Acceptance, falsification and stop

- **Positive:** trusted prospective provider retirement/compatibility warning with two approved options; a *developer-composed* autonomous evaluator chooses one, Gas City safely applies the permitted future configuration, later session starts with the selected runtime, and a real outcome is linked back.
- **Counterfactual:** same inputs, `hold` or a different lawful choice yields a different future outcome; no developer-supplied actor means no invented autonomous S4 decision.
- **Authority and compatibility:** reject unsupported provider, unapproved credentials, stale config revision or a provider whose resume mode cannot preserve the existing conversation. No interruption of active worker rights.
- **False success:** a provider launch/reconciliation failure must yield a failed receipt rather than a claimed adaptation success. Don't relabel current rate-limit handling as future S4.
- **Stop as `NO_USEFUL_CHANGE`:** when native patches, existing orders/formulas or queued upstream work already achieve the same useful later-session result at lower/equal whole-life cost.
- **Stop as `NEEDS_EVIDENCE`:** absent real future input, accepted baseline, safe first-party authorized apply, changed later session, independent consumer demand or ownership clarity.

**Tests are proposed, not executed.** No implementation or Index grading is claimed.

## 6. Independent next paths

1. **Gas City original-native:** prototype a narrow pack/order/formula recipe and document its gaps. Only later, after separate authorization, propose the smallest non-duplicate provider/config/session improvement.
2. **OpenSiro Profile/Skills:** request methodological clarification only if direct evidence finds a genuine S4 ownership/constructor ambiguity.
3. **Domain-specific variant:** use a permitted fork/pack experiment to compare alternative configurations without requiring SDK changes.

## 7. Cost hypothesis and decision

Compare the same planned provider migration using **manual native configuration** vs **developer-composed adaptation**. Collect engineering and test hours, operational intervention frequency, forced restarts, failed later runs, security/compatibility issues and maintenance cost. **`NOT_MEASURED`**.

**Final decision: `NO_USEFUL_CHANGE` for NEW SDK/core S4; the old conditional S4 architecture below is a historical rejected hypothesis.** A bounded future S4 scenario is plausible, and Gas City exposes promising primitives, but whether a *new* first-party constructor is useful is **not established**. This is a complete plan-only case, not an implementation-ready `S4=C` finding. No external-original Issue/PR/comment, public fork Issue or product-code changes are authorized by this document.

**AI disclosure:** Prepared with AI assistance, using public source review. No native tests, independent human audit, actual model-switching experiment or measured savings are claimed.
