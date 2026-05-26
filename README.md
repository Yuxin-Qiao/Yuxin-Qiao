# Yuxin Qiao

Software engineer and open-source contributor interested in AI developer tools, coding agents, and developer productivity.

I like building small, reliable tools that make complex developer workflows easier to understand, debug, and trust.

## Open-source focus

I contribute to [steipete/CodexBar](https://github.com/steipete/CodexBar), focusing on AI coding-provider usage, quota visibility, billing semantics, subscription visibility, diagnostics, and menu-bar UX.

My recent work has focused on making provider data more understandable and reliable, especially around MiniMax usage, quota reporting, reset timing, billing records, and provider metadata.

## Selected contributions

### MiniMax provider support

- Added and improved MiniMax token-plan quota visibility.
- Improved remaining / used quota mapping.
- Added support for displaying both 5-hour and weekly quota windows.
- Filtered invalid quota placeholder rows.
- Added regression tests for provider usage parsing.

### Billing and usage semantics

- Improved billing-history handling by filtering explicitly failed billing records.
- Helped keep local token totals, charts, and method / model aggregation aligned with valid billing data.
- Worked on clearer separation between quota reset timing, renewal timing, and subscription-related semantics.

### Provider metadata and diagnostics

- Added tests for MiniMax plan-title propagation.
- Verified real provider plan names flow through parser output into the shared menu model.
- Worked on diagnostic and redaction-related improvements so debugging output stays useful without exposing sensitive data.

### Menu-bar UX and reliability

- Improved how AI coding-provider usage is represented in the menu bar.
- Added focused tests around real-world provider edge cases.
- Contributed small, reviewable fixes aimed at making CodexBar more trustworthy for daily use.

## What I like building

- AI coding workflow integrations
- CLI and menu-bar developer tools
- Provider usage and quota visibility
- Privacy-aware diagnostics
- Tests for messy real-world API and billing data
- Small product improvements with clear user value

## Tech interests

- Java / backend engineering
- Swift / macOS apps
- TypeScript / scripting / CLI tooling
- AI coding agents
- Developer productivity tools
- Open-source infrastructure

## Currently

Building and contributing to open-source projects around AI developer tooling.

Open to software engineering opportunities.
