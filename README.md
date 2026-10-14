# 📚 AI-Powered Journaling & Personal Growth System

A structured system for personal and professional development through daily journaling with an AI coach. This template helps you show what you do, weighed against what your role asks of you, recognize patterns, and record reflections you can actually use in a performance review.

There is also a [Dutch version](https://github.com/TimoBakx/ai-journaling-template-nl).

## 🎯 Purpose

This journaling system is designed to:
- **Make your work visible**, weighed against the expectations and responsibilities of your role
- **Preserve insights** from daily experiences, conversations and learning moments
- **Recognize patterns** in your thinking, behavior and collaboration
- **Collaborate with AI** as a sparring partner with a critical eye
- **Build a searchable archive** of your thoughts and learning experiences
- **Prepare performance reviews** with concrete, dated examples

### 💡 Why this system?

Subtle but valuable development often remains invisible. What you did well in March, you no longer remember precisely in September, and a conversation about your performance then runs on impressions instead of facts. By briefly recording every day what happened, and strictly weighing at the end of the day and the week what was above expectations and where you dropped the ball, you build a record that shows your actual development.

The AI coach is not a note taker but a sparring partner: it asks follow-up questions when something is too vague, mirrors patterns you do not see yourself, and is critical when you label something as growth too easily.

## 🗂️ Structure

```
notes/
├── AGENTS.md                  # AI Coach instructions (role, guidelines, way of working)
├── CLAUDE.md                  # Imports AGENTS.md for Claude Code
├── .claude/skills/            # Workflows as skills
│   ├── start-day/             # Start of the workday
│   ├── reflection/            # End of day reflection
│   ├── weekly-review/         # Weekly review and next week's kickoff
│   ├── add-project/           # Record a project, including working agreements
│   └── natural-writing/       # Writing style: human, concrete, no AI patterns
├── journal/                   # Daily journaling and reflection
│   ├── [YEAR]/[WEEK]/
│   │   ├── 0-kickoff-week-[WEEK].md     # Guiding overview for the week
│   │   ├── 1-monday-[YEAR]-[MONTH]-[DAY].md
│   │   ├── ...
│   │   ├── 5-friday-[YEAR]-[MONTH]-[DAY].md
│   │   ├── week-evaluation.md           # Weekly reflection
│   │   └── checkin.md (optional)        # For conversations with your manager
│   ├── daily-journal-template.md
│   ├── weekly-kickoff-template.md
│   ├── weekly-review-template.md
│   └── checkin-template.md
├── work-evaluation/
│   ├── expectations.md        # The active state: learning goals, expectation and assessment per component of your role
│   └── archive/               # Conversation reports, self-evaluations and earlier versions of expectations.md
├── profile/                   # Personal assessments (optional)
│   ├── big-five.md
│   ├── disc.md
│   ├── human-design.md
│   ├── neurodivergence.md
│   └── professional.md
├── projects/                  # Project context (optional)
│   ├── _template.md
│   └── [project-name].md
├── people/                    # Colleagues and collaboration partners (optional)
│   ├── _template.md
│   └── [name].md
└── tools/                     # Reverse lookups of identifiers in external tools (optional)
    └── README.md
```

### 📅 Week structure example

```
journal/2026/45/
├── 0-kickoff-week-45.md
├── 1-monday-2026-11-02.md
├── 2-tuesday-2026-11-03.md
├── 3-wednesday-2026-11-04.md
├── 4-thursday-2026-11-05.md
├── 5-friday-2026-11-06.md
└── week-evaluation.md
```

Week numbers follow the ISO 8601 standard (use `date +%V` on Unix systems).

## 🚀 Getting started

### 1. Configure your AI coach

All instructions live in `AGENTS.md`: the role of the coach, the guidelines for journaling, reflection and evaluation, and how strictly things are weighed. Go through the file and fill in the placeholders in [brackets], at least:

- **Tone & personality**: how do you want the coach to feel?
- **Main goal**: where is your focus?
- **Being seen**: what is your fuel at work, and what are the signals that it is falling away?
- **Tooling & integrations**: which tools do you connect, if any?

`AGENTS.md` is the open standard most tools read (Cursor, VS Code with Copilot, Codex, Aider, Zed and others). Claude Code reads `CLAUDE.md`, which imports the file. The workflows in `.claude/skills/` are Claude Code skills; if you use another tool, you can take the content of each `SKILL.md` over as a rule or paste it into your instruction file.

### 2. Record the expectations of your role

Fill in `work-evaluation/expectations.md`: the components of your role (from your organization's job profile or competency framework, or your own list of responsibilities if there is none), per component the expectation at your level and the latest assessment from a conversation, and your learning goals. This file is the yardstick for the daily reflection and the weekly review.

Conversation reports, self-evaluations and old growth plans go into `work-evaluation/archive/`. After every conversation, `expectations.md` goes into the archive as a snapshot and a new version starts with the new assessment.

### 3. (Optional) Fill in your profiles

The `profile/` directory helps your AI coach understand you better: Big Five, DISC, Human Design, neurodivergence and professional background. The more context, the sharper the coaching. None of this is required.

### 4. Start journaling

1. Start the day with the `start-day` skill (or ask your coach to start the day): it creates the daily file, looks at the week kickoff, the previous day and, if connected, your task manager and calendar, and lays your learning goals alongside the planning.
2. Share what you are doing throughout the day. The coach processes it in the Daily Flow and asks follow-up questions when something is still too vague to read back usefully later.
3. Close the day with the `reflection` skill: you fill in "What I Am Proud Of", the coach fills in the rest, you have the final say. The weighing (above expectations, dropped balls) gets backlinks in `expectations.md`.

### 5. Weekly review

At the end of the week, in its own session, with the `weekly-review` skill: patterns across the days, work on the learning goals, the week's weighing per component, and to close, the kickoff for next week.

### 6. (Optional) People & projects

- **`projects/`**: context per project, including the working agreements at the start (the `add-project` skill walks through them)
- **`people/`**: colleagues, collaboration patterns and team dynamics
- **`tools/`**: which identifier in which external tool belongs to which project

### 7. (Optional) Connect your tools

The system works without integrations. If you connect a task manager, calendar, ticket system, chat or email through MCP, the coach uses them to fill the planning, complete the daily flow and find feedback moments. The rules for that are in `AGENTS.md` under "Tooling & integrations": reading may be proactive, writing only on request, and the journal stays the primary place.

## ⚖️ Meets or above expectations

The biggest lesson from a year of journaling: weighing against "growth" does not work. Growth is vague, and an AI coach that looks for growth finds it everywhere. This system therefore weighs against the **expectation per component of your role**:

- **Meets expectations** is what the description of the component asks for. Good work that belongs to your role. A fine outcome, and on most days that is all there is.
- **Above expectations** is the extra step beyond that description: new behavior, application in a new context, an improvement that reaches further than your own work. Only on your own initiative, and with a source of recognition: who saw this (👥 a colleague, 🪞 yourself, 🤖 the journal)?
- **Dropped balls** are where you could have done something differently yourself, always with a concrete fix for next time.

Learning goals have no status. The only question is whether you worked on them this week, and how. "Not this week" is a normal outcome, and a week without an example of above expectations can be a good week.

## 🔍 Tips

### Cross-referencing
- **Link to projects**: `([Project](../../../projects/project.md))` in headers and tasks
- **Link to people**: `[Name](../../../people/name.md)` in your notes
- **Link to earlier entries**: refer to patterns and earlier moments

### Consistency
- Use the templates for daily and weekly entries
- One session per day, and a separate session for the weekly review, so that yesterday's assumptions do not bleed into today unnoticed
- The journal is the primary place; a task manager is supporting

### Depth
- Be specific: concrete examples work better than general statements
- Let the coach ask follow-up questions when something is unclear, and correct it when it fills in something that is wrong
- Write your external texts (emails, messages) yourself and have the coach review them; that keeps you sharper than having a draft written

## 🌱 Philosophy

- **Safety**: this is your space for reflection
- **Honesty**: share authentically, and weigh strictly
- **Patience**: development takes time, small steps count
- **Curiosity**: keep asking questions
- **Visibility**: make explicit and tangible what otherwise stays invisible

## 🔄 What changed since the first version

The first version of this template (November 2025) was built on Cursor rules and on looking for "growth". A year of daily use produced these changes:

- **From growth to expectations.** The journal weighs against the expectation per component of your role in `work-evaluation/expectations.md`, not against a vague picture of growth. Learning goals no longer have a status.
- **Dropped balls, with a fix.** Next to above expectations, the journal tracks where you could have done something differently yourself, and what you will do differently next time.
- **Source of recognition.** Every example of above expectations marks who saw it, so the journal does not become a closed loop that confirms itself.
- **Questions instead of filling in.** The coach does not present an assumption as a missed signal; it asks a question. That difference decides whether you get defensive or start thinking more broadly.
- **Weigh, don't match.** Five fixed pitfalls when weighing, and the rule: do not search in order to fill.
- **Being seen.** "Who saw you today?" and an outside view in the reflection, because whoever does more and more themselves loses, without noticing, the feedback that used to come naturally.
- **Timing of coaching.** During the day, only follow-up questions to complete the note; weighing and patterns belong to the reflection and the weekly review.
- **One session per day.** So that yesterday's assumptions do not bleed into today.
- **The week kickoff.** A guiding document at the start of the week, not a task list.
- **Working agreements per project.** Record the Way of Work at the start of an engagement.
- **Writing style.** The `natural-writing` skill against AI patterns, and no coined labels.
- **Tooling.** From Cursor rules to `AGENTS.md` and skills, and optional integrations with task manager, calendar, tickets and chat.

## 🎯 Adapting to your situation

This template is a starting point:
- Remove what you do not use; profiles, people, projects and tools are all optional
- Adapt `AGENTS.md` to your preferences and your role
- Experiment with what works and what does not

Start simple, and refine as you learn more about what you need.
