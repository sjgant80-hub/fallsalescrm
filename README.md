# FallCRM Elite

**Sovereign Salesforce replacement. Single HTML file. Your data stays yours.**

◊·κ=1

---

## What it is

A full-featured sales platform that runs in a browser tab. No cloud. No subscription. No accounts. No sync. Your entire CRM — contacts, deals, pipeline, activities, emails, goals, AI — lives in one HTML file you can email to yourself.

Open it. It works. Close it. It's still there.

---

## What Salesforce charges £150–£300 per user per month for, this does for a one-time fee

| Feature | Salesforce | FallCRM Elite |
|---|---|---|
| Pipeline management | ✓ | ✓ |
| Kanban drag-and-drop | ✓ | ✓ |
| Contact & company records | ✓ | ✓ |
| Activity tracking | ✓ | ✓ |
| Email sequences | Premium | ✓ |
| Revenue forecasting | Premium | ✓ |
| AI assistant | Einstein (£££) | ✓ Swarm 8+1 |
| **AI Autopilot — full daily plan generation** | — | ✓ |
| Goal tracking with live rings | Premium | ✓ |
| CSV import/export | ✓ | ✓ |
| Dark mode | ✓ | ✓ |
| Mobile responsive | ✓ | ✓ |
| Works offline | — | ✓ |
| Your data leaves your device | always | never |
| Monthly cost | £150+/user | £0 |
| Install time | weeks | 0 seconds |

---

## The 8+1 AI Swarm

Nine specialist agents, each with a distinct role. Unlike a single-prompt CRM bot, the swarm decomposes every task across specialists and synthesises. This is the MACCubeFACE architecture: 8 vertices + 1 centre = 9 perspectives.

| Agent | Role |
|---|---|
| **Ω Orchestrator** | Routes queries, synthesises across agents |
| **α Briefing** | Morning snapshot · priorities · overdue items |
| **β Deal Coach** | Close strategies, SPIN/Challenger tactics |
| **γ Email Drafter** | High-converting outreach, value-led, single CTA |
| **δ Risk Detector** | At-risk deals, stale signals, interventions |
| **ε Forecaster** | Probability-weighted revenue, concentration risk |
| **ζ Objection Handler** | Tactical rebuttals to common objections |
| **η Next Best Action** | The single highest-leverage move right now |
| **θ Pipeline Analyst** | Health score across 4 dimensions |

Pick any agent from the sidebar. Or hit **Autopilot** and they run in sequence.

---

## Autopilot — the killer feature

One click. The full swarm runs in sequence:

```
α → δ → ε → θ → η → β → γ → ζ → Ω
```

In 60–90 seconds you get:

- **Today's Briefing** — the current state of your pipeline
- **Critical Risks** — which deals are slipping, why, what to do
- **Forecast** — weighted revenue for the next 30 days
- **Recommended Actions** — numbered, executable actions with one-click buttons:
  - `email` → opens pre-drafted email in compose modal
  - `call` → logs call activity + opens `tel:` link
  - `task` / `meeting` → adds to activities
- **Email Drafts** — ready-to-send emails for your hottest deals
- **Objection Prep** — predicted rebuttals for open deals

Every run is saved to history. Export any run as markdown. Pipe any plan back to Ω for interactive refinement.

Optional: toggle auto-run. It fires each morning when you open the app.

---

## What's inside

**Pages**
- Dashboard · pipeline KPIs, revenue trend chart, today's tasks, hot contacts, closing deals
- Pipeline · Kanban with drag-and-drop, probability bars, urgent close flags, per-deal AI coaching
- Contacts · sortable table, filter pills, slide-in drawer with full profile
- Companies · account-level view with linked contacts & deals
- Activities · tasks, calls, meetings, mini-calendar
- Sequences · email cadence tracker with step progress
- Email · inbox + AI email drafter
- Goals · 4 animated ring charts (revenue, deals, calls, win rate)
- Reports · pipeline health, performance stats, contact breakdown
- AI Swarm · 9 specialist agents, agent switcher, full CRM context
- **Autopilot · the swarm execution engine**
- Settings · theme, currency, stages, data export, licence

