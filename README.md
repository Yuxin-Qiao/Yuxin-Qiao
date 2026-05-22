# Yuxin-Qiao

## Open-source

### CodexBar

I contribute to [steipete/CodexBar](https://github.com/steipete/CodexBar), with a focus on AI coding-provider usage, quota, billing, subscription visibility, and menu-bar UX.

#### Merged PRs

- [steipete/CodexBar#970](https://github.com/steipete/CodexBar/pull/970) — MiniMax Token Plan quota support
  - Fixed remaining-vs-used quota mapping
  - Added 5-hour and weekly quota display for MiniMax token plans
  - Filtered invalid quota placeholder rows
  - Added MiniMax regression tests

- [steipete/CodexBar#1083](https://github.com/steipete/CodexBar/pull/1083) — MiniMax coding-plan title propagation tests
  - Added focused tests ensuring provider plan names flow from parser output into the shared menu model
  - Verified missing MiniMax plan metadata does not create fake fallback labels
  - Test-only contribution with no production behavior change

- [steipete/CodexBar#1089](https://github.com/steipete/CodexBar/pull/1089) — MiniMax billing-history failed-record filtering
  - Filtered explicitly failed MiniMax billing-history records out of local aggregation
  - Preserved backward compatibility for older or partial billing payloads
  - Added regression coverage for token totals, charts, and model/method breakdowns

#### Open PRs / In review

- [steipete/CodexBar#1099](https://github.com/steipete/CodexBar/pull/1099) — OpenCode renewal-date visibility
  - Preserves OpenCode/OpenCodeGo `renewAt` / `renew_at` as `renewsAt`
  - Surfaces renewal timing through `NamedRateWindow(title: "Renews")`
  - Provider-specific; no new API calls or shared lifecycle model

- [steipete/CodexBar#1100](https://github.com/steipete/CodexBar/pull/1100) — Kimi primary-only icon progress regression coverage
  - Adds a regression test for Kimi icon progress rendering when `UsageSnapshot.primary` exists and `secondary` is nil
  - Uses pixel inspection to prove the rendered primary Kimi bar is present
  - Refs issue #1043

#### Proposal / design reference

- [steipete/CodexBar#1007](https://github.com/steipete/CodexBar/issues/1007) — MiniMax billing-history token usage summary proposal
  - Proposed local billing-history aggregation for token usage summaries
  - Covered today / last-30-days token usage, method/model breakdowns, and web-session-only fallback design
  - Avoided raw billing-row persistence and sensitive account-field display

---

## 开源

### CodexBar

我正在持续参与 [steipete/CodexBar](https://github.com/steipete/CodexBar)，主要关注 AI coding provider 的用量、额度、账单、订阅周期可视化以及菜单栏体验。

#### 已合并 PR

- [steipete/CodexBar#970](https://github.com/steipete/CodexBar/pull/970) — MiniMax Token Plan 额度支持
  - 修正 remaining / used 额度映射
  - 增加 MiniMax Token Plan 的 5 小时 / weekly 额度展示
  - 过滤无效 quota placeholder 行
  - 增加 MiniMax 回归测试

- [steipete/CodexBar#1083](https://github.com/steipete/CodexBar/pull/1083) — MiniMax coding-plan title 传递测试
  - 增加测试，确保 provider 返回的真实 plan name 能从 parser 传递到 shared menu model
  - 验证缺失 plan metadata 时不会生成虚假的 fallback label
  - 纯测试型贡献，不改变生产逻辑

- [steipete/CodexBar#1089](https://github.com/steipete/CodexBar/pull/1089) — MiniMax billing-history failed records 过滤
  - 将明确失败的 MiniMax billing-history 记录排除在本地聚合之外
  - 保留对旧版或部分 billing payload 的兼容性
  - 增加 token totals、charts、model/method breakdown 的回归覆盖

#### 审阅中的 PR

- [steipete/CodexBar#1099](https://github.com/steipete/CodexBar/pull/1099) — OpenCode renewal date 可视化
  - 保留 OpenCode/OpenCodeGo 的 `renewAt` / `renew_at` 字段为 `renewsAt`
  - 通过 `NamedRateWindow(title: "Renews")` 展示续费/到期时间
  - provider-specific，不新增 API 调用，不引入共享 subscription lifecycle model

- [steipete/CodexBar#1100](https://github.com/steipete/CodexBar/pull/1100) — Kimi primary-only icon progress 回归测试
  - 增加 Kimi 在只有 `UsageSnapshot.primary`、没有 `secondary` 时仍能渲染菜单栏进度条的测试
  - 使用 pixel inspection 证明 primary Kimi bar 实际被渲染
  - 对应 issue #1043

#### 提案 / 设计参考

- [steipete/CodexBar#1007](https://github.com/steipete/CodexBar/issues/1007) — MiniMax billing-history token usage summary 提案
  - 提出本地 billing-history 聚合，用于 token usage summary
  - 覆盖今日 / 近 30 天 token 用量、method/model breakdown，以及 web-session-only fallback 设计
  - 不持久化原始账单行，不展示敏感账号字段
