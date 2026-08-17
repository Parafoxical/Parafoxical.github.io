# Why the site is arranged the way it is

Every grouping and every heading, with the reason. Written after a full audit of all
121 cards, their kinds, their placement and their cross-links.

---

## The organising principle

**The sheets follow the order the work happens in.** Discover, then Analyse, then
Specify, then Validate. Everything else is either a thing you do across all four
(Keeping control, Ways of working) or a lookup (Technical literacy, Tools, Glossary).

This is not the only possible order. The alternative — grouping by kind, so all the
documents live together and all the techniques live together — reads well as a reference
and badly as a course, because it asks you to learn what a BRD is before you have any
idea why anyone would write one.

**Define once, link everywhere.** A term gets exactly one card, on the sheet where the
concept is taught. Every other mention anywhere in the pack is a hover link. This is the
rule that keeps the overview page honest: it can *mention* anything, but it may not
*teach* anything that belongs to a later sheet.

---

## Sheet 01 — What a business analyst does

Six cards. Two blocks. Deliberately the thinnest sheet in the pack.

| Block | Why |
|---|---|
| **The job** | `business-analysis` and `business-analyst`. The discipline and the person. Nothing else qualifies as "the job" — everything else is a thing the job involves. |
| **The four stages** | `discover-stage`, `analyse-stage`, `specify-stage`, `validate-stage`. The map of the next four sheets. |

The heading "The four stages" is plural and concrete because the block is a list of
named things, not an argument.

**The note above the four stages** exists because this page used to carry nine extra
cards — solution, analysis, specification, validation, problem definition, option
assessment and three architecture terms — and a reader would meet them here, hover, and
commit to learning them properly, hours before the sheet that actually teaches them. The
overview page was doing four other sheets' teaching. The note tells you not to.

Sheet 01 is the one to police. Every future card proposed for it needs a reason it is
not on the stage sheet that owns it, and "it looks foundational" is the argument that
readmits `requirement`, then `stakeholder`, and rebuilds the nine-card block one
reasonable case at a time.

---

## Sheet 02 — Discover

Twenty-one cards, the heaviest sheet, correctly so: Discover is where most of the work
is. The blocks are ordered as questions you ask in sequence.

| Block | Why that grouping, why that name |
|---|---|
| **Why you are here** | `problem-definition`, `discovery-session`. Both are about establishing that there is a problem before anyone proposes a fix. Named as a question because that is what the block answers. |
| **Who you ask** | `stakeholder`, `stakeholder-engagement`. People, before techniques — you cannot choose an elicitation method until you know who you are eliciting from. |
| **How you draw it out** | `elicitation` plus its seven techniques. "Draw it out" rather than "gather" on purpose: the whole point of the elicitation card is that requirements are pulled out, not collected. The heading teaches the same lesson the card does. |
| **What you are collecting** | `requirement`, `requirements-engineering`, `requirements-gathering`. The output of the block above. |
| **Where the business is now** | `as-is`, `process-mapping`, `process-model`. Moved here from the old Process mapping sheet: you map the current state *while* discovering, not afterwards. |
| **Drawing a process** | `bpmn` and its three shapes. Follows the block above because you need the notation before you can draw anything. |

---

## Sheet 03 — Analyse

Ten cards. The stage that turns facts into a recommendation.

| Block | Why |
|---|---|
| **What analysis is** | `analysis` alone. It opens the sheet because it is the activity the whole phase is named after — taught where it is done, not on the overview. |
| **Where it should get to** | `to-be`, `future-state`. Two names for one idea, deliberately adjacent so you learn they are synonyms rather than meeting them separately and assuming they differ. |
| **The gap between them** | `gap-analysis`, `impact-analysis`. Renamed from "The difference between them", which said nothing about what was inside it. "Gap" is the word the cards use. |
| **Choosing what to do** | `option-assessment`, `solution`. `solution` sits here because choosing between solutions is the moment the word matters, and the moment to learn that a solution need not be software. |
| **Improving a process** | `bpi`, `lean-six-sigma`, `digital-transformation`. Moved off Technical literacy, where they never belonged — they are approaches to change, not technical vocabulary. |

