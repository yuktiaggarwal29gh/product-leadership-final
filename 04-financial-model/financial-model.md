# Financial Model: Meridian

> Module 5 · Master Product Financials & Strategic Bets, ★ Deliverable 5
>
> The business case for funding your bet, and the explicit kill criteria that would tell you to stop.

## Make your evaluation and funding decision
- **What assumption is doing the most work? If this number is 20-30% off, what changes?:** The upsell-rate improvement (6%→8%) is doing all the work — it’s the sole driver of the $896K return. But more importantly, even at face value this number hides a bigger problem than being “20-30% off”: it conflates causation with attribution (see structural issue below). If the 8% target is 20-30% optimistic (i.e., real improvement lands closer to 6.5%-7%), the incremental upsell count shrinks from 8 accounts to roughly 2-4, and the payback case weakens dramatically.
- **What is the structural problem in this case? Look past the headline numbers for something that does not hold up on closer inspection.:** The $896,000 return figure is calculated by multiplying all 32 upsells at 8% by $28,000 — but 24 of those 32 accounts would have upgraded anyway at the 6% baseline rate. Only the incremental upsells (8% minus 6% = 2%, or 8 accounts) can actually be attributed to the AI feature. Recalculated correctly: 8 incremental upsells × $28,000 = $224,000 incremental ARR, not $896,000. That changes payback from the claimed 2.4 months to ~9.6 months ($180,000 ÷ $224,000 annualized) — still positive, but four times weaker than the case presents, and it silently drops the Enterprise churn rate (12%) entirely, which should discount even that $224K further since some of those upsold accounts will churn within the year.
- **Is the kill criterion complete and actionable? Does it name the consequence, or hand the decision back to the room?:** It’s mostly complete — it names the metric (Standard-to-Enterprise upsell rate), the threshold (7%), the timeline (end of Q3), and a concrete consequence (pause the feature, reallocate Q4 capacity before headcount is committed). That’s a real kill switch, not a vague “we’ll reassess.” One gap: it doesn’t say what happens to the $180K already spent, or whether partial credit toward the 7% threshold changes the decision — worth tightening if this were a live case.
- **Your verdict: FUND / FUND WITH ONE CONDITION / DO NOT FUND. If a condition, name it; otherwise explain in one sentence.:** FUND WITH ONE CONDITION — correct the ARR model to count only incremental upsells above the 6% baseline before final approval; the corrected ~9.6-month payback is still a reasonable bet, but the team needs to sign off on the real number, not the inflated one.

## Write your business case
- **The strategic bet. What specific outcome are you backing, who does it serve, and what is the mechanism that connects the product decision to a financial result?:** Meridian builds reliable offline-first capture and sync for the field-adoption mobile app, serving superintendents and foremen working on job sites with poor or no connectivity. The mechanism: connectivity failures are a primary reason field teams default to their phone camera and group texts instead of Meridian — if the app can’t reliably capture and sync data offline, no amount of UX simplification (daily-log fields, foreman app) will drive adoption, because the tool fails at the moment it’s needed most. This is the dependency underneath KR1 (field DAU 12%→55%).
- **The assumptions. List the assumptions your case rests on, then rank them: which one, if wrong, most changes your conclusion?:** 1.	Offline reliability is the primary adoption blocker, not just a contributing factor — if connectivity issues are actually secondary to UX friction (e.g., too many form fields), fixing offline sync alone won’t move field DAU much, and the daily-log simplification (Rock #3) may matter more than this bet assumes.
	2.	Field DAU baseline of 12% and target of 55% — if the true current baseline is meaningfully lower (say 5%), the mechanism connecting offline capability to adoption may need a longer timeline or a different primary lever.
	3.	$1.2M investment estimate for the build — a standard SaaS-style estimate; if offline-first sync proves more technically complex on this platform than assumed (e.g., legacy data model conflicts), cost and timeline could expand significantly.
- **The expected return. What does the bet generate and when? Express it at unit level (per customer) and at scale (what volume hits target).:** •	Per customer: an average mid-market GC account ($5M–$50M) generates ~$14K ACV; if offline reliability converts a churn-risk account into a retained one, that’s $14K in retained ARR per account, compounding via 3-year average retention (LTV ~$42,000).
	•	At scale: hitting 25% field DAU by month 6 (the kill-criterion checkpoint) implies enough of the 400 Standard/mid-market accounts are actively engaging that mid-market churn (22%→10% target) starts moving measurably; full realization at 55% field DAU is the 12-month target tied to the broader KR1 OKR
- **The kill criterion. Name the specific metric, threshold, timeline, and financial consequence that tells the team to stop. Actionable, not a conversation.:** If field DAU does not reach 25% of active field users by month 6, we will pause further offline-sync engineering investment and reallocate Q3 capacity to re-diagnose whether the adoption blocker is connectivity-related or UX-related (e.g., daily-log complexity), before committing further headcount to this specific bet.

## Stress-test and finalize
- **Paste your finalized business case here.:** Business Use Case: Offline Reliability for Field Users

Business Problem

Field users often work in low-connectivity environments. When the product cannot reliably support offline work, daily engagement suffers and creates a retention risk for mid-market General Contractor (GC) accounts.

Business Bet

Invest in offline-sync reliability to increase field adoption and engagement, with the expectation that sustained adoption will contribute to reducing mid-market churn.

Expected Return

* Per customer: An average mid-market GC account ($5M–$50M) generates approximately $14K ACV. Retaining one churn-risk account protects approximately $14K in annual recurring revenue (ARR), with a 3-year average retention implying approximately $42K in LTV per retained account.
* At scale: There are approximately 400 Standard/mid-market accounts, representing roughly $5.6M in annual ACV at the $14K average.
* Retention upside: Reducing mid-market churn from 22% to 10% represents a 12-percentage-point improvement. Applied across 400 accounts, this equates to approximately 48 additional retained accounts, or ~$672K in retained ARR annually and approximately $2.0M in 3-year LTV.
* Downside case: Even a more modest reduction in churn from 22% to 16% would retain approximately 24 additional accounts, protecting ~$336K in ARR annually.

Adoption Milestones

* Month 6: Reach 25% field DAU across active field users within the target Standard/mid-market accounts. This is the checkpoint for determining whether offline reliability is solving a meaningful adoption barrier.
* Month 12: Reach 55% field DAU, aligned to the broader KR1 objective and expected to provide sufficient adoption to assess measurable movement in mid-market churn.

Load-Bearing Assumption

The critical assumption is that connectivity-related reliability is a meaningful barrier to field adoption and that increased, sustained field usage from offline reliability will contribute to improved account retention.

The month-6 adoption milestone is therefore treated as an early validation signal—not as proof by itself that churn will decline.

Investment & Payback

The initiative should proceed only with a defined incremental engineering investment. Payback will be evaluated against the expected retained ARR:

Estimated payback period = Incremental offline-sync investment ÷ expected annual retained ARR

At the target churn improvement from 22% to 10%, the expected annual retained ARR is approximately $672K.

Kill Criterion

If field DAU does not reach 25% of active field users by month 6, we will pause further offline-sync engineering investment and reallocate Q3 capacity to re-diagnose whether the adoption blocker is connectivity-related or UX-related (for example, daily-log complexity) before committing additional headcount to this specific bet.

Decision

This is a conditional investment: proceed with offline-sync engineering, measure adoption at month 6, and continue investment only if the 25% field-DAU threshold is achieved. The potential upside is meaningful, with approximately $672K in annual retained ARR at the target churn reduction, while the explicit kill criterion limits continued investment if the core adoption hypothesis is not supported.

