# Gas City — independent six-function roadmap receipt (Upstream v0.18)

## Identity and pins
- Original repository: gastownhall/gascity
- Original HEAD: 187bf9a653df221bd82fbee6d14ff4fcb77962a1
- Observed at: 2026-11-19
- Accepted Index assessment: https://github.com/opensiro/vsm-harness-index/blob/394ce776e6945115891b8f7cc459f5a7f7d7aa39/assessments/ga/gascity.md
- Accepted assessment blob SHA: 91478bc006342a6f92f41e3670d5708e50592da1
- Accepted review ref: 03f6fe825cf0a54c677c241e4aaa7e76dade28a5
- Accepted reviewed at: 2026-11-18
- Profile / Skills procedure: 0.2.4 / 0.3.8
- System in focus: installed first-party Gas City with supported bundled core pack, agent sessions, rigs, bead/formula workflow graph, orders, provider abstraction, city controller and reconciler; third-party watcher packs, model vendors, custom agents and parent operator policy are outside the default owner boundary
- Receipt contract: proposal-gate
- Repository-wide source map: README, AGENTS, CONTRIBUTING, ROADMAP, LICENSE, docs and engdocs architecture, Go cmd/gc provider/session/order/config/reconciler, internal runtime/config/orders/beads and bundled pack manifests, examples, tests, Bazel CI, original Issues and PRs; current original commit pinned above
- Accepted VSM vector: S1=A · S2=C · S3=P · S3*=C · S4=— · S5=—
- Target transition: S4=— -> S4=C
- Priority rationale: S1 already has autonomous workers, S2 composable conflict mediation, S3 present city control is legitimately parent/operator-owned, S3* has a composable review quorum, S5 is outside city policy authority; S4 alone offers a bounded prospective-choice gap that can be hypothesized on existing ordered formula and runtime update seams
- S1 disposition: ALREADY_A — configured coding agent chooses task operations and returns finished bead and code/result
- S2 disposition: ALREADY_C — developer-configured workflow/preflight resolves competing scoped work and branch effects, rather than assuming scheduler equals autonomous coordination
- S3 disposition: PARENT_P — operator selects current city interventions; city controller/reconciler enforces valid commands and configuration; new S4 actor may only act within operator-preauthorized scope
- S3* disposition: ALREADY_C — installed quorum reviewer lanes and synthesis return independent corrective findings into workflows
- S4 disposition: P0_S4_C_HYPOTHESIS — no installed first-party prospective provider-life-cycle actor/qualified future-choice/guarded later-session feedback loop; present health gate and order scheduler are reusable parts, not by themselves complete S4
- S5 disposition: NO_TARGET_PARENT_SCOPE — operator/provider credentials, identity and ultimate rules are outside the considered city-level policy loop; deliberate omission UNVERIFIED
- P1 dependencies: source-native provider-future evidence schema and trust/TTL checks; opt-in operator policy/allowlist, existing configuration publication/reload integration with concurrent-edit and active-session safeguards; tests with a later real session receipt
- P2 optional: NONE — do not request a generic S4 controller, new governance engine or independently unnecessary optimization
- Proposed C construction: bounded opt-in first-party future-provider adaptation formula/pack and ONE protected conditional config-application/feedback seam; a developer-composed autonomous model actor selects retain/migrate/hold from preauthorized options, protected configuration effect enters existing controller/reconciler after safe checks, and subsequent actual session outcome is recorded back into the formula's next decision; no new S3/S5 autonomy granted
- C sufficiency falsifier: discover a complete supported stock order/formula plus safe conditional config edit and actual later-session return that needs zero new first-party port; or show that the purported application authority is absent or unsafe, or operator benefit is indistinguishable from native manual route
- Scenario basis: HYPOTHETICAL
- Proposal-stage decision: GO
- Research disposition: NEEDS_EVIDENCE
- Proposed validation: isolated scratch city with synthetic dated provider deprecation notice, two operator-approved providers, same task tested via manual config patch/reload versus optional agent actor, positive retain/migrate/hold and missing-actor/forbidden/stale/concurrent-edit/active-session/launch-fail negatives and linked later-session outcome; source checks now only
- Validation state: NOT_RUN
- Proposal falsifier: native manual or order/pack route already meets all lawful C links with no distinct first-party port, or an authorized actor cannot safely effect a later session without crossing operator policy

## Rights and authority
- MIT: https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/LICENSE. Contributor protocol: https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/CONTRIBUTING.md. External CLA/DCO-specific obligations NOT_VERIFIED.
- Fork state: opensiro-contributions/gascity on opensiro/meta read 2026-11-19, owner_control=ALLOW, attention=WATCHING; authority is fork-local research metadata only, not public Issues/PRs or source implementation
- Parent choice: human city operator owns S3 present commitments and policy allowlist; no autonomous agent may expand providers, permissions or credentials
- This proposal GO is a falsifiable constructibility hypothesis, not an Index regrade, shipped C, maintainer acceptance, implementation, benchmark or feature request

