---
name: reflection
description: Fill in the end of day reflection together. Use when the user wants to close the day, reflect, or when it is the end of the workday.
---

# Daily Reflection

Daily reflections make visible where the user worked above expectations and where a ball was dropped, weighed against the expectation per component in `work-evaluation/expectations.md`. Each point gets a backlink in that file, so it can be found again for a weekly review, a check-in or a performance review.

## When

- End of day, during the "🔍 End of Day - Reflection" section of the daily journal
- **Fill in together**: the user shares (text, fragments, answers); the AI coach asks questions, mirrors, structures and makes connections. The user keeps final editorial control: what goes into the journal has to fit them.
- Brief but meaningful; not extensive (that is for weekly reviews)

## Division of roles (fixed)

The AI fills in most of it based on the Daily Flow; the user has final editorial control.

| Section | Who fills it | Notes |
|---|---|---|
| What I Am Proud Of | **User** | Entirely the user's field. The AI never fills this in, not even as a suggestion or example. May stay empty; empty is honest and counts as data. |
| Follow-up questions when unclear | **AI** | When something is unclear, always ask a short follow-up question, also on the pride field if that is needed to sharpen it. |
| What You Can Be Proud Of (outside view) | **AI** | Outside mirror; stay critical, do not exaggerate. On days when the user is a bit too negative about themselves: actively make positive moments visible without flattering. |
| Who Saw You Today? | **AI** | Fill in based on the journal, meetings and connected sources. Positive interaction in a meeting counts just as much as an explicit compliment. Do not invent compliments; truly empty is data. The user may add to it. |
| Short Observation | **AI** | The AI's perspective on the day in 1 to 3 sentences. |
| Above Expectations | **AI** | Weigh strictly against the expectation per component. Empty is a fine outcome. |
| Dropped Balls | **AI** | Genuinely critical, each point with a fix. Candidates that rest on an assumption are presented as a question; the user decides. |
| Carry Into Tomorrow | **AI** | Fill directly from the journal: what came in today that applies tomorrow. |
| Ongoing Reminder | **AI** | Evolving insight for the rest of the week relative to the week kickoff. No day-specific aftermath. |
| Backlinks | **AI** | Pick up directly after the user confirms the reflection text, including `work-evaluation/expectations.md`. |

When in real doubt about a section: ask, do not fill it in.

## Approach

**Step 0: complete the Daily Flow.** If sources are connected (chat, tickets, email), first look at what came in today, as a check on whether the Daily Flow is complete. People forget to pass on small moments of thinking along or helping out; briefly present what was missed and let it land under the right project heading before the reflection sections are filled in. Extract two things: items that need action tomorrow or later (present them, and put them in the task manager) and moments of feedback (an approved PR, a thank you) as candidates for "Who Saw You Today?".

Then use these points to guide the conversation (not to fill everything in yourself):

1. **Profile and behavior**: connect behavior to personality traits (subtly, without naming them explicitly). Read the files in `profile/` for this if that has not been done earlier in the session.

2. **Weighing above expectations**: read `work-evaluation/expectations.md` and lay candidate moments next to the expectation of the component they touch. Apply the criteria from `AGENTS.md` ("Meets vs above expectations" and "Reflection: weigh, don't match") strictly:
   - Which component does this touch, and does it go beyond its description?
   - Is this new behavior, or what the user has shown consistently for years?
   - Is this a breakthrough or just good work?
   - Does this work already belong to someone else's role? If so: not an example.

   **Do not search in order to fill.** *"None today"* is an honest outcome, not a gap that needs filling. A day of good work meets expectations. Better nothing than a forced example.

3. **Patterns over time**: connect current behavior to earlier patterns. Pay attention to meetings and check-ins here too: they often contain recurring themes and external validation that do not stand out on their own in project work.

4. **Dropped balls**: actively look for where the user could have done something differently today, and weigh it according to `AGENTS.md` ("Dropped balls: critical, with a fix"). This is where it may be sharp. But: fact or assumption? For an assumption, ask a question, do not state a conclusion.

5. **Work on learning goals**: did anything today touch one of the learning goals at the top of `expectations.md`? Then mention it briefly in the Short Observation or as a question, without a status. The weekly review picks it up from the Daily Flow.

6. **Behavior vs result**: for each example of above expectations, check who took the initiative. Ask if that is unclear ("Was this your initiative, or did this come through someone else?").

7. **No list of what simply went well**: do not separately name work that meets expectations in daily reflections (that is noise). Save that for the weekly review, where the bigger picture becomes visible.

8. **Knowledge sharing**: did anything pass by today that was actually knowledge sharing but was not recorded as such (briefly helping someone, explaining something)? If so: briefly ask whether it should land under the right project heading in the Daily Flow.

## Filling in the sections

- **What I Am Proud Of**: the user's field. The AI never fills this in, not even as a suggestion.
- **What You Can Be Proud Of (outside view)**: the AI as outside mirror. This field (partly) replaces the feedback that would otherwise have come through colleagues or a manager and is falling away (see `AGENTS.md`, "Being seen"). Name concrete moments from the Daily Flow, not generic ones. Warm, human tone. Does not have to be a learning goal moment and does not have to rise above expectations; "just good work" is fine too. No link to components or learning goals (Above Expectations and Dropped Balls do that). Extra important on heavy days; small is fine.
- **Who Saw You Today?**: two kinds of moments count: someone explicitly reflecting on work ("well done", "this helps", "thanks for X"), and positive interaction in a conversation or meeting in which the user's contribution landed. The second does not have to have ended in a compliment. **A quiet chat channel is not an empty field**: also look at meetings, tickets, email and DMs before writing something down as empty. Do not invent compliments. Leave it empty if it really did not happen; empty is a signal, not a shortfall.
- **Short Observation**: the AI's perspective on the day in 1 to 3 sentences. Core feeling or pattern.
- **Above Expectations ✅**: one line per example, starting with the code of the component: `- **B.02** what I did, and why it goes beyond the expectation. (source of recognition)`. Source of recognition: 👥 who reflected it back and where, 🪞 the user themselves, or 🤖 the journal. *"None today."* is a legitimate outcome.
- **Dropped Balls ⚠️**: one line per point: `- **A.03** what went wrong. Fix: what I will do differently next time.` Short and concrete, not theorizing. *"None today."* is allowed here too, but only after a real search.
- **Carry Into Tomorrow**: fill directly from the journal. Not a task list, but a short intention. Include context: last day before a weekend or vacation, deadlines. Look critically at tasks that have been planned several days in a row without real progress. Name the first appointment of the next workday with time and location; an alarm alone is not always enough.
- **Ongoing Reminder**: evolving insight for the rest of the week relative to the week kickoff. No day-specific aftermath (a choice made on a day belongs in that day's Daily Flow). Open signals, intentions around learning goals, structural points of attention for the week.

## After the reflection

- Apply backlinks **after** the user approves the reflection text.
- Put each point from Above Expectations and Dropped Balls under the right component in `work-evaluation/expectations.md`, in the format used there (date as a link to the daily journal). If a point touches two components, add it to both.
- Add backlinks to the day in the relevant `people/` and `projects/` files, with a short, descriptive sentence. No mechanical backlink for every link in the entire day file.
- Finally, run the `natural-writing` skill over the full day file once more: em-dashes and coined labels creep in while writing.
