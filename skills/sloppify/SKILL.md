---
name: sloppify
description: "Editorial filter for removing AI-generated padding from product copy and UI structure. Use when reviewing or writing user-facing text, screens, components, onboarding, empty states, settings, dashboards, marketing pages, or flows that feel generic, repetitive, over-explained, over-designed, or padded. Trigger on: 'sloppify this', 'this feels AI', 'clean up the copy', 'too much text', 'too many cards', 'too many buttons', 'remove duplication', 'make this sharper', 'watered down'."
---

# Sloppify

Slop is content or interface structure that looks polished but does not help the user. It repeats, decorates, hedges, explains the obvious, or adds choices without improving comprehension or action.

Every word, button, and container must earn its place.

## Core Tests

Apply these tests to all visible copy, layout, and actions.

1. **Removal test**  
   If removing it costs the user no fact, decision, action, warning, or orientation, remove it.

2. **Specificity test**  
   If the line could appear unchanged in another product, rewrite it with the actual object, state, user need, or consequence.

3. **Duplication test**  
   If a headline, subtitle, body line, tooltip, CTA, or section repeats the same idea, keep the clearest version.

4. **Container test**  
   If a card, panel, divider, or disclosure only decorates thin content, flatten it.

5. **Action test**  
   Every button must map to a distinct user action. Do not use buttons for passive facts, statuses, labels, or duplicate routes.

6. **Evidence test**  
   Prefer visible facts, current state, next steps, constraints, or consequences. Cut abstract reassurance.

## Copy Patterns

### Negative parallelism

Avoid `not X, but Y` constructions. They sound decisive while delaying the actual point.

Bad:
> Not just a dashboard, but a smarter way to work.

Better:
> See overdue tasks, blocked work, and next steps in one view.

Bad:
> This is not another settings page. It is your control center.

Better:
> Manage notifications, privacy, billing, and team access.

### Empty affirmation

Cut supportive lines that contain no fact, action, or observation.

Bad:
> Small steps still matter.

Better:
> You completed 2 of 5 required steps.

Bad:
> Everything you need is right here.

Better:
> Upload the file, choose a template, then export the report.

### Generic value claim

Replace abstract benefit language with what the user can see or do.

Bad:
> Unlock powerful insights with a seamless experience.

Better:
> Compare revenue, churn, and active accounts by month.

Bad:
> Built to help teams move faster.

Better:
> Assign owners, set due dates, and review blockers before standup.

### App self-narration

Do not make the product describe itself as an actor unless the brand voice explicitly requires it.

Bad:
> The app found something important.

Better:
> Three invoices are past due.

Bad:
> We noticed your setup is incomplete.

Better:
> Add a payment method to finish setup.

### Explaining obvious state

If the UI already shows a state, do not narrate it.

Bad:
> Search mode is active, so results are filtered by your query.

Better:
> 12 results for "contract"

Bad:
> You are currently viewing archived items.

Better:
> Archived items

### System apology

Do not expose implementation thresholds or internal limits unless they help the user act.

Bad:
> You need at least 5 entries before this section becomes available.

Better:
> Add more entries to see trends.

Bad:
> This feature is unavailable because no valid records were returned.

Better:
> No records found.

### Count leak

Use exact numbers when they help decisions. Avoid dumping internal counts to make copy sound precise.

Bad:
> Based on 7 events, 4 updates, and 3 recent changes.

Better:
> Based on recent activity.

Good when the number matters:
> 3 files failed to upload.

### Hedge stacking

Use one qualifier at most. Multiple hedges erase the claim.

Bad:
> Some users may often find this option helpful in certain cases.

Better:
> Use this when the default format does not match your report.

Bad:
> This can generally help reduce possible setup issues.

Better:
> This reduces setup errors.

### Intro and recap padding

Do not wrap one idea in an introduction and closing summary.

Bad:
> Managing access is an important part of keeping your workspace organized. Use this section to invite teammates and adjust permissions. Keeping permissions up to date helps everyone work better together.

Better:
> Invite teammates and set permissions.

### Triplet stacking

Avoid repeated groups of three benefits or adjectives unless the list is genuinely scannable and distinct.

Bad:
> Fast, flexible, and powerful tools for modern, growing, ambitious teams.

Better:
> Create reports from saved templates.

### Banned Generic Language

Rewrite these on sight unless they are part of a real proper noun:

`delve`, `intricate`, `tapestry`, `pivotal`, `underscore`, `foster`, `enhance`, `crucial`, `robust`, `seamless`, `boast`, `unlock`, `empower`, `leverage`, `showcase`, `groundbreaking`, `cutting-edge`, `game-changer`, `myriad`, `actionable`, `testament`, `cornerstone`, `innovative`, `vibrant`, `transformative`

Also avoid:

- `In today's...`
- `In a world where...`
- `Imagine this...`
- `It's worth noting that...`
- `At the end of the day...`
- `In conclusion...`
- `serves as a testament to...`
- `paves the way for...`

## UI Patterns

### Over-nested containers

Flatten nested surfaces unless each level has a clear job.

Bad:
> Page section -> card -> inner card -> stat tile -> label

Better:
> Page section -> grouped stats

Bad:
> A card containing one sentence and another card containing one button.

Better:
> One row with the sentence and action.

### One-item sections

A section header implies a group. If there is only one item, merge or remove the header.

Bad:
> Security  
> Change password

Better:
> Change password

Bad:
> Summary  
> Your export is ready.

Better:
> Your export is ready.

### Duplicate CTAs

One destination needs one primary entry point in the current context.

Bad:
> Header: Export  
> Footer: Export report  
> Empty state: Start export

Better:
> Primary action: Export report

### Buttons for passive information

Do not wrap labels, statuses, dates, or stats in button styling unless they are interactive.

Bad:
> [Active] [12 members] [Last updated today]

Better:
> Active - 12 members - Updated today

### Disclosure as justification

Do not hide explanations behind panels whose real purpose is to defend weak content.

Bad:
> "Why am I seeing this?" under every recommendation.

Better:
> State the reason in the line if it changes user trust.

Example:
> Price changed since your last order.

### Repeated metric representations

Do not show the same number as a card, chart, progress bar, percentage, and sentence.

Bad:
> 72% complete  
> progress bar at 72%  
> "You are 72% done"  
> 72/100 card

Better:
> 72% complete

### Decorative data cards

Related data should share a surface. Do not split every value into its own card.

Bad:
> Four separate cards for name, status, owner, and date.

Better:
> One row: name, status, owner, date.

## Rewrite Method

1. Read all visible copy, labels, actions, empty states, tooltips, and containers.
2. Delete anything that fails the removal test.
3. Merge repeated ideas.
4. Flatten containers that do not clarify hierarchy.
5. Reduce buttons to distinct actions.
6. Rewrite remaining copy with concrete facts, states, or next steps.
7. Prefer shorter output unless extra words add real clarity.

## Output Style

When sloppifying, provide:

1. **What to cut** - duplicated, generic, or decorative elements.
2. **What to rewrite** - before/after copy where useful.
3. **What to restructure** - cards, buttons, sections, or hierarchy.
4. **Clean version** - the tightened copy or UI structure.

Do not only criticize. Produce the sharper version.
