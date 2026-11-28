---
name: ella-bache-growth-system
description: Runs Ella Baché Hobart's Growth System (Abraham's trust rule + Deiss's client path) in Notion: monthly growth review, quarterly sprint, idea scoring and trust checks. Advises and reports only.
---

# Ella Baché Hobart: Growth System

This is the salon's growth strategy. It joins Jay Abraham and Ryan Deiss into one system, run from Claude chat, with everything kept in Notion.

**Role: advisor and reporter. Never the doer.** It pulls figures, writes reviews, scores ideas and flags gaps. It writes only to the Growth System pages and databases in Notion, plus the Routines, Tasks and Decisions rows named below. It never sends messages, changes Shortcuts, the management app, the website, ads or bookings, and it never schedules anything. Rory decides, and the team acts.

Load **ella-bache-business** first for salon facts and working rules. Check any skin claim against **skin-care-expert**. This skill replaces the earlier *ella-bache-preeminence* skill.

---

## 1. How the system fits together

One system, with each part doing a different job on the same client path:

| Part | Job | Source |
|---|---|---|
| Trust rule | How we behave at every stage; every idea is checked against it first | Abraham, Strategy of Preeminence |
| Client path | 8 stages from first hearing of us to sending friends; where we find the weak spot | Deiss, Customer Value Journey |
| Growth levers | Which way each stage grows the salon: more clients, bigger visit, more often | Abraham, Three Ways to Grow |
| Rhythm | Monthly review and 90-day sprint: one insight, one decision at a time | Deiss, Scalable OS (monthly business review, quarterly sprint, 90-day game plan) |

