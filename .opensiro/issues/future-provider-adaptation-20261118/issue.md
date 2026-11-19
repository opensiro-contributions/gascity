# Gas City — prospective provider S4 constructor (Human)

**PLAN_ONLY · GO (proposal only) · NEEDS_EVIDENCE · NOT IMPLEMENTED · NOT PUBLISHED**

**Canonical receipt:** [roadmap.md](roadmap.md) · **AI/developer source-native contract:** [constructor-sufficiency.md](constructor-sufficiency.md).

## Why this matters
Gas City can already run configurable coding agents, schedule orders/formulas and reconcile runtime configuration. A bounded hypothetical future-provider incompatibility creates a different question: can a developer plug in an independent future-oriented agent that chooses among *operator-preapproved* alternatives, safely affects the **next eligible** session, and receives the real outcome back?
Historical accepted Index: [Gas City assessment](https://github.com/opensiro/vsm-harness-index/blob/394ce776e6945115891b8f7cc459f5a7f7d7aa39/assessments/ga/gascity.md), reviewed 2026-11-18 at `03f6fe825cf0a54c677c241e4aaa7e76dade28a5`; Profile 0.2.4 / Skills 0.3.8. Original current HEAD: [187bf9a653df](https://github.com/gastownhall/gascity/commit/187bf9a653df221bd82fbee6d14ff4fcb77962a1).

| Function and plain-language role | Historical Index | Current source-native owner / feedback | Priority |
|---|---|---|---|
| **S1 · Operations** | A | [agent sessions](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/README.md) execute coding work and return bead/task results | ALREADY_A |
| **S2 · Coordination** | C | [formulas/orders](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/engdocs/architecture/orders.md) and scoped conflict preflights support developer-composed coordination | ALREADY_C |
| **S3 · Current management** | P | [controller/reconciler](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/controller.go) enforces human operator present-time choices | PARENT_P retained |
| **S3* · Independent audit** | C | separate first-party reviewer formula and synthesis return corrective findings; accepted Index is the dated anchor | ALREADY_C |
| **S4 · Prospective adaptation** | — | [provider health](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/provider_health_gate.go) and manual config support only parts, not a full autonomous future-change loop | P0: proposed C |
| **S5 · Policy and identity** | — | provider credentials, purpose and ultimate allowed choices remain with human operator | NO_TARGET |

## Proposed smallest complete user outcome
**Target transition:** S4=— -> S4=C
**Proposal-stage decision:** GO
**Research disposition:** NEEDS_EVIDENCE

**P0:** An opt-in first-party adaptation formula uses a dated future-provider compatibility signal. A developer-composed model chooses `retain / migrate / hold` *within* operator-approved providers, a narrow safe conditional config-effect port applies only to later eligible work, and the later actual session/task outcome returns to the next adaptation decision. The proposal is **not** an autonomous rewrite of city policy.

**P1:** Trust/expiry of notice, operator allowlist, concurrency and expected-config-revision checks, active-work protection, later real session receipt. **P2:** none.

## Track A / Track B
| Existing native mechanisms (A) | Proposed incremental S4 completion (B) | Stop / falsify |
|---|---|---|
| [Orders](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/engdocs/architecture/orders.md), [health gate](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/provider_health_gate.go), [provider swap](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/provider_swap.go) and manual config/reload | One opt-in future chooser + protected config-effect/return port if required | If a stock order/formula with manual or guarded native config already closes every link, do not add SDK code |
| Existing source Issues [#8419](https://github.com/gastownhall/gascity/issues/8419) and [#8367](https://github.com/gastownhall/gascity/issues/8367) are model-alias/pricing maintenance, not a request for this whole constructor | Reuse and do not duplicate them | Maintainer demand NOT_STATED; not inferred |

## Future acceptance (NOT RUN)
Compare the exact same synthetic future notice, allowed choices and next coding task in a scratch city against manual config/reload and the cheapest supported pack. Verify alternative decisions, forbidden provider/stale config/missing actor/active-session negative cases, and **actual later session feedback**, not merely successful reload. No cost, ROI or live result is claimed.

## Decision and publication
Proposal-stage **GO** follows v0.18: a source-mapped, falsifiable hypothetical design may be accepted without prior measured utility. The old generic SDK `NO_GO` remains historically preserved; this is not a claim of novel demand or a finished implementation. There is no authority to publish a public Issue/PR or modify product source.
