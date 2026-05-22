# Yuxin-Qiao

## Open-source

### CodexBar

I contribute to [steipete/CodexBar](https://github.com/steipete/CodexBar), focusing on AI coding-provider usage, quota, billing, subscription visibility, and menu-bar UX.

**Merged PRs**
- [#970](https://github.com/steipete/CodexBar/pull/970) — MiniMax Token Plan quota support: fixed remaining/used mapping, added 5-hour + weekly quota display, filtered invalid quota placeholder rows, and added regression tests.
- [#1083](https://github.com/steipete/CodexBar/pull/1083) — MiniMax coding-plan title propagation tests: verified real plan names flow from parser output into the shared menu model without fake fallback labels.
- [#1089](https://github.com/steipete/CodexBar/pull/1089) — MiniMax billing-history failed-record filtering: excluded explicitly failed billing records from local token totals, charts, and model/method aggregation.
- [#1099](https://github.com/steipete/CodexBar/pull/1099) — OpenCode renewal-date visibility: preserves `renewAt` / `renew_at` as `renewsAt` and surfaces it via `NamedRateWindow(title: "Renews")`; provider-specific, no new API calls.
- [#1100](https://github.com/steipete/CodexBar/pull/1100) — Kimi primary-only icon progress regression coverage: test-only PR using pixel inspection to prove the Kimi primary progress bar renders when `secondary` is nil. Refs [#1043](https://github.com/steipete/CodexBar/issues/1043).
- [#1101](https://github.com/steipete/CodexBar/pull/1101) — UsageStore snapshot preservation for network failures: preserved last successful quota snapshots for additional URL transport failures and added regression coverage. Fixes [#1097](https://github.com/steipete/CodexBar/issues/1097).

**Proposal / design reference**
- [#1007](https://github.com/steipete/CodexBar/issues/1007) — MiniMax billing-history token usage summary proposal: local aggregation design for today / last-30-days token usage, method/model breakdowns, and web-session-only fallback without persisting raw billing rows.


---

## 开源

### CodexBar

我持续参与 [steipete/CodexBar](https://github.com/steipete/CodexBar)，主要关注 AI coding provider 的用量、额度、账单、订阅周期可视化和菜单栏体验。

**已合并 PR**
- [#970](https://github.com/steipete/CodexBar/pull/970) — MiniMax Token Plan 额度支持：修正 remaining/used 映射，增加 5 小时 + weekly 额度展示，过滤无效 quota placeholder，并补充回归测试。
- [#1083](https://github.com/steipete/CodexBar/pull/1083) — MiniMax coding-plan title 传递测试：验证真实 plan name 能从 parser 传递到 shared menu model，且不会生成虚假 fallback label。
- [#1089](https://github.com/steipete/CodexBar/pull/1089) — MiniMax billing-history failed-record 过滤：将明确失败的 billing 记录排除在 token totals、charts、model/method 聚合之外。
- [#1099](https://github.com/steipete/CodexBar/pull/1099) — OpenCode renewal date 可视化：保留 `renewAt` / `renew_at` 为 `renewsAt`，并通过 `NamedRateWindow(title: "Renews")` 展示；provider-specific，不新增 API 调用。
- [#1100](https://github.com/steipete/CodexBar/pull/1100) — Kimi primary-only icon progress 回归测试：纯测试 PR，使用 pixel inspection 证明只有 `primary`、没有 `secondary` 时 Kimi 主进度条仍会渲染。对应 [#1043](https://github.com/steipete/CodexBar/issues/1043)。
- [#1101](https://github.com/steipete/CodexBar/pull/1101) — UsageStore 网络失败时保留 snapshot：为更多 URL transport failure 保留最后一次成功的 quota snapshot，并补充回归测试。修复 [#1097](https://github.com/steipete/CodexBar/issues/1097)。

**提案 / 设计参考**
- [#1007](https://github.com/steipete/CodexBar/issues/1007) — MiniMax billing-history token usage summary 提案：设计本地聚合今日 / 近 30 天 token 用量、method/model breakdown 和 web-session-only fallback，且不持久化原始账单行。
