# 06 --- SaaS Product Blueprint

## Product principle

The SaaS should not be "another community app." It should make the economic and operating system work better.

The first version should answer:
1. What should I do next?
2. Who can I help/refer?
3. What did I commit to?
4. What value have I received?
5. Is my business improving?

## User roles

- Platform Admin
- Chapter Leader / Facilitator
- Member
- Optional Specialist/Guest
- Future Multi-Chapter Operator

## Core entities / data model

### User
name, contact, role, chapter, permissions.

### Business
name, category, subcategory, service area, website, description, revenue band (optional), employee band, ICP, offers, average customer value, exclusions.

### Chapter
name, geography, facilitator, meeting cadence, seats/categories, member count, status.

### Membership
business, chapter, seat/category, join date, dues, status, renewal, attendance.

### Referral Trigger
source category/business, destination category/business, event, listen-for phrase, qualifying questions, handoff instruction.

### Referral
sender, recipient, prospect/customer, trigger, date, status, estimated value, actual value, close/loss, notes, attribution.

### Goal
member/business, metric, baseline, target, deadline, status.

### KPI Snapshot
business, period, leads, conversions, revenue, average ticket, referrals, reviews, optional margin fields.

### Experiment
business, lever, hypothesis, baseline, action, target, start/end, outcome, annualized impact, lesson.

### Commitment
member, meeting, action, due date, status, result.

### Meeting
chapter, date, agenda, attendance, discussion items, decisions, commitments, assets.

### Asset
template/campaign/script/checklist, module, owner, generated/customized version.

### Win
member, source (referral/experiment/action), economic value, evidence, date, permission-to-share flag.

## MVP screens

1. **Home Dashboard**
   - next meeting;
   - commitments due;
   - referrals needing action;
   - YTD value received;
   - current growth experiment;
   - quick actions.
2. **Referral Wheel**
   - visual network;
   - member cards;
   - trigger events;
   - send referral;
   - open referrals;
   - referral results.
3. **Growth Scorecard**
   - simple monthly KPIs;
   - trends;
   - leverage calculator.
4. **Experiments**
   - active;
   - completed;
   - results;
   - lessons.
5. **Meetings**
   - agenda;
   - prep;
   - notes;
   - commitments;
   - follow-up.
6. **Member Directory**
   - ICP;
   - services;
   - trigger events;
   - introduction instructions.
7. **ROI / Value**
   - dues paid;
   - referred pipeline;
   - closed referred revenue;
   - experiment impact;
   - wins.

## AI features worth testing

Do not build all at once.

### Meeting Copilot
Convert meeting notes/transcript into:
- decisions;
- commitments;
- due dates;
- experiments;
- unresolved issues;
- follow-up summary.

### Referral Copilot
Given a situation, suggest relevant member(s) and explain the trigger match.

### Growth Opportunity Finder
Given KPIs, calculate possible leverage:
- leads × conversion × ticket;
- pricing lift;
- conversion lift;
- frequency lift;
- reactivation potential.

### Campaign Builder
Generate member-specific:
- reactivation email/SMS;
- referral ask;
- review request;
- estimate follow-up;
- partnership outreach.

### Chapter Health
Flag:
- low attendance;
- member receiving no referrals;
- unbalanced giving/receiving;
- unanswered referrals;
- missing categories;
- declining engagement.

## Important product insight

The most defensible dataset may eventually be the **relationship between intervention and outcome**:
- what type of business;
- what problem;
- what experiment;
- what asset;
- what result.

Over time the system could answer: "Businesses like yours with this pattern tend to get the fastest return from these three actions."

## Base44-friendly MVP approach

Using the user's preferred stack/capabilities, this can be built as a straightforward entity-driven app:
- React + Tailwind + shadcn/ui;
- Entities SDK for Chapter, Business, Membership, Referral, Trigger, KPI, Experiment, Commitment, Meeting, Asset, Win;
- Core InvokeLLM for summaries/recommendations/content generation;
- SendEmail for invitations and follow-up;
- recharts for KPI/value trends;
- react-hook-form for member/referral/experiment forms;
- no unnecessary external libraries.

## MVP sequencing

**Phase 0:** spreadsheet/manual process.

**Phase 1:** member directory + referrals + commitments + ROI.

**Phase 2:** KPI scorecard + experiments + meetings.

**Phase 3:** AI meeting/referral/growth assistants.

**Phase 4:** multi-chapter administration, billing, benchmarks, leader playbooks.

Do not build Phase 3--4 until actual chapter behavior proves the data model.
