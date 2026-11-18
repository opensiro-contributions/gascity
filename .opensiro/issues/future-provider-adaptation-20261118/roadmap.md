# Capability Roadmap Receipt — Gas City (source-pinned PLAN_ONLY)

**FINAL FOLLOW-UP DECISION (2026-11-18): `NO_USEFUL_CHANGE` for a NEW Gas City SDK/core S4 constructor.** The initial `NEEDS_EVIDENCE` plan and conditional P0 below are superseded **as an implementation recommendation**. Verified native agents/packs/orders/formulas/configuration and the existing narrower original issues do not establish any missing SDK port or incremental user benefit. **This is not an accepted VSM grade or proof of complete S4=C.** [Full source-native verdict](verification-20261118.md). No public fork/original Issue is recommended or published for this rejected SDK proposal.


## Identity and pins

- Original repository: gastownhall/gascity
- Original HEAD: 03f6fe825cf0a54c677c241e4aaa7e76dade28a5
- Initial case observed HEAD: 208a43158ccd33a8f1e066d80daf65c9f3bea713 (one intervening orphan-cleanup commit, irrelevant to this S4 decision).
- Observed at: 2026-11-18
- Accepted Index assessment: NOT_AVAILABLE — no Gas City assessment found in the canonical Index tree at https://github.com/opensiro/vsm-harness-index/commit/5f6ea0c777733813ca42e3f210390a719488dcfb
- Accepted assessment blob SHA: NOT_AVAILABLE
- Accepted review ref: NOT_AVAILABLE
- Accepted reviewed at: NOT_AVAILABLE
- System in focus: One first-party Gas City deployment with city pack and rig scopes, agents, work beads, orchestrator, order triggers, events, runtime registry, config and session reconciliation; external provider vendor lifecycles and third-party packs are not automatically owned by the core.
- Profile/Skills attribution: NOT_AVAILABLE for Gas City (do not import Gas Town's accepted vector).
- Index audit: canonical vsm-harness-index main `5f6ea0c777733813ca42e3f210390a719488dcfb` on 2026-11-18, recursive tree filename search no `gascity`; Index issue search no `gascity`. Treat accepted six-function vector as NOT_ASSESSED, not a negative grade.
- Original default/main HEAD and fork HEAD matched at creation; separate https://github.com/opensiro-contributions/gascity has parent `gastownhall/gascity`. Original commit link: https://github.com/gastownhall/gascity/commit/208a43158ccd33a8f1e066d80daf65c9f3bea713.
- Human Issue: https://github.com/opensiro-contributions/gascity/blob/opensiro/meta/.opensiro/issues/future-provider-adaptation-20261118/issue.md
- AI/developer technical contract: https://github.com/opensiro-contributions/gascity/blob/opensiro/meta/.opensiro/issues/future-provider-adaptation-20261118/constructor-sufficiency.md

## Rights and authority

- MIT source license: https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/LICENSE
- Contributor guidance: https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/CONTRIBUTING.md ; original [ROADMAP](https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/ROADMAP.md) recommends feature-form Issue for substantial work; Bazel `make check`, acceptance and integration tiers. Using AI is allowed with human responsibility.
- External third-party interaction, original Issue/PR/comment and public fork Issue publication are distinct consent gates. No CLA/DCO exclusion or AI disclosure-policy waiver is assumed.
- Verified fork `opensiro-contributions/gascity`, parent `gastownhall/gascity`, `opensiro/meta` dedicated for research. Owner's present request permits fork provisioning/persisting one named research case, NOT public text publication, code implementation or third-party maintainer interaction.
- Fork metadata owner control: initial scoped ALLOW decision for case persistence only, event attribution in `.opensiro/events/`. No broad automatic publication mandate.

## Existing work / overlap

**Original source SHIPPED at `208a43158ccd33a8f1e066d80daf65c9f3bea713`:**
- https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/getting-started/how-gas-city-works.md — six generic primitives, durable formula workflow and event bus.
- https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/tutorials/07-orders.md — orders can invoke formulas or commands on schedule, condition or events; generic automation does not imply S4.
- https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/docs/guides/gastown-config-recipes.md — root/rig provider override through pack patches, not a future autonomous decision witness.
- https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/cmd/gc/runtime_registry.go and https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/internal/config/pack_runtimes.go — pack-declared runtime registry and supported config validation.
- https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/cmd/gc/cmd_reload.go — source-native configuration reload; changes to active sessions require separate protected lifecycle evidence.
- https://github.com/gastownhall/gascity/blob/208a43158ccd33a8f1e066d80daf65c9f3bea713/ROADMAP.md — first-party 1.6 priorities: reconciler reliability (#7093), performance (#7094), contributor onboarding (#7095).

**Original work / source status observed 2026-11-18:**
- [#8419 stale model aliases](https://github.com/gastownhall/gascity/issues/8419): OPEN, concrete stale model catalog, not a future-controller request.
- [#8367 model-pricing gap](https://github.com/gastownhall/gascity/issues/8367): OPEN; no assertion model cost fixed.
- [#19 account/quota rotation](https://github.com/gastownhall/gascity/issues/19): OPEN, mainly present-rate-limit response.
- [#2075 provider/runtime pack split](https://github.com/gastownhall/gascity/issues/2075): OPEN, proposed architecture; some registry and pack functionality already present.
- [#9006 runtime protocol completeness](https://github.com/gastownhall/gascity/issues/9006): OPEN, first-party maintainers are evaluating missing capabilities.
- [#8370 asleep config drift](https://github.com/gastownhall/gascity/issues/8370): OPEN / deferred until eligible case; only same-provider bounded resume conditions even discussed.
- [PR #8693 standby provider](https://github.com/gastownhall/gascity/pull/8693): OPEN, UNMERGED, head `8dbcddac9fc710430aef7362f7e53f9da4eee5f7`, reactive stall response.
- [PR #2718 k8s runtime identity](https://github.com/gastownhall/gascity/pull/2718): OPEN, UNMERGED, head `12d2f286e537495b7f3798f32b738afca3fe5c70`.
- [PR #4967 event-driven reconciliation](https://github.com/gastownhall/gascity/pull/4967): OPEN, UNMERGED, head `cd8854f3b80912faca40e04e5534bb2a98e6fb91`.

## Function ownership

- Canonical S1: NOT_ASSESSED; configured agents execute work, but no accepted current Index owner state.
- Canonical S2: NOT_ASSESSED; orchestrator/dependency gating present, no accepted ownership classification.
- Canonical S3: NOT_ASSESSED; reconciler maintains present session/resource state, no accepted ownership classification.
- Canonical S3*: NOT_ASSESSED; review steps may be independently configured, but no accepted complementary-audit witness.
- Canonical S4: NOT_ASSESSED; future provider options may be composed using packs, orders, agents and runtime selection, but first-party future-disturbance → autonomous lawful choice → guarded later-session operation → feedback **not established**.
- Canonical S5: NOT_ASSESSED; reserved operator/provider-policy rights not a default autonomous S5 grade.
- Disturbance: credible, externally verified prospective model/provider lifecycle change, not a current 429/retry failure.
- Decision owner: candidate independently developer-composed S4 actor operating within delegated options; S3 current operational state remains owned by orchestrator/reconciler; S5 reserved policy cannot be altered.
- Return: actual future session ID, effective provider/model, task/result/failure must feed back into current management, not just return a static suggestion.

## Capability priority

- **P0 / REJECTED conditional S4 C-construction hypothesis (historical; NO new SDK core):** source-linked future provider disturbance → versioned compatibility/options → developer-composed lawful choice `retain/migrate/hold` → guarded first-party config/session effect in a later session → observed real feedback to S3. This is not an Index C grade or a proved new need.
- **P1 / prerequisites:** independent accepted Index baseline; actual future input and alternative compatible runtime; first-party native manual vs pack/formula/agent pilot; staleness/right checks; protected active sessions and subsequent results; measure material value.
- **P2 / NONE:** no separate compelling S3 or S5 constructor.
- **C sufficiency claim:** NOT_PROVEN. Five linked first-party ports, a developer-configured autonomous choice and positive/negative later-session tests are required before a formal candidate can be proposed.
- **Decision:** NO_USEFUL_CHANGE for adding a *new SDK/core S4 adaptation constructor*. Existing native composition and specific owner issues are the next lowest-cost paths; no S4 closure/grade is asserted. [Final evidence](verification-20261118.md).

## Implementation options

- First and cheapest: current root/rig `[[patches.agent]]`, provider config and native order/formula with real future signal, approved options and manual review. May be sufficient.
- If user task needs an autonomous future decision and existing pieces can compose it, implement only as a permitted Gas City pack/agent policy (no new core API).
- Only if a first-party safety/feedback integration is genuinely missing after a tested native prototype, propose its smallest SDK config/session/receipt change to original's owner. Avoid duplicating #19, #2075, #9006, #8693, #2718 and #8370.
- Proposed acceptance cases T01–T10 in [AI companion](https://github.com/opensiro-contributions/gascity/blob/opensiro/meta/.opensiro/issues/future-provider-adaptation-20261118/constructor-sufficiency.md) include future positive, alternative hold, missing actor, unauthorized provider, stale revision, active-session protection, failed launch, missing unmerged capability, baseline comparison and unsupported runtime.
- Native tests: NOT_RUN; future code would require `make check`, `make test-acceptance`, `make test-integration`, test-scratch-city isolation and actual CI evidence.
- If no material capability, classify idea `NO_USEFUL_CHANGE`. A necessary future governance/rights choice remains human.

## Specification and domain alternatives

- Independent Index assessment under canonical Index ownership; no copied Gas Town vector and no newly asserted C. Profile/Skills work only if a genuine methodology ambiguity survives source evidence.
- Domain-specific experimental pack/fork independent of original Go implementation; compare developer-composed options with manual current native workflow.
- Original third-party feature discussion and outward code PR require distinct exact current-conversation consent; this research does not contact maintainers.

## Cost experiment

- Same prospective provider migration, matched alternative scenarios and supported first-party mode.
- Compare manual native config+reload, pack/order policy and any actual SDK port on implementation/review/test time, repeated adaptation operations, failed later sessions, operator interventions, downtime, security risks and maintenance.
- Cost status: NOT_MEASURED

## Delivery and publication

- Result: NO_USEFUL_CHANGE
- Route: PLAN_ONLY; [exact proposed Human Issue](https://github.com/opensiro-contributions/gascity/blob/opensiro/meta/.opensiro/issues/future-provider-adaptation-20261118/issue.md) + linked AI contract + receipt persisted in dedicated fork metadata.
- Fork public Issue: NOT PUBLISHED; previous draft superseded. No new public feature issue recommended for a rejected speculative core capability.
- External issue: DRAFT — NOT PUBLISHED
- Actual original Issue, PR, code edits, Index acceptance, cost experiments and native tests: NOT_PERFORMED.
- Receipt validator: NOT_PASSABLE_WITHOUT_ACCEPTED_GAS_CITY_INDEX_BASELINE. Canonical validator requires real pinned assessment blob/review SHA/date; no fabricated values; structural source/link and authorization checks reported separately.
- Next permitted action: decline new SDK S4 work. Use existing original issue pathways for concrete bugs; a future new case requires a real prospective user task, a failing native comparator, protected later-session evidence, and cost/benefit.
