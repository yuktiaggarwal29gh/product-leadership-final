# Outcome Roadmap & Trade-off Memo: Meridian

> Module 2 · Prioritization & Roadmapping for Product Leaders, ★ Deliverable 2
>
> Translate your strategy into a multi-team, outcome-driven roadmap, and a memo defending the hard prioritization calls behind it.

## 1. Outcome roadmap

_A multi-team roadmap organized by **outcomes**, not feature lists. Show how near-term revenue pressure is balanced against long-term platform bets._

| Horizon | Outcome / bet | Owning team(s) | Success signal |
|---|---|---|---|
| **Now (0 to 3 mo)** | We bet simplifying the daily log (14→4 fields), shipping a dedicated foreman-facing mobile app, and reliable offline capture/sync will make Meridian the default field-documentation tool over camera + group text | Mobile/Field Product, Field Engineering, Design | Field DAU rises from 12% baseline toward 55% target; time-to-first-log on new sites drops |
| **Next (3 to 6 mo)** | We bet validating whether compliance-checklist automation drives retention, fixing the broken Procore integration, adding schedule-change push notifications, and instrumenting field-adoption cohort tracking will protect enterprise trust while confirming field adoption is translating into retention | Enterprise Product, Integrations Eng, Data/Analytics | Procore-affected accounts stabilize; cohort data shows early correlation between field adoption and retention; compliance-checklist decision made (build/defer) |
| **Later (6 to 12 mo)** | We bet that once field adoption is proven, selectively investing in enterprise-expansion plays (exec reporting, subcontractor portal) and adjacent capabilities (AI-assisted RFI drafting, time-tracking, web UI refresh) can extend value — but only where field data supports it | Enterprise Product, Platform, Growth | Mid-market churn trending from 22% toward 10%; any Later item greenlit only with field-adoption or retention data backing it, not commercial pressure alone |


# Meridian — Now / Next / Later Roadmap

**Frame:** Outcome bets, not delivery milestones. Everything ladders to: *make Meridian indispensable to the field without eroding enterprise depth.*

---

## 🔵 NOW (max 3 — this quarter's strategic bets)

| # | Bet | Linked OKR |
|---|-----|-----------|
| 1 | We bet simplifying the daily log from 14 required fields to 4 will make Meridian faster to use than a phone camera and group text for field superintendents and foremen. | KR1 — field DAU 12%→55% |
| 2 | We bet a dedicated foreman-facing mobile experience, built independently of the PM web app, will make field teams choose Meridian as their default tool instead of a workaround. | KR1 — field DAU 12%→55% |
| 3 | We bet reliable offline capture and sync will remove connectivity as a reason field teams abandon Meridian on active job sites. | KR1 — field DAU 12%→55% (enabling bet underneath #1 and #2) |

*Note: all three Now bets serve KR1 by design — it's the leading indicator; KR2 and KR3 are lagging validations of whether KR1 actually mattered.*

---

## 🟡 NEXT (max 5 — queued, not started)

| # | Item | Why it waits |
|---|------|---------------|
| 1 | Validate whether compliance-checklist automation (item #5) is a retention driver or a sales chip | Needs a deliberate proven-vs-prospective call before it can be scored as Rock or Hard No |
| 2 | Fix the Procore integration break affecting 2 existing clients | Real churn-risk protection (KR2 guardrail), but remediation not a bet — sequenced after field bets prove out, unless client risk escalates |
| 3 | Push notifications for schedule changes (item #11) | Genuine field-adoption lever, but smaller than the three Now bets — natural fast-follow once the foreman app ships |
| 4 | Instrument and launch field-adoption cohort tracking (retention-by-cohort) | Can't meaningfully measure this until Now bets are live long enough to generate cohort data |
| 5 | Data model migration for multi-project dashboards (item #3, tech debt) | Enabling infrastructure, not itself an outcome — only worth funding once it's blocking a Now/Next bet directly |

---

## ⚪ LATER (bets, not commitments — right direction, not yet resourceable)

- **Executive reporting dashboard with custom KPIs** (item #10) — real commercial pressure (2 renewals at risk), but scores zero on field adoption; revisit only if KR2 shows genuine strain, not because renewal pressure resurfaces
- **Subcontractor portal with document sharing** (item #14) — plausible enterprise-expansion play, outside current core use case
- **Time-tracking module** (item #12) — scope expansion beyond documentation/coordination; revisit only if field-adoption data shows it's genuinely adjacent
- **AI-assisted RFI drafting** (item #9) — consistent with "AI as accelerator, not moat"; worth exploring once core field capture is proven
- **Web UI refresh** (item #13) — cosmetic/buyer-facing; no field-adoption case for prioritizing it this year

---

**Flag worth keeping in view:** nothing in Now or Next actively *builds* toward KR3 (mid-market churn 22%→10%) beyond hoping KR1 causes it. The falsification trigger says to question the assumption if field adoption improves without retention improvement after two quarters — worth deciding now what data in Next will catch that early.

## 2. Trade-off memo

_What did you sequence first, what did you push out, and what did you cut entirely, and why? Use WSJF / cost of delay reasoning where it helps._

> I chose to sequence … first because …
>
> I pushed out … because …
>
> I cut … entirely because …

## Link to full artifact

_[link to this deliverable in your repo]_
