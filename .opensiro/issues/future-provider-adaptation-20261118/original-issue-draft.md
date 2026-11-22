# Proposal: optional future-provider adaptation for Gas City orders — Opensiro VSM architecture review

## Proposal in the project's own terms

**What exists today:** Gas City already has [orders and formula dispatch](https://github.com/gastownhall/gascity/blob/f4627bc5a305450b2cb93967ae631324c9a9ce22/cmd/gc/order_dispatch.go), [provider-health checks](https://github.com/gastownhall/gascity/blob/f4627bc5a305450b2cb93967ae631324c9a9ce22/cmd/gc/provider_health_gate.go), [provider switching](https://github.com/gastownhall/gascity/blob/f4627bc5a305450b2cb93967ae631324c9a9ce22/cmd/gc/provider_swap.go) and normal operator-driven configuration/reload paths. These solve current operational problems; they do not automatically demonstrate an agent-owned decision about a *future* provider change.

**What may be missing:** An optional, source-native way for a bounded formula or pack to consider a dated future provider/model change, compare allowed choices, recommend retain/migrate/hold, and confirm the outcome of a **subsequent** agent session after a lawful operator-approved change. This is a construction hypothesis, not a reported defect.

**Closest existing project-native solution:** The operator watches announcements, chooses an approved provider, applies normal config/reload, and checks a later agent run. Existing orders and custom packs may already make further core changes unnecessary.

**Existing discussion:** [#8419](https://github.com/gastownhall/gascity/issues/8419) is an **open** model-alias choice with a human follow-up, not this future-choice/feedback loop. Pricing issue [#8367](https://github.com/gastownhall/gascity/issues/8367) was **closed on 2026-11-21**, so it is not cited as an outstanding need. [PR #9275](https://github.com/gastownhall/gascity/pull/9275) is an **open, unmerged** proposal for revision-guarded singleton-agent provider overrides and later `session.woke` provider/model feedback; it could supply important native building blocks, but it is not shipped at the observed source HEAD. Please prefer or reuse this work where appropriate.

The requested conversation is about architecture fit, not permission to implement without maintainer review.

## How we reached this proposal — Opensiro VSM assessment

Opensiro applies Stafford Beer's Viable System Model (VSM) to ask which *agent* owns an organizational decision and its feedback, not to grade a project's quality or the human maintainer organization.

**Historical assessment:** [accepted Opensiro Index record](https://github.com/opensiro/vsm-harness-index/blob/a3fcf7c156ef4d1132680890bc11544681fd30c0/assessments/ga/gascity.md), accepted Index commit `a3fcf7c156ef4d1132680890bc11544681fd30c0`; accepted assessment blob `91478bc006342a6f92f41e3670d5708e50592da1`; accepted review ref `03f6fe825cf0a54c677c241e4aaa7e76dade28a5`; reviewed 2026-11-18; Profile `0.2.4`, Skills methodology `0.3.8`.

**Boundary:** First-party installed Gas City runtime and bundled core pack, provider/session/reconciler/orders paths. Third-party packs, individual model vendors, human operator policy and OpenSiro's own organization are outside this assessment.

**Current original HEAD:** [main@f4627bc5a305450b2cb93967ae631324c9a9ce22](https://github.com/gastownhall/gascity/commit/f4627bc5a305450b2cb93967ae631324c9a9ce22), observed on 2026-11-22. This is 31 commits after the case research reference `e6e47235027b758b9a86b0ddb99fb5d3a69c59e4`. In that range we inspected the changed-file list and relevant provider/config/formula changes; unchanged provider health/swap/order dispatch paths were rechecked. This does **not** constitute a new accepted Index assessment.

| Function / plain-language role | Historical Index state | Current source-backed boundary |
| --- | --- | --- |
| **S1 · Operations** | Agents do work | A | Worker sessions perform tasks and return task results |
| **S2 · Coordination** | Avoid interference | C | Optional workflow/preflight compositions can coordinate scoped work |
| **S3 · Current management** | Regulate active commitments | P | The operator retains current city intervention authority; controller and reconciler enforce commands |
| **S3* · Independent review** | Return corrective evidence | C | Configured review/quorum paths can return findings |
| **S4 · Future adaptation** | Anticipate external change | — | No complete first-party future-provider choice/effect/feedback loop was established |
| **S5 · Identity/policy** | Ultimate authority | — | Human operator/provider credentials remain outside the agent-ownership boundary |

**States:** `A` = autonomous agent-owned decision and feedback; `C` = developer-composable first-party function path; `P` = supported parent-governed S3–S5 ownership; `A(P)` / `C(P)` = independently evidenced accompanying parent mode; `—` = no material first-party path established in the *historical* boundary; `?` = unresolved evidence. These are ownership categories, **not quality ranks**, and historical `—` does not make Gas City defective.

## Why this particular construction?

**Whole-repository prioritization:** A six-function source review selected a bounded S4 prospective provider-choice question, rather than a general new manager or changes to already assessed S1/S2/S3/S3* paths. Maintainer interest is NOT_STATED.

**Construction hypothesis:** Historical `S4=— -> S4=C`: a developer could optionally compose a future-provider adaptation actor that makes a source-backed retain/migrate/hold choice within operator-set limits and learns from later, real session feedback. This is *not implemented* or an Index regrade.

**Native building blocks:** Existing order/formula engine, provider-health checks, provider swap, configuration/reload and session result records. Proposed PR #9275 could add a safer revision-guarded scoped override and explicit provider/model event, but is not available in default-branch code yet.

**Minimal proposed addition:** Prefer an example or pack using existing primitives. Add a narrowly scoped first-party connection only if it is demonstrated that a legitimate future-choice proposal cannot be applied safely and correlated with the actual next-run result using the current public interfaces.

**Scope exclusions:** No autonomous credential changes, general provider registry rewrite, default self-upgrading, overriding operator permissions or editing the configuration of a currently running session.

## Proposed approach and validation

1. A formula or opt-in component receives a dated provider/model change notice and checks approved alternatives.
2. A developer-composed actor may recommend retain/migrate/hold with evidence, but the operator must authorize any configuration change. Existing safe config/reload interfaces should remain authoritative.
3. Record which provider/model a **later** session actually used, and its result; use that evidence on the next recommendation. If open PR #9275 or existing APIs already provide the effect/return path, reuse those paths instead of introducing another one.

**Hypothesized benefit:** Better prospective maintenance of an operator's recurring agent work. No user demand, native test success, safety improvement or cost reduction has been measured.

**How to falsify:** Existing orders/packs/configuration and run metadata already permit the complete lawful future-choice-to-outcome loop; or no safe conditional configuration effect can be established. Either result would make this addition unnecessary or invalid.

**Cost status:** NOT_MEASURED. A future matched scenario should compare manual provider change with a hypothetical assisted change, including engineering, review, migration, testing and maintenance effort. Native tests are NOT_RUN.

## Feedback requested

**Would a small example/pack plus current (or PR #9275's proposed) config and session feedback surfaces be sufficient for this future-provider scenario?** If so, no new first-party core interface is warranted. If there is a real missing link, which protected operation or return signal would it be? This is a request for maintainer design feedback, not a commitment to send a PR.

## Three independent ways to participate

- **Gas City:** Prefer current native behavior and the maintainer's roadmap; consider a narrow addition only if it fits.
- **VSM methodology:** Challenge the function mapping through [Opensiro Profile](https://github.com/opensiro/vsm-harness-profile) or [Skills](https://github.com/opensiro/vsm-harness-skills).
- **Independent experiment:** Explore the hypothesis in a permitted private/domain fork or optional pack without requiring Gas City adoption.

## Research attribution and AI disclosure

[Opensiro Upstream](https://github.com/opensiro/upstream) · [source-pinned Gas City case](https://github.com/opensiro-contributions/gascity/blob/3eed2db60462208bb80952aecaf6a88a341ddbe4/.opensiro/issues/future-provider-adaptation-20261118/roadmap.md)

**AI involvement:** AI assistance was used to review sources and draft this proposal. No shipped constructor, independent native test result, current Index regrade, measured benefit or maintainer endorsement is claimed.