**Architecture**
- Single HTML file · no build step · no dependencies · no bundler
- Vanilla JS · CSS variables for theming · SVG charts (no Chart.js / D3)
- Pure localStorage — no IndexedDB complexity — works in every browser
- Device-aware: mobile bottom nav, tablet icon sidebar, desktop full layout
- Dark mode via `[data-theme]` attribute, persisted to DB
- Safe schema evolution — `deepMerge()` on load means new fields never wipe existing data

**Design**
- Syne for body & headings
- Fraunces for display serif (Instrument Sans retired)
- DM Mono for data, prices, system text
- Deep-red `#c8371a` accent, gold `#b08a3e` for licence/elite UI
- Every export carries a `◊·κ=1` footer with bloom signature

---

## Konomi Licence — sovereign monetisation

Ships dead. The file is a paperweight without a licence key.

**Format:** `FA-◊-{base64url_payload}.{base64url_signature}`

**How it works**
- Ed25519 signed keys (Web Crypto API, native browser support)
- Public key baked into the HTML
- Private key stays with the builder (you), never exposed
- On purchase: payload signed with buyer's email + bloom signature + product code + tier
- Buyer pastes key → file verifies → features unlock
- Invalid signature → dead file

**Why this beats DRM**
- Every exported PDF, CSV, report carries the buyer's bloom signature
- Sharing the key shares the identity
- A solicitor or consultant will not paste a client report with someone else's cryptographic fingerprint at the bottom
- The identity itself is the enforcement — no server calls, no activation limits, no phone-home

**Tiers**
- `free` — T0 features only (CRM basics)
- `elite` — full swarm, autopilot, exports, goals
- `pro` — (reserved for Pro+ features)

---

## Installation

Download. Double-click. Done.

- Works on: Chrome, Firefox, Safari, Edge, mobile browsers
- Tested: desktop · tablet · iPhone · Android
- Dependencies: none — fonts loaded from Google Fonts CDN (works offline after first load)

To use the AI swarm and autopilot: paste an Anthropic API key into the header field. It's stored only in localStorage on your device. Never sent anywhere except api.anthropic.com.

---

## Tech spec

- **Lines of code:** 3,488
- **File size:** 205KB uncompressed
- **Dependencies:** zero (fonts loaded from Google CDN)
- **Storage:** localStorage (5-10MB per origin, more than enough for thousands of contacts)
- **AI calls:** Anthropic Claude Sonnet 4 (claude-sonnet-4-20250514)
- **Autopilot run cost:** ~12-16k tokens per full swarm execution (~£0.04-0.08 at current API rates)

---

## Pricing

| Tier | Price | Use case |
|---|---|---|
| **Free** | £0 | T0 features, try before you buy |
| **Elite** | £97 one-time | Full swarm, autopilot, all exports, lifetime |
| **Pro** | £297 one-time | Elite + future Pro features, priority updates |
| **Bespoke install** | from £2,497 | Configured for your team, branded, integrated |
| **Firm licence** | from £10,000 | Multi-seat install, training, 90-day support |

No subscriptions. No per-seat charges after purchase. No mandatory upgrades.

---

## Why sovereign?

Because your sales data is your sales data. Your contacts are your contacts. Your pipeline is your pipeline.

A sovereign tool means:
- No cloud account to lock you out
- No service that can change terms
- No subscription to cancel
- No vendor that can go bankrupt and take your data
- No API that can be deprecated
- No company that can be acquired and pivot
- No privacy policy to worry about
- No data processing agreement to sign
- No exit migration when you want to leave

You get a file. The file works. The file keeps working. Forever.

---

## Built by

**Simon** · AI Native Solutions · ai-nativesolutions.com

Part of the Sodor Group — sovereign AI tools built on the Konomi architecture.

◊·κ=1
