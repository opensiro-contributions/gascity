# Gas City — native-first S4 constructive sufficiency check

**Status: PLAN_ONLY / NEXT CHECK DESIGNED / NOT_RUN.**  
**Current engineering decision: NO_GO on a NEW generic SDK/core S4 controller.**  
**Research question remains open:** Can a developer construct a lawful, useful prospective S4 loop from existing first-party mechanisms, and if not, exactly what *smallest* missing port blocks it?

This is the **next validation step within the existing Gas City case**, not a replacement Index assessment, a new implementation authorization, a new public Issue or an automatic upgrade. The previous terminal decision stays bounded to the proposed universal SDK feature. Completion of this plan requires additional actual evidence; merely saving it does **not** establish native sufficiency or the absence of a useful improvement.

## 0. Admission, source and authority

- Exact original: [`gastownhall/gascity`](https://github.com/gastownhall/gascity), MIT.
- Accepted Index: [Gas City general assessment](https://github.com/opensiro/vsm-harness-index/blob/34e11ec4dd52e1ba3ee0111d8bca73f13918f54f/assessments/ga/gascity.md), Index commit `34e11ec4dd52e1ba3ee0111d8bca73f13918f54f`, assessment Git blob `91478bc006342a6f92f41e3670d5708e50592da1`, catalog row **1287**, `status: included`, Profile **0.2.4**, Methodology **0.3.8**. Reviewed source `03f6fe825cf0a54c677c241e4aaa7e76dade28a5` on 2026-11-18.
- Accepted six-state vector (not an implementation plan): **S1=A · S2=C · S3=P · S3*=C · S4=— · S5=—**. The bounded `S4=—` state means no complete first-party future-adaptation loop was established in the *assessed installed mode*. It does not prove that an additional controller would help.
- Latest original `main` seen while preparing this plan: [`3764de45ea174753b4a401d98f6ab86740a151f7`](https://github.com/gastownhall/gascity/commit/3764de45ea174753b4a401d98f6ab86740a151f7) on 2026-11-18. [Compare with assessment review ref](https://github.com/gastownhall/gascity/compare/03f6fe825cf0a54c677c241e4aaa7e76dade28a5...3764de45ea174753b4a401d98f6ab86740a151f7): three commits — claim exclusions (#8127), closed named-session identity (#9128) and worker-environment test hang budget (#9267). They affect current claim/session/test mechanics, not the documented first-party prospective-provider policy loop. The accepted `review_ref` **must not** be silently repinned.
- Current first-party evidence is pinned to accepted source `03f6fe825cf0a54c677c241e4aaa7e76dade28a5`: [agents/formulas](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/docs/getting-started/how-gas-city-works.md), [order triggers](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/docs/tutorials/07-orders.md), [provider config patches](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/docs/guides/gastown-config-recipes.md), [config editor](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/internal/configedit/configedit.go), [reload](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/cmd/gc/cmd_reload.go), [runtime registry](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/cmd/gc/runtime_registry.go) and [event documentation](https://github.com/gastownhall/gascity/blob/03f6fe825cf0a54c677c241e4aaa7e76dade28a5/engdocs/architecture/event-bus.md).
- **Rights:** fork `opensiro/meta` metadata can retain this plan; a new custom pack, source code, actual run that modifies a deployed city, external correspondence or public fork Issue requires its applicable separate owner approval. An isolated purely read-only inspection may proceed under ordinary research authorization. No GitHub original/fork product branch change follows from documenting this plan.

## 1. Exact counterfactual user task and experiment inputs

**User:** city operator responsible for a few approved coding agents across rigs who faces an upcoming model/provider discontinuation and wants the *next eligible session* to use an approved alternative without silently interrupting existing work.

**Eligible S4 stimulus:** a real or explicitly **synthetic test fixture** describing a **future** change in model availability/compatibility. Include `source`, `observed_at`, `effective_at`, `provider`, `model`, `affected_agents`, `verified`, `fixture`, and an immutable notice ID. A current HTTP 429, retry, alias spelling error or quota exhaustion does not establish this S4 distinction.

**Alternatives:** `retain`, `migrate`, `hold`, each accompanied by an *operator-provided* allowlist/compatibility decision and expected configuration revision. The agent may **select among lawful options**, never add a new provider, secret, budget, credential scope or S5 right.

**Success for a real S4 claim:** prospective notice → lawful alternatives → independently configured developer decision agent chooses one → first-party protected effect on **later eligible** work → actual later session provider/model + task result/failed result causally returned to current S3 management. All five links must be attributable to shipped first-party entry points. A simulated notice can prove a technical pathway but **not** external demand, actual vendor risk or economic value.

## 2. Four ordered, bounded checks — do not implement everything in the existing issue queue

### Check 1 — Native capabilities and smallest supported scenario

Inventory the reviewed source, then verify exact latest source for changes relevant to the experiment. Trace the supported **order → formula/agent → lawful decision → config editor/reload → later session** path with runtime guards. Pin actual source files and test names; do not assume all interfaces are accessible or safe just because the building blocks exist.

Document a manual baseline with an already approved provider/model patch and normal configuration reload. If even the manual provider transition cannot safely preserve active work, document that **before** testing an autonomous actor. No original product code change.

### Check 2 — Constructive sufficiency and rights, first party first

Design, and execute **only after appropriate implementation/run authorization**, an isolated scratch-city opt-in pack/order/formula variant using already shipped native interfaces. The agent decision actor must be developer-composed and must have two causally different lawful choices. An independent protected application bridge may be necessary; **do not give a model unrestricted controller-side `exec`, raw config writes, credentials or a fabricated cross-process CAS capability**.

Require protected authority checks for operator allowlist, stale config revision, concurrent human edits and in-flight session leases. If native `gc reload` reports `accepted` or `applied`, that is **not** completion: attach the effective runtime of an actual later started session and its task outcome to the choice ID.

### Check 3 — Source-owned overlap and necessity

Before suggesting a feature PR, check the precise existing original issues/PR heads and compare *function plus actor plus downstream right*, not matching keywords:

- [#8419](https://github.com/gastownhall/gascity/issues/8419) model aliases and [#8367](https://github.com/gastownhall/gascity/issues/8367) price metadata: narrow present defects; their repair is **not** a prerequisite to every S4 experiment.
- [#19](https://github.com/gastownhall/gascity/issues/19) quota/account and [PR #8693](https://github.com/gastownhall/gascity/pull/8693) standby provider: chiefly reactive failure handling, not proof of prospective choice.
- [#2075](https://github.com/gastownhall/gascity/issues/2075) provider/runtime packs, [#9006](https://github.com/gastownhall/gascity/issues/9006) runtime protocol, [PR #2718](https://github.com/gastownhall/gascity/pull/2718) runtime identity: possible owner work; never count an unmerged PR as shipped.
- [#8370](https://github.com/gastownhall/gascity/issues/8370) deferral of broad conversation retention: conservatively protect active sessions; do not silently revive a rejected adjacent feature.

For every missing link, distinguish **missing existing configuration**, **needs a domain-specific pack only**, **genuine narrow first-party SDK gap**, **operator policy/authorization problem**, or **not supported / no validated user need**. Link concrete source/PR evidence rather than collecting a generic feature wishlist.

### Check 4 — Matched baseline, falsifiers and final engineering decision

Use the **same notice, affected agent, allowed choices, concurrency preconditions and later task** for both manual/native baseline and developer-composed alternative. Record total engineering/test/review effort, repeated human interactions, failed launches, in-flight disruption, security violations and maintenance; state `NOT_MEASURED` until numbers genuinely exist.

| ID | Scenario / stimulus | Oracle — must observe in an actual authorized scratch run |
| --- | --- | --- |
| **AC-01** | Verified future notice, two approved alternatives, configured S4 actor selects `migrate` | Later eligible first-party session runs on the chosen approved runtime/model; linked task/feedback receipt returned |
| **AC-02** | Same eligible facts, actor selects `hold` | No configuration mutation; durable hold reason; later run remains on its prior lawful setting |
| **AC-03** | Omit S4 actor and retain standard orders/config | No imaginary autonomous choice, while normal manual/current workflow continues |
| **AC-04** | Expired/unverified future notice, unavailable or forbidden provider | Refused/held, no secret or policy escalation; explicit failure/denial evidence |
| **AC-05** | Operator edits config after choice, or eligible worker has active lease | Stale apply rejected; in-flight worker not forcibly restarted or silently switched |
| **AC-06** | Reload succeeds but selected provider fails at next launch/resume | Real later task failure returned; **no false S4 success** |
| **AC-07** | Native-only manual/pack baseline yields same protected later result | Additional SDK controller disallowed absent a demonstrable incremental user benefit |
| **AC-08** | Fixture is synthetic, or no qualifying user need can be sourced | Technical conclusion may be `PATH_PLAUSIBLE`, but demand/value remains `NEEDS_EVIDENCE` — never claim proved utility |

**Proposed evidence to preserve when and only when run:** frozen notice/allowlist/config snapshots; exact source and installed version; actor configuration; optional pack file diff; command/test logs; observed session ID, provider/model, task result and linked decision ID; operator rights and failure receipts; baseline vs variant time/maintenance comparison; original overlapping issue/PR status at measurement. **None of these run artifacts exists or is claimed by this document.**

## 3. Mandatory decision rules (do not conflate grades with engineering gates)

| Outcome of this check | Engineering disposition | Assessment effect |
| --- | --- | --- |
| Native pack/formula + protected first-party application **achieves** the user task at reasonable cost | **NO_GO_CORE / PACK_SUFFICIENT** — optionally document the reusable pack; no new generic SDK controller | **No automatic S4 grade**; independent Index reassessment if supported boundary changes |
| Native comparator **reproducibly fails** a necessary first-party integration despite allowed rights, and a concrete user benefit survives the original overlap review | **GO_MINIMAL_PORT** — specify **one** missing SDK/config/session/receipt port, a test and minimal PR scope through a **separate Upstream upgrade/consent gate** | Still no grade until separately assessed |
| Only manual path succeeds; developer composition would increase risk/cost without a named independent need | **NO_GO** — keep manual/provider issue route | No grade change |
| Technical path plausible, but prospective user demand, current source binding or actual later outcome unavailable | **BLOCKED / NEEDS_EVIDENCE** on *further implementation*, with explicit missing witness; not a disproven S4 idea | No grade change |
| Safety/rights/active-session requirements cannot be met by an authorized supported implementation | **NO_GO_UNSAFE** — do not bypass via privileged shell or guessed authority | No grade change |

**This stage may conclude `GO` only for the smallest demonstrated residual first-party port, not for "add S4" in general.** The general VSM assessment and any domain-specific pack assessment are separate authority chains. Do not implement #8419, #19, #2075 or other issues *as a speculative dependency* merely to see what happens.

## 4. Current documented result / next action

- **Plan prepared**: YES, pinned source, canonical assessment, positive/negative tests, source overlap, rights and stop rules.
- **Original-native runtime proof**: NOT_RUN.
- **Real prospective user need**: NOT_ESTABLISHED.
- **Measured benefit**: NOT_MEASURED.
- **Universal S4 SDK constructor**: **NO_GO remains in effect**.
- **Immediate permitted action**: source-first static tracing and preparation of a disposable fixture and evidence checklist. Any executable pack/model session, deployed configuration effect, outside original maintainer communication or public fork Issue needs its independent applicable approval.
- **Return to user**: record which link actually fails, the smallest native alternative and one of the decision outcomes above, not another undifferentiated request to "wait for all other issues."

**AI assistance disclosure:** This is an AI-assisted *research/test plan*, not evidence of actual first-party runtime behavior or an accepted S4=C constructor.
