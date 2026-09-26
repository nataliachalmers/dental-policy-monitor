---
name: dental-policy-monitor
description: Weekly scan of CMS, Medicare, Congress and state Medicaid dental policy changes as a one-page brief with primary-source links and Overjet relevance flags. Use when Natalia asks for the policy brief or what changed.
---

# Dental Policy Monitor (Delegate task)

Natalia gives direction and reviews. Claude gathers, sorts and summarizes. Claude never makes a policy judgment or recommends a strategy decision; it reports what changed and where to verify it.

## Time window
Default: the last 7 days (previous Monday to Sunday when run on a Monday). If the user names a window ("since Sept 1"), use that. Do not widen the window on a quiet week; say it was quiet instead.

## Sources to check (in this order)
1. **Federal Register** (federalregister.gov): CMS rules and notices mentioning dental, oral health, Medicare Part B dental, PFS, OPPS, MA, Medicaid.
2. **CMS** (cms.gov, medicaid.gov New & Notable): newsroom, fact sheets, CMCS Informational Bulletins, State Medicaid Director / State Health Official letters, Medicare dental coverage page, MLN Matters. Also RFIs on sam.gov.
3. **Approved state plan amendments and 1115 waivers** on medicaid.gov that touch dental.
4. **State Medicaid agencies and legislatures**: adult dental benefit changes, rate changes, delivery model changes (FFS / MCO carve-in / dental benefit manager), prior-authorization rules.
5. **Congress** (congress.gov, committee sites for Energy & Commerce, Ways & Means, Senate Finance, HELP, Judiciary): dental bills introduced or advanced, hearings and markups touching dental, Medicaid dental, MA supplemental benefits, dental insurance, or AI in claims review. Link the congress.gov bill page or the committee hearing page.
6. **Trusted trackers** to find leads (never cite as the only source): ADA News, ADA Health Policy Institute, CareQuest Institute, NASHP, KFF, MACPAC, Commonwealth Fund, MSDA, state dental associations.

Search with dated queries (month and year) and prefer primary sources. If a lead comes from a tracker, find the primary document before including it.

## What counts
Include: rules (proposed/final), coverage or benefit changes, payment/rate changes, codes (CDT/HCPCS, e.g. G0330), billing and claims requirements, prior-authorization or FWA rules, quality measures, waivers/SPAs, bills and hearings, court decisions, budget actions, and comment deadlines.
Skip: opinion pieces, vendor marketing, consumer explainer sites, and items older than the window unless there is a new action on them.

## Topic tags
Medicare coverage · Medicare payment/codes · Medicaid adult benefit · Medicaid pediatric/EPSDT · Delivery model · Rates · Prior auth / FWA · Quality measures · Workforce / scope · Teledentistry / AI / interoperability · Legislation · Other

**Overjet flag:** add "⚑ Overjet" after the tag when an item touches AI or automated claims review, radiograph/imaging requirements, claims attachments, interoperability/FHIR/data standards, prior authorization, FWA/program integrity, or quality measurement. Say in a few words which of these it touches. This is a relevance flag, not advice.

## Output format (one page)
```
# Dental Policy Brief: week of <Mon date> to <Sun date>
Checked: <sources checked> · Prepared <date> · VERIFY BEFORE USE

## Top 3 this week
1. <One line: what changed, who, key date>. Why it matters, in one clause. [primary link]

## Federal (CMS / Medicare / Medicaid)
| Item | Type | Status & key date | Tag | Source |

## Congress
| Bill / hearing | Chamber & committee | Status & key date | Tag | Source |

## States
| State | What changed | Status & effective date | Tag | Source |
(Alphabetical by state. "No dental changes found" if none.)

## Deadlines coming up
- <Comment deadline / effective date / expected final rule>: <item> [link]

## Watch list (unconfirmed)
- Items seen only in secondary sources, with what still needs confirming.
```

## Rules
- Every table item and every Top 3 item has a direct link to a primary source (Federal Register, CMS, medicaid.gov, sam.gov, congress.gov, committee site, state agency or legislature). No primary link: move it to the Watch list.
- Give exact dates (published, effective, comment deadline). Never guess a date. If sources disagree (e.g. on a bill number), say so on the Watch list.
- Summarize facts only. No "should", no strategy advice. At most one clause on why it matters.
- Say plainly when a week is quiet; never pad.
- Keep it to one page: at most 3 top items, 10 federal rows, 10 Congress rows, 15 state rows.
- Save the brief as a markdown file named dental-policy-brief-YYYY-MM-DD.md.
- End with: "Review checklist: confirm each Top 3 item against its source before sharing or using in decisions."
