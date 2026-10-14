---
name: start-day
description: Start of the workday. Use when the user begins their day, needs a new day file, or when it is the first interaction of the day.
---

# Start Day

Workflow for opening a new workday in the journal.

## When

- First interaction of the day
- The user asks to start the day
- There is no day file for today yet

**Always in its own session** (see `AGENTS.md`, "One session per day"). If another day has already been processed in this session, do not start this workflow on your own: say that the new day belongs in a new session and stop there.

## Steps

1. **Create the day file**
   - Location: `journal/[YEAR]/[WEEK]/`
   - Naming convention: `[DAYNUMBER]-[day]-[DATE].md` (e.g. `3-wednesday-2026-03-11.md`)
   - Day numbers: 1=monday, 2=tuesday, 3=wednesday, 4=thursday, 5=friday
   - Template: `journal/daily-journal-template.md`
   - Create the week directory if it does not exist yet. Determine the date and week number via the terminal, not from memory.

2. **Consult the week kickoff**
   - Read `journal/[YEAR]/[WEEK]/0-kickoff-week-[WEEK].md`
   - Fill the **🎯 Planned** section with the tasks and meetings planned for today
   - Carry over tasks that were pushed forward from the previous day
   - **Possible Feedback is not a task**: items under "📨 Possible Feedback This Week" are not something the user actively drives today. Do not list them as tasks, do not reserve room for them. Only process them when something actually comes in that day, and then in the Daily Flow under the right project heading.

3. **Check the previous day**
   - Read the journal of the previous workday
   - Check for open tasks (`[ ]` and `[~]`) that need to be carried over
   - Check the **Carry Into Tomorrow** section for intentions

4. **Check the task manager** (if connected)
   - Fetch today's tasks, overdue tasks and upcoming deadlines. The task manager takes precedence over the week kickoff, also in wording (see `AGENTS.md`).
   - Add relevant tasks to **🎯 Planned**, short and as one-liners.
   - Tasks where the ball is with someone else go under **⏳ Waiting For Response**, with what they are waiting for in parentheses.
   - Flag: deadlines that clash with the day, tasks that have been pushed forward for several days (is there a threshold to getting started?), and a day without [your fuel].

5. **Check the calendar** (if connected)
   - Add appointments to **🎯 Planned** with their time: `- [ ] Meeting name (11:00)`
   - Watch for hidden context: an unexpected amount of meetings? Gaps for focused work? Work location? This feeds step 9.

6. **Check tickets, chat and email** (if connected)
   - Window: since the previous workday (after a weekend or days off: the last workday before that). Use an absolute date, not a relative window like "last 24 hours": that shifts with whatever time the check happens to run, and gaps appear.
   - The window deliberately overlaps with what was already seen the previous morning. Weigh against the journal of the previous workday before marking anything as new; a handled item still looks open in an inbox.
   - Items that need action today go into **🎯 Planned** as one-liners; what can wait may go to the task manager with a reference to the source. When in doubt, ask first.
   - Mention the rest briefly at most in the morning overview. Skip newsletters and automated notifications.

7. **Lay out the learning goals**
   - Read the learning goals at the top of `work-evaluation/expectations.md` (the rest of the file is for the reflection and the weekly review)
   - Connect the planned meetings and tasks to relevant learning goals
   - Briefly name which learning goals may be relevant today

8. **Proactive coaching**
   - Which learning goals touch the planned meetings?
   - Are there specific things to watch for?
   - Short and practical: no long stories, only usable signals

9. **Signal check** (see `AGENTS.md`, "Being seen")
   - **Days without [your fuel]**: scan the last 2 to 3 Daily Flow sections. Several days in a row without any of it: name it, not dramatically, but concretely.
   - **Empty "Who Saw You Today?"**: check the last few days. Several (nearly) empty fields in a row is a signal; bring it up as a soft observation, not as an accusation.
   - **Weekend or Monday dip**: if the user comes in flat, tired or down, do not go straight to task planning. Make a little room first.
   - **Role stacking today**: lots of meetings, project management and client contact without time for the user's own work? Flag it early, so the user can make a deliberate choice.

## Loading context

At the start of a session, also read the files in `profile/` for personal context. Use these subtly as background for the coaching, without naming them explicitly.
