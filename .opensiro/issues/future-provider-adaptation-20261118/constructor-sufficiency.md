# Gas City — S4 constructor sufficiency contract (AI/developer)

**Canonical receipt:** [roadmap.md](roadmap.md) · **Human:** [issue.md](issue.md). This is source-only plan, not an implementation or test certification.

**Target transition:** S4=— -> S4=C
**Proposal-stage decision:** GO
**Research disposition:** NEEDS_EVIDENCE

## Scope and competing owners
Original [HEAD](https://github.com/gastownhall/gascity/commit/187bf9a653df221bd82fbee6d14ff4fcb77962a1); [accepted Index](https://github.com/opensiro/vsm-harness-index/blob/394ce776e6945115891b8f7cc459f5a7f7d7aa39/assessments/ga/gascity.md). Full six-function historical/current matrix is rendered only in Human [issue.md](issue.md) and receipt. Coding agents are S1; composer-owned conflict/review formulas already support S2/S3*. The human operator is current S3/P and holds policy/allowed providers, not delegated to the proposed S4 actor.

## Track A: shipped source / original work
1. [Order architecture](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/engdocs/architecture/orders.md): supported cron/event/condition `order.toml` can dispatch exec or agent formula; order history/tracking is not a prospective decision.
2. [Provider health gate](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/provider_health_gate.go): one current health snapshot per tick, read from an optional watcher-written file. Stale/unreadable entries fail open; gate/alert is reactive S3 machinery, not proof of future S4.
3. [Provider swap](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/provider_swap.go), [config CLI](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/cmd_config.go) and [drift deferral](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/cmd/gc/config_drift_episode.go): runtime effect, inspection and active-work safety exist. The `gc config` command currently offers show/explain, not a complete conditional agent-written patch + authoritative post-session evidence contract.
4. [#8419](https://github.com/gastownhall/gascity/issues/8419), [#8367](https://github.com/gastownhall/gascity/issues/8367): present maintainer feature/bug scope; do not duplicate. [Maintainer roadmap](https://github.com/gastownhall/gascity/blob/187bf9a653df221bd82fbee6d14ff4fcb77962a1/ROADMAP.md) names reliability/performance/onboarding. No evidenced request for this S4 actor.

## Track B: minimum function-specific C chain (all proposed)
| Link | First-party candidate atop A | Falsifier |
|---|---|---|
| Future sensing | Versioned signed/attributed effective-at compatibility notice; optional adapter, TTL and support confidence separate from present health | Only current outage/429 and no forward evidence |
| Options | Immutable retain/migrate/hold candidate set intersected with operator allowlist and provider compatibility; forbidden candidate never enters decision | Actor expands parent permission |
| Autonomous decision | Developer-composed model agent in first-party supported formula chooses one of >=2 lawful options with reason and stable choice key | deterministic order/host script already gives identical legitimate choices |
| Safe effect | Narrow opt-in conditional provider config patch (expected revision, authorized affected agents and safe work fences), existing controller observes config and reconciles next eligible session | Existing config editor already provides same atomic conditions; then no new code |
| Real feedback | Capture identity/provider/actual task result of later session and return it to the actor for next choice; fail/hold and no false completion on reload-only ack | Only file write/reload ack, no actual task result |

## Implementation minimum and boundaries
P0 is *not* a new generic controller. Start with a source-native opt-in pack/formula on a disposable scratch city. If the stock pack/manual mechanism cannot safely commit a developer-composed choice, specify just one conditional config application + later-session feedback port; do not create another scheduled worker or policy/S5 engine. P1 adds evidence, allowed options, config-version check, lifecycle enforcement and native tests. No P2.

## Future native tests (all NOT_RUN)
Positive: a dated synthetic future notice with two allowed providers yields one actor-selected option, guarded safe apply, later session with that provider and actual result returned. Alternative: no need to migrate yields retain/hold. Negative: absent actor, stale/forged notice, forbidden provider, concurrent human config change, in-flight work, failed launch and missing later-result acknowledgement must never report success or escalate rights. Compatibility: default absent-opt-in must follow stock code paths. Baselines: stock operator edit/reload and supported order/script/pack, same task and evidence; measure implementation/maintenance effort, success and human interventions.

## Scope conclusion and historic comparison
Current-source proposal GO with NEEDS_EVIDENCE is compatible with v0.18 proposal-stage rules and does not assert a new production capability. Earlier fork case (2026-11-18) was NO_GO on *new generic S4 SDK/controller*, with a native-first feasibility plan; our narrower optional constructor uses the same family of scenario, so novelty/actual demand is not claimed. Overlap may falsify need for a new core port. No native tests, GitHub publication, original maintainer approval or Index regrade.
