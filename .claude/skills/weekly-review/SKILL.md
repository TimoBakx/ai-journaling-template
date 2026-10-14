---
name: weekly-review
description: Write the weekly review. Use at the end of the workweek for a deeper reflection on patterns, learning goals and the weighing against the expectations of the role.
---

# Weekly Review

Weekly reviews are moments of **deeper reflection**: analyzing patterns, working out insights, making connections, and looking at where the learning goals were worked on and how the week relates to the expectation per component in `work-evaluation/expectations.md`.

## When

- End of the week (Friday or the last moment of the workweek)
- Location: `week-evaluation.md` inside the week directory (`journal/[YEAR]/[WEEK]/`)
- Template: `journal/weekly-review-template.md`
- Covers the full workweek

**Always in its own session** (see `AGENTS.md`, "One session per day"). Do not tack it onto a day session, not even when Friday has just been finished: the weekly review has to read and weigh the daily journals itself, not lean on whatever happens to still be in the conversation.

## Preparation

- Read **all daily journals** of this week
- Read the **previous two weekly reviews** as context
- Read the **week kickoff** of this week
- Read `work-evaluation/expectations.md` for the learning goals, the expectation per component and what is already listed under Above expectations and Dropped balls

## Template sections

- **📅 This Week**: overview per day with links and a short summary
- **🎯 Major Themes**: the main subjects of the week
- **🎯 Work On Learning Goals**: per learning goal: did I work on it this week, and if so, how (with links to the days). No status, no symbols. "Not this week" is an ordinary outcome.
- **⚖️ This Week's Weighing**: the points from Above Expectations and Dropped Balls of the daily journals, grouped per component, with the source of recognition for above expectations and the fix for a dropped ball. Plus whatever the week analysis adds.
- **📚 Knowledge Sharing Check**: what was learned or done that can be shared, and with whom?
- **🧠 Self-Insight & Profile Confirmations**: brief
- **👀 Who Saw You This Week?**: aggregation of the daily notes; empty = empty, that is data
- **🚩 Open Signals (Persistent)**: named needs, insights or observations that have not been addressed yet
- **🏢 Meeting Expectations**: what simply went well, only when something stands out
- **🔄 Check Against This Week's Kickoff**: to what extent did the week follow the kickoff document?
- **💡 Actions Next Week**: concrete follow-up steps
- **🌟 Week Summary**: the big reflection on the week

## Approach

- **Ask follow-up questions on big insights** and on anything unclear
- **Connect the days**: what connects the different days?
- **Recognize trends**: patterns that were visible before as well
- **Weigh against the components** in `expectations.md`, strictly according to `AGENTS.md` ("Reflection: weigh, don't match"; the five mistakes). Critical questions per candidate: which component, and beyond its description? New behavior? Breakthrough or just good work? Someone else's role? A peak, or the completion of earlier work?
- **Dropped balls across the week**: does the same kind of dropped ball recur on the same component, or did an earlier fix not work? Name that. Once is a data point.
- **Update `expectations.md`**: are all points from this week's daily journals listed under the right component? Add what is missing. If the week analysis finds an example or dropped ball that was not seen on the days, present it to the user first.
- **Do not search in order to fill**: do not automatically make something up under every component or learning goal. A week without an example of above expectations is a legitimate outcome.
- **Kickoff check**: to what extent were the points from the kickoff document followed? Why were some points dropped? Points that were picked up but not processed in the journal?

## Source of recognition for above expectations: mark it honestly

For each example of above expectations, explicitly mark where that recognition comes from:

- **👥 Confirmed externally**: a human (colleague, stakeholder, manager) reflected this back; name who and where
- **🪞 By the user**: the user recognizes this as above expectations themselves, without external confirmation
- **🤖 By the journal**: the agent flags this based on pattern recognition, without a human having confirmed it

Purpose: prevent "Above expectations ✅" from becoming a closed loop in which the journal confirms itself. Writing down "above expectations" does not make it true. If over several weeks nearly all recognition sits in 🪞 or 🤖 and never in 👥, that is a signal: not a failure of the user, but a sign that recognition around the user is too thin.

## Aggregating "Who Saw You?"

Read the daily fields from the daily journals and aggregate them. Empty is empty: do not fill it with "nobody specific" as a consolation, do not invent generic compliments. Three weeks in a row (nearly) empty is a signal for a conversation with the manager.

## Knowledge sharing check

Look at the past week for things that can be shared proactively, and with which audience: [fill in your own audiences, for example: your team, a chapter or guild, all developers, the whole company].

## Weeks in which everything simply meets expectations

Not every week has to show something above expectations, and not every week includes work on every learning goal. That is fine. Observe neutrally: "No examples of above expectations this week" or "No work on this learning goal this week". Forcing above expectations is not healthy; situations have to arise naturally.

## Closing: the week kickoff for next week

At the end of the weekly review, create a `0-kickoff-week-[WEEK].md` for next week, based on `journal/weekly-kickoff-template.md`.

### High-level view, no duplicate task list

The week kickoff is a **guiding document** for the start of the week, not a task list. Everything that is already in the task manager (tickets, deadlines, specific actions) belongs there, not here again. Double bookkeeping produces noise instead of direction.

What **does** go into the kickoff:

- **🎬 This Week**: atmosphere, mode, energy (working from home or at the office, short week, project pressure). Explicitly ask the user for the planning per day if that is recorded somewhere, and pose the check: *"Does this picture match, or am I missing something?"*
- **🚩 Open Signals**: structural observations, after cleaning up (see below).
- **📨 Possible Feedback This Week**: one line per project, items a response may come in on without the user driving them.
- **🗓️ Planned Meetings**: checked against the calendar for the whole workweek, including overlap or conflicts.
- **🎯 Learning Goals: What To Watch For**: advisory, short, not every learning goal required. Only where the agent adds something. No self-made jargon labels; concrete, recognizable wording. If there are no strong opportunities already visible in the planning: say so honestly.
- **💡 Points of Attention**: at the level of the week (energy, patterns, planning risks). No tickets, no tasks.

What does **not** go into the kickoff: ongoing matters with tickets and deadlines (task manager), lessons from the past week (weekly review), and a hook per project under every learning goal (too much detail, too repetitive).

### Actively clean up open signals

When carrying open signals over to the new kickoff: actively clean up, do not drag everything along. Main question: *"is this relevant for the coming week?"*, not *"is this old?"*. Rules of thumb in order of importance:

1. Relevant for the coming week (planning, current sprint, planned meetings, known deadlines)? Keep, regardless of age.
2. Waiting for a one-off response? Move to 📨 Possible Feedback.
3. Self-correction or implicit closure mentioned by the user? Actively ask whether the signal can be removed.
4. Older than about three weeks, no new insights, not relevant for the coming week? Candidate for cleanup. If it is an organizational pattern, ask whether it may move to a dossier.

When in doubt: better to keep and ask than to discard silently.

### Pick up directly instead of parking

Small things that can be done right away (refreshing a project file, a mini task): directly ask whether the user wants the agent to do it, instead of parking it as a point of attention in the kickoff. Points of attention are for things that run along through the week, not for five-minute tasks.

### Waiting for feedback is not an ongoing matter

For each item, check: *"what is the user's action here this week?"*. If the answer is "wait and respond when it comes in", it belongs in 📨 Possible Feedback, not under open signals. Experiencing items that are already finished but waiting for a response as workload builds false tension around things the user is not actively driving.