---

## Sheet 04 — Specify

Seventeen cards. The documents and who receives them.

| Block | Why |
|---|---|
| **What a specification is** | `specification`, `artefact`. The general words before the specific documents. |
| **The document ladder** | `brd`, `frd`, `functional-spec`. "Ladder" because they are rungs — business need at the top, system behaviour at the bottom — and the relationship between them is the thing being taught. |
| **Kinds of requirement** | `business-requirements`, `functional-requirement`. |
| **Agile artefacts** | `user-story`, `epic`, `acceptance-criteria`, `use-case`. Separated from the document ladder because these are what the same job looks like in an agile team. |
| **Describing a system** | `uml`, `oo`. Moved off the old Process mapping sheet. Sitting next to BPMN implied UML and BPMN were alternatives to each other; they are not. BPMN describes the business process being discovered, UML describes the system being specified. |
| **Who you hand it to** | `solution-architect`, `delivery-team`, `enterprise-architecture`, `togaf`. The old sheet 01 had a "The people" block where these were context-free. They now appear at the point in the process where you actually deal with that person or that constraint. |

---

## Sheet 05 — Validate

Seventeen cards. Its id is `validatep`, not `validate`, because `validate` is now a term
id and the two would collide.

| Block | Why |
|---|---|
| **What validation means** | `validation`, `business-validation`. The distinction from verification is the whole point of the sheet, so it opens with it. |
| **Acceptance** | `uat`, `uat-planning`, `sign-off`. The formal path from "users try it" to "someone accepts responsibility". |
| **Defects** | `defect`, `triage`, `severity`, `priority`. Severity and priority are adjacent because the entire lesson is that they are different and often disagree. |
| **Kinds of testing** | `regression-testing`, `e2e`, `test-case`. |
| **Going live** | `change-approval`, `release-management`, `sla`, `incident-escalation`, `incident`. Everything that happens after acceptance and before you can stop worrying. |

---

## Sheets 06 to 09

**06 Keeping control** — Scope / Prioritising / Logs and registers. Unchanged. These
apply across all four stages rather than sitting inside one, which is why it follows
them rather than interrupting them.

**07 Ways of working** — Around the method / The two shapes / Scrum / Kanban. "The two
shapes" holds `waterfall` and `agile` because the card content is a shape comparison:
everything decided up front, versus the next bit decided and a readiness to be wrong.

**08 Technical literacy** — one block, `api`, `integration`, `sql`, `erp`. Renamed from
"The words that aren't about process", which was the sheet's own subtitle repeated back;
it is now **Systems and data**, which says what the four cards are. Four cards is thin,
and this sheet is the obvious candidate to absorb technical vocabulary as later sheets
get read, or to fold into 09.

**09 Tools and certifications** — Diagramming / Delivery and tracking / Data and
reporting / Enterprise platforms / Certifications / **For the interview**. The last block
is new: `star` was sitting under Certifications, and STAR is not a certification — it is
a structure for answering interview questions. It now has its own block of one, which is
honest, rather than a wrong home that was tidier.

---

## The kinds, and what decides them

Seven tags. The tag answers "what kind of thing is this?", which is a different question
from "where does it live?".

| Kind | Test |
|---|---|
| `definition` | A concept or category you must be able to state |
| `process` | An activity or way of working — something done over time |
| `technique` | A named method you apply |
| `document` | A thing you write and hand over |
| `role` | A person or a team |
| `software` | A named product |
| `qualification` | A certification |

Eleven cards carry no tag at all — the three BPMN shapes, the four MoSCoW letters, the
four RAID letters. They are parts of a bigger idea, not kinds of their own, and tagging
them would add noise without adding information.

### The rule that changed

