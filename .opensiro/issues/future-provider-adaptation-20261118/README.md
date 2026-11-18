# Gas City — assessment-backed OpenSiro roadmap

**FINAL OPERATOR DECISION: `NO_GO` for adding a new SDK/core S4 adaptation controller now.**  
**Research result: `NEEDS_EVIDENCE` on a useful additional capability; not a proved `NO_USEFUL_CHANGE`.**  
**PLAN_ONLY · INDEX_PREREQUISITE_PASSED · NOT PUBLISHED · NOT IMPLEMENTED.**

## Canonical accepted assessment — mandatory preflight satisfied

- [Gas City canonical assessment](https://github.com/opensiro/vsm-harness-index/blob/34e11ec4dd52e1ba3ee0111d8bca73f13918f54f/assessments/ga/gascity.md) from `opensiro/vsm-harness-index@34e11ec4dd52e1ba3ee0111d8bca73f13918f54f`, **blob `91478bc006342a6f92f41e3670d5708e50592da1`**, `status: included`, catalog position **1287** with matching `repository` and `review_ref`.
- Accepted **S1=A, S2=C, S3=P, S3*=C, S4=—, S5=—**. Profile **0.2.4**, Methodology **0.3.8**, reviewed **2026-11-18** at `03f6fe825cf0a54c677c241e4aaa7e76dade28a5`.
- Current original [`gastownhall/gascity/main`](https://github.com/gastownhall/gascity/commit/03f6fe825cf0a54c677c241e4aaa7e76dade28a5) checked at the same ref. Accepted assessment age at study: **0 days**; no new-ref re-review needed.
- Verified parent: [working fork](https://github.com/opensiro-contributions/gascity) is a fork of `gastownhall/gascity`, `opensiro/meta` is separate from unchanged product `main`.

## Final case documents

- [issue.md](issue.md) — Human decision: why OpenSiro, accepted six-function baseline, original alternatives, concrete `NO_GO` and remaining evidence.
- [constructor-sufficiency.md](constructor-sufficiency.md) — AI/developer proof-of-sufficiency contract, negative tests and minimal native retry condition.
- [roadmap.md](roadmap.md) — source-pinned Capability Roadmap Receipt, admitted Index refs, rights, priorities, terminal decision, publication gate.
- [verification-20261118.md](verification-20261118.md) — independent assessment-backed rerun and documented correction of the earlier premature `NO_USEFUL_CHANGE`.

The original preliminary `NEEDS_EVIDENCE`, and subsequent pre-assessment `NO_USEFUL_CHANGE`, are retained in Git history, **not ratified as canonical prior decisions**. The [Upstream prerequisite protocol](https://github.com/opensiro/upstream/blob/main/PROTOCOL.md#mandatory-accepted-assessment-prerequisite--fail-closed) was satisfied before this re-evaluation.

## Native-first S4 feasibility checkpoint (2026-11-18)

**New next step:** [native-s4-feasibility.md](native-s4-feasibility.md) specifies the concrete future-provider counterfactual, supported first-party entry points, positive/negative evidence, baseline comparison and terminal `PACK_SUFFICIENT / GO_MINIMAL_PORT / NO_GO / BLOCKED` decision criteria. **This is a plan only, NOT_RUN**, and does not rescind the terminal `NO_GO` for a *new universal SDK controller*. Do not implement other original Issues in bulk as an experimental prerequisite. New approved implementation or public publication still needs its normal consent gate.

**Latest original `main` checked for this plan:** [`3764de45ea174753b4a401d98f6ab86740a151f7`](https://github.com/gastownhall/gascity/commit/3764de45ea174753b4a401d98f6ab86740a151f7); [compare with accepted assessment ref](https://github.com/gastownhall/gascity/compare/03f6fe825cf0a54c677c241e4aaa7e76dade28a5...3764de45ea174753b4a401d98f6ab86740a151f7). Three post-assessment commits affect claim/session/test handling, not a shipped prospective S4 loop. Accepted Index `review_ref` is still `03f6fe825cf0a54c677c241e4aaa7e76dade28a5`.

## What to do now

**Do not** add another global SDK controller, create an original feature/PR, publish an unapproved fork Issue, or classify a proposed S4 constructor as shipped. **Do** reuse existing first-party packs, orders, formulas, agent provider patches and exact original Issues. If a real future-provider disturbance and affected developer workflow become available, compare manual/native pack with an autonomous developer-composed policy and reopen a *new bounded* roadmap only if the existing first-party path demonstrably fails a user goal.

**Public GitHub fork Issue:** NOT CREATED. The [complete local Human Issue draft](issue.md) remains a research artifact and may not be published without exact fresh owner consent; current `NO_GO` means publication is not recommended. Original-repository communication: NONE. Product code: NONE. Native tests: NOT_RUN. Cost: NOT_MEASURED.

## Post-assessment source freshness — 2026-11-18T18:49:01Z

The accepted Index `review_ref` **remains frozen** at [`03f6fe825cf0a54c677c241e4aaa7e76dade28a5`](https://github.com/gastownhall/gascity/commit/03f6fe825cf0a54c677c241e4aaa7e76dade28a5). Later on the same day the original `main` advanced one commit to [`d1c45f12f6a7102333c6574fe6de571377fd532f`](https://github.com/gastownhall/gascity/commit/d1c45f12f6a7102333c6574fe6de571377fd532f) ([exact comparison](https://github.com/gastownhall/gascity/compare/03f6fe825cf0a54c677c241e4aaa7e76dade28a5...d1c45f12f6a7102333c6574fe6de571377fd532f)): [#8127](https://github.com/gastownhall/gascity/pull/8127) — `feat(hook): honor gc.exclude_claimants on every claim tier`.

The changed `cmd/gc/cmd_hook*.go`, `internal/beadmeta/exclude_claimants.go`, `internal/config/workquery.go`, workquery fixtures/tests and CLI reference affect **current work claim/routing mechanics**. They do not supply a prospective provider/model signal, S4 adaptation chooser, future-policy apply or downstream adaptation feedback in the investigated S4 case. Thus **the assessment's historical pin is not silently advanced** and the narrow roadmap **NO_GO** for a *new S4 SDK controller* remains supportable. A separate Index owner may re-review affected S2/current-operation interpretations if future evidence warrants it; this check is **not** canonical new-ref reassessment.

The local [accepted-source roadmap receipt](roadmap.md) records the independently observed newest original HEAD while keeping the accepted `review_ref` unchanged. No tests of the new source were executed in this freshness check. Source and Index are not asserted byte-identical at the later observation time.