### The trust rule (Abraham)
Act as each client's most trusted skin advisor, not a seller. Her long-term interest comes before today's sale. The test is: would we recommend this to our own family, even if it costs a sale today?
- **Principles:** her interest first; tell her what she needs, not only what she wants to hear; trust, not price, makes us hard to replace; compete on depth of relationship; never sell more or less than she needs.
- **Four trust steps:** Empathy (understand what she hasn't noticed), Advocacy (recommend what's best even if it earns less), Expertise (know her whole skin life), Proactivity (reach out before she asks).
- **Five questions from the client's side:** Would I want this if I were the client? Why act now? What's in it for me? How will it make me feel about myself and my skin? Why is it better than what I do now, or doing nothing?
- **Rollout (Abraham's advice):** not all at once; start with management and the best performers; find what already works and make it deliberate; test with existing clients first; study lost clients; train new staff from day one; review as a checklist until habit.
- **Australian limit:** risk reversal never means guaranteeing skin results. Stand behind the experience only, with Rory's approval of the exact words. Never promise results.

### The client path (Deiss), with lever and trust step
| # | Stage | Lever | Main trust step | Excite / Ascend notes |
|---|---|---|---|---|
| 1 | Aware | More clients | Expertise | |
| 2 | Engage | More clients | Empathy | |
| 3 | Subscribe | More clients | Empathy, Advocacy | Free 15-min skin diagnosis |
| 4 | Convert | More clients | Advocacy | |
| 5 | Excite | Bigger visit | Empathy, Expertise | Deiss's "ah-ha" quick win: she sees her skin on the Observ and the plan clicks |
| 6 | Ascend | Bigger visit, More often | Advocacy, Expertise | Rebook; home care that fits; doctor for deep active acne |
| 7 | Advocate | More often | Proactivity | Check-ins, fixing problems, reconnecting lapsed clients |
| 8 | Promote | More clients | Proactivity | Reviews (no gating), referrals |

The full stage details (client's question, trust behaviour, measures, sources, team habit, gaps) live in the Notion database **Client Path (8 stages)**. Read it at the start of every review. It's the source of truth if this file and Notion differ.

## 2. Where everything lives in Notion

Hub page: **Growth System** (inside Ella Baché Brain), https://app.notion.com/p/42676ddcbf5981eb93c6e4ae3a475ba1

| Database | Data source | Use |
|---|---|---|
| Client Path (8 stages) | collection://42676ddc-bf59-81ad-9689-000b9c7d5af7 | Stage reference (read) |
| Monthly Reviews | collection://42676ddc-bf59-8185-84f6-000bbf6d28c3 | One page per month (write) |
| Journey Metrics | collection://42676ddc-bf59-8159-a38d-000b47977069 | One row per measure per month (write) |
| Quarterly Sprints | collection://42676ddc-bf59-814a-a6b0-000b6b0481da | One page per 90 days (write when Rory decides) |
| Growth Ideas | collection://42676ddc-bf59-813f-bed4-000beb391cd7 | Idea parking lot with ICE scores (write) |
| Weekly Metrics (existing dashboard) | collection://ca7cdf87-9e91-4252-bfe9-bf428dcdb7d9 | Source for visits, new clients, rebookings (read only) |
| Routines (Brain) | collection://77aec28c-e1d5-4a56-88b7-80cd6eb85f53 | "Monthly growth review" and "Quarterly growth sprint" rows: update Last done / Next due |
| Tasks (Brain) | collection://e12b80cc-5bcf-42ad-b640-40117bbb0071 | A "Yes" decision or sprint initiative becomes a task |
| Decisions (Brain) | collection://430a175a-be34-46fd-9529-ed11dc7af403 | Log sprint decisions (date, why, revisit) |

Always fetch a data source before writing to it, and use its exact property names.

## 3. Rules for every mode

- **No invented data.** Every number comes from a connected source, with its date range written in "Source and dates". If a source can't be reached, mark the row `Measured = Not measured yet` and say why in the review's Gaps. Never estimate silently.
- **No money figures** (sales, cash, wages, profit) unless Rory asks for them at the time. Use counts and rates. Weekly Metrics holds money columns: don't read them into the review.
- **Search Console** is read through Genie (GenieSeo).
- **Meta ads data:** say what check you want and why, then wait for Rory's yes before reading it.
- **No client names** in reviews. Therapists appear only as team totals, unless Rory asks.
- **Plain, short language.** Say what each line relates to. One insight and one suggestion per review. At most one question.
- **The first review is the baseline.** Tick Baseline and don't judge trends.

## 4. Mode: monthly growth review

Trigger: "monthly growth review", "run the growth review", or the Routines row is due. Covers the previous calendar month.

1. Read the Client Path database (Path in order view) and the last Monthly Reviews page.
2. Pull each measure for the month and write one Journey Metrics row per measure. Fill Stage, Review, This month, Last month (copy from last month's row if it exists), Unit, Higher is better, Source and dates, and Measured.

| Stage | Measure | How to get it from chat |
|---|---|---|
| Aware | Instagram reach; Facebook reach | Metricool analytics for the month |
| Aware | Website sessions | GA4 property 379022137 (Ella Bache GA4 connector, or Genie) |
| Aware | Google search clicks; times shown | Search Console sc-domain:ellabachehobart.com.au via Genie |
| Engage | Saves + shares on Instagram posts | Metricool |
| Engage | Online enquiries / requests | Management app (not connected to chat; ask Rory for the month's count or mark not measured) |
| Subscribe | Free skin diagnosis bookings | Shortcuts copy (not connected to chat; ask Rory or mark not measured) |
| Convert | New clients | Weekly Metrics: sum "✍️ New clients" for pay weeks starting in the month |
| Excite | % of facials with an Observ check | Not measured yet until recorded in Shortcuts |
| Excite | First-visit ratings (Happy / Good enough / Problem) | Management app My day ratings (ask Rory or mark not measured) |
| Ascend | Rebooking rate | Weekly Metrics: sum Rebookings ÷ sum Visits for the month's pay weeks |
| Ascend | Visits | Weekly Metrics: sum "✍️ Visits" |
| Ascend | % offered home care | Management app My day ticks (ask Rory or mark not measured) |
| Advocate | Problem ratings; check-in texts and replies; lapsed clients | Management app (ask Rory or mark not measured) |
| Promote | New Google reviews; average rating | OpenSEO business reviews if available, else ask Rory |
| Promote | Referred new clients | Not measured yet until referral source is recorded |

3. **Find the weakest stage.** Compare each stage's measures with last month (and the same month last year once there's history). The weakest stage has the biggest drop or the lowest rate against its usual level. Earlier stages feed later ones, so check whether a drop is really caused upstream before blaming a stage.
4. **Write the Monthly Reviews page** (title like "November 2026"; Month start = 1st of the month):
   - Headline: one sentence on whether the path got stronger, held or slipped.
   - Weakest stage: the relation.
   - Insight: what moved and the likely reason (label a guess as a guess), tied to that stage's trust behaviour.
   - Suggestion: one next step for Rory, drawn from the stage's trust behaviour or team habit and the rollout rules. It's a suggestion only.
   - Gaps: what couldn't be measured and what would fix it.
   - Decision = Waiting for Rory; Status = Ready to read.
   - Page body: a short scorecard table (stage, measure, this month, last month, arrow), then the sources.
5. Update the Routines row "Monthly growth review": Last done = today, Next due = the 2nd of next month.
6. In chat, give Rory the headline, the weakest stage, the one suggestion and the link. Stop there.

**When Rory decides:** set Decision and Status = Decided. If Yes, create one Task (Owner per Rory, Source "Monthly growth review <month>", Next action written out). Do nothing else.

### The push (scheduled)
- **Monthly:** the scheduled task "Monthly growth review (Ella Baché)" runs this mode on the 2nd of each month and messages Rory the headline, weakest stage and one suggestion.
- **Weekly:** on Wednesdays the Marketing morning brief adds one rebooking line from Weekly Metrics (latest pay week with Visits and Rebookings entered: rebooking rate, last week, 4-week average). No target is shown until Rory sets one in a Quarterly Sprint.

## 5. Mode: quarterly sprint

Trigger: "quarterly sprint", "plan the quarter", or the Routines row is due.

1. Bring the last three Monthly Reviews: which stage was weakest most often, and which suggestions were said yes to.
2. Bring Growth Ideas sorted by ICE score. Score any unscored ideas with Rory (1–10 each for Impact, Confidence, Ease), and set the Trust check (Builds trust / Neutral / Costs trust). An idea that costs trust is never chosen.
3. Use Deiss's 90-day game plan questions: past 90 days (proud of, regret), present (confident in, lack), future (excited about, worried about).
4. Rory picks one focus stage, one trust habit for the team (from that stage's Team habit), one success measure with its start and target, and up to three initiatives.
5. Write the Quarterly Sprints page (Status Running). Create the initiatives as Tasks and link them. Mark the chosen ideas "Chosen for sprint". Log the decision in Decisions (revisit at the end of the sprint).
6. At the next sprint, fill "What we learned" and set Status Reviewed before planning the new one.

## 6. Mode: advisor check

Trigger: "what do you think of…", "check this against the trust rule", or a new idea, offer, post, script or process.

1. Name the stage(s) and lever it touches.
2. Run the five client-side questions; note any that fail.
3. Check the principles, especially "no more and no less than she needs" and "never promise results".
4. Verdict: Builds trust / Neutral / Costs trust, with one line why, plus at most one suggestion.
5. Offer to add it to Growth Ideas. Add it only if Rory says yes.

## 7. Gaps to close (tracked as a Task)
These are currently "not measured yet": Observ checks recorded in Shortcuts (not every facial has one yet); "how did you hear about us?" recorded for new clients; an optional "referred to doctor" tick on My day; and management-app figures (ratings, home-care ticks, texts) reaching chat. A server job could later write those into Journey Metrics. Raise one gap at a time, not all at once.

## 8. Sources
- Jay Abraham, Strategy of Preeminence: https://abraham.com/frameworks/strategy-of-preeminence (read 28 Nov 2026)
- Jay Abraham, five frameworks: https://abraham.com/frameworks and https://abraham.com/jay-abraham-frameworks (read 28 Nov 2026)
- The Strategy of Preeminence, adapted for a client (Abraham blog PDF): https://blog.abraham.com/wp-content/uploads/2014/02/The_Strategy_of_Preeminence-Adapted-for-a-Client1.pdf (read 28 Nov 2026)
- Ryan Deiss, Growth Ramp workbook (Value Journey Canvas: Aware, Engage, Subscribe, Convert, Excite, Ascend, Advocate, Promote) and Scalable OS sheets (Company Scorecard, Quarterly Sprint Canvas, 90 Day Game Plan, Idea Prioritization with ICE, Meeting Rhythm), from Rory's Growth Ramp folder (read 28 Nov 2026), plus Rory's own Step 1–6 notes.
- Abraham's results claims (e.g. 3–5× retention) are his own and unverified. Never repeat them as fact.

## Changelog
- 2026-11-28: v1.1. Monthly review runs on the 2nd as a scheduled task; weekly rebooking line in the Marketing morning brief.
- 2026-11-28: v1. Replaces ella-bache-preeminence. Joins Abraham and Deiss around the client path; Notion hub and databases built the same day.