Minor processes used to be tagged `definition`. That was a workaround from when the site
was organised by kind: a small activity like problem definition looked odd filed under
"process" next to Waterfall and Agile. Now the site is organised by process, the
workaround is unnecessary and actively misleading. **A minor process is still a process.**

---

## What the audit found

All 121 cards checked for kind, placement and heading; all 169 defined terms checked for
link coverage across every card and every glossary entry.

| Finding | Count | Action |
|---|---|---|
| Terms mentioned somewhere but not hoverable there | **149** | All linked |
| Cards with the wrong kind | **6** | All corrected, on both card and glossary twin |
| Cards in a block that did not fit | **1** | STAR moved to its own block |
| Block headings that did not describe their contents | **2** | Renamed |

### The six kinds corrected

| Card | Was | Now | Why |
|---|---|---|---|
| `problem-definition` | definition | **process** | A small activity is still an activity |
| `option-assessment` | definition | **process** | Same |
| `change-approval` | definition | **process** | A governance gate is a step, not a concept |
| `elicitation` | definition | **process** | It is the umbrella activity above the seven techniques in its own block |
| `erp` | software | **definition** | A category of system, not a named product. It was the only card tagged `software` that was not a product name |
| `acceptance-criteria` | definition | **document** | A written list, like the rest of the Agile artefacts block |

### The linking rules

A mention becomes a link unless it is already inside a link, already inside a highlight
(one signal per word), in the card that defines it, or owned by a longer term. That last
rule is what makes **business requirements** link as a whole phrase rather than leaving
*requirements* pointing somewhere vaguer, and what stops *Azure* being linked inside
*Azure DevOps*.

Inflections count. *Validating* links to Validation, *specs* to Specification, *stories*
to User story. That was the reported symptom — reading the Survey card with the word
"validating" sitting there dead — and it is fixed.

Six aliases were rejected during the audit for being ordinary English rather than the
term: *to be*, *as is*, *the gap*, *escalation*, *prioritising*, *observed*. Each of them
produced at least one wrong link in testing — "stays ready **to be** wrong" linking to
the To-be card being the clearest.

A later pass audited the links the other way round, comparing each link's text against
what it points at. That found **20 pre-existing wrong links**, all of them the phrase
"to be" pointing at the To-be card — "waiting *to be* picked up", "has *to be*",
"expressed so as *to be* individually verifiable". None of them referred to the to-be
state. All removed. Four other flagged classes turned out to be legitimate short forms —
*backlog* for Product backlog, *Dynamics 365* for D365, *BA*, *Dev Ops*.

## Sheet 10 — The gaps

The chase-up list used to carry truncated blurbs ending in an ellipsis, so the only way
to read a definition was to hover it. Each entry now carries the **full** plain-English
definition, taken straight from that term's glossary entry — which means it inherits the
highlights and hover links that entry already has, rather than keeping a second copy of
either that could drift.

All 28 entries are highlighted to the same four-type system as the cards. Twenty-two of
them had no highlight markup at all before this pass.

---

## Judgement calls deliberately left alone

- **`epic` stays `document`.** An epic is a size category, which argues for `definition`,
  but it sits in a block of written artefacts and is itself written down. Either reading
  is defensible; changing it would be churn on a coin toss.
- **`sprint` and `ceremonies` stay `process`.** A sprint is a period rather than an
  activity, but both are parts of the Scrum way of working and the sheet is Ways of
  working. Consistency within the sheet beats precision about the part of speech.
- **`itil` and `prince2` stay `qualification`.** Both are frameworks as well as
  certifications. They sit in the Certifications block because that is how they appear on
  a CV, which is the reason they are in the pack at all.
- **`digital-transformation` and `bpi` are cards on sheet 03 while the gaps sheet lists
  them as padding.** That contradiction predates this restructure. The cards are worth
  having; the gaps sheet is telling you not to *study* them. Worth resolving, but it is a
  content decision rather than a structural one.