## Existing work / overlap
- SHIPPED: [orders architecture](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/engdocs/architecture/orders.md); [order dispatcher](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/order_dispatch.go); [provider health gate](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/provider_health_gate.go); [provider swap](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/provider_swap.go); [config CLI](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/cmd_config.go); [config-drift deferral](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/config_drift_episode.go); [maintainer roadmap](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/ROADMAP.md).
- Orders dispatch event/cron/condition triggered shell or agent formula work. Provider gate consumes pack-supplied health, and stale/absent health is treated as no enforced negative signal; it does not independently predict future compatibility
- Provider selection and provider swap exist, but `gc config` shows/explains the resolved configuration; no complete supported independently authorized S4 conditional commit + subsequent session verification contract was established in the default first-party boundary
- Current original narrow defects: [#8419](https://github.com/gastownhall/gascity/issues/8419) model alias drift and [#8367](https://github.com/gastownhall/gascity/issues/8367) pricing, not a first-party future S4 actor/return path. [PR #2962](https://github.com/gastownhall/gascity/pull/2962) supplies the present-health gate. Maintainer [ROADMAP.md](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/ROADMAP.md) prioritizes session/reconciler reliability, performance and onboarding, not this hypothetical feature; maintainer interest NOT_STATED
- Native lowest-cost alternative: operator selects allowed provider, edits city config and triggers normal reload; supported order/formula pack may be adequate without any generic new first-party code. That comparison must be tested, not dismissed

## Function ownership
- S1 current actor: configured coding model controls actual coding tasks through launched worker sessions and gives bead/result feedback; already A
- S2 current actor: developer-built conflict-aware formula/review coordination via scoped work and preflight; already C
- S3 present owner: human operator, backed by status, suspend/resume, controller and reconciler; legitimate P retained
- S3* independent judgment: separately configured reviewers and synthesis, composable C; no parallel audit subsystem
- S4 current owner: none within bundled standard distribution for prospective future signal→option→authorized later change→task feedback; proposed bounded developer-composed actor would fill this as C only if tested
- S5 identity/ultimate goals: operator/parent authority external to installed city; no local autonomous S5

## Capability priority
- P0: S4=— -> S4=C — prospective provider-compatibility adaptation through first-party opt-in formula and narrow protected update/return seam; source-grounded hypothetical not proof of value
- P1: defined future notices and expiry; allowlisted developer choice; compare-and-swap expected config revision; safe in-flight lease handling; real next session provider/outcome receipt; CI and scratch integration fixtures
- P2: NONE
- Confidence: medium on source-mapped constructor hypothesis; low on incremental operational value; index provenance high

## Parallel contribution-on-top review
- Evaluation object: minimal optional first-party S4 constructor on installed Gas City provider/config/session boundary, not a general new AI supervisor or S3 controller
- Existing-work overlap: shipped orders and formula launch, provider health gate, config diagnostics, provider swap and config drift deferral; original issues #8419/#8367 plus #2962 health gate
- Our on-top contribution: compose those first-party primitives and, ONLY if native pack/manual path lacks this safety contract, add one tested opt-in conditional configuration effect + later-session feedback adapter, not a new scheduler
- Incremental benefit: hypothesized preemptive authorized next-session selection with attributable returned outcome and no manual per-event edit; NOT_MEASURED and must be checked against same-task native baseline
- Decision scope: GO for complete bounded S4 constructor proposal/experiment only; NOT permission to implement, change third-party source or publish, and not an accepted capability/Index grade

| S4 C link | Track A source-native baseline | Track B minimal proposed link | Refuting witness |
|---|---|---|---|
| Future disturbance and lawful options | Current health snapshot and manual `gc doctor`/config, no autonomous forecast guarantee | Dated compatible future-provider evidence plus preconfigured retain/migrate/hold allowlist | Source already provides protected future-event policy port |
| Independent developer-composed actor | Orders schedule exec/formula work, but no shipped S4 chooser | Opt-in formula worker chooses among approved alternatives; absent actor leaves manual mode unchanged | Deterministic script or manual/pack entirely sufficient for same effect |
| Authoritative enforcement | Provider swap, reload, active-work drift deferral | Narrow conditional config apply with current-revision guard and no forbidden provider/suspend surprises | Safe native config edit already offers same envelope/transaction |
| Later real return | Session and bead events/status | Wait for actually launched later session, verify configured runtime and task result; feed evidence back to next S4 choice | Only config-accepted reply available, no lawful outcome attribution |

## Implementation options
- P0 is PLAN_ONLY: build minimal adapter specification and compare native pack script, not an SDK-wide controller; no product implementation authorized
- Test option A: manual update or already-supported order/formula without first-party changes
- Test option B: optional first-party named S4 adapter using existing order + one protected conditional apply/return port, only if A misses necessary safety
- Do not silently amend live city.toml, user secrets or in-flight sessions; consent for actual scratch-city execution and external communication is separate

## Specification and domain alternatives
- Do not rewrite Profile or Skills. A third-party site-specific plugin may solve a single provider problem but cannot be counted as bundled first-party closure without standard supported binding
- Original code owner retains design decisions; no unsupported S5 promotion or required model provider

## Cost experiment
- Paired identical dated synthetic future notice, same city, two allowed options, same next provider-bound task; compare manual change, script/formula pack and proposed protected port
- Measure engineering/test/review/maintenance burden, manual interventions, failed restarts, safe-change refusals and true later-task return
- Cost status: NOT_MEASURED

## Delivery and publication
- Result: PLAN_ONLY
- External issue: DRAFT — NOT PUBLISHED
- Human: [issue.md](issue.md). AI: [constructor-sufficiency.md](constructor-sufficiency.md). Receipt: [roadmap.md](roadmap.md). Existing older [native-s4-feasibility.md](native-s4-feasibility.md) is retained as historic evidence, not execution proof
- Native validation: NOT_RUN; structural validator to be run locally after metadata update
- Historical comparison AFTER independent decision: 2026-11-18 case at fork `b1125cb3` rejected a new generic SDK S4 controller with `NO_GO / NEEDS_EVIDENCE`; this v0.18 re-run selects a narrower **proposal-stage** opt-in first-party S4 actor/application/return design as `GO / NEEDS_EVIDENCE`, explicitly untested and overlapping the previous scenario; no new feature is claimed as discovered or implemented
- No public fork/original Issue, comment, PR, code change or production experiment authorized
