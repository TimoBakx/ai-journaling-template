# 📚 AI-Powered Journalling & Personal Growth System

A structured system for personal and professional development through daily journalling with AI support. This template helps you make growth visible, recognize patterns and capture meaningful reflections.

There is also a [Dutch version](https://github.com/TimoBakx/ai-journaling-template-nl).

## 🎯 Purpose

This journalling system is designed to:
- **Track personal and professional growth** through structured reflection
- **Preserve insights** from daily experiences, conversations and learning moments
- **Recognize patterns** in your thinking, behavior and development
- **Collaborate with AI** for improved self-knowledge and guidance
- **Build a searchable archive** of your thoughts and learning experiences
- **Make growth visible** for evaluations, conversations and career development

### 💡 Why This System?

Subtle but valuable growth often remains invisible in traditional evaluation systems. Through systematic documentation of:
- **Daily experiences** and concrete events
- **Growth moments** and breakthroughs (large and small)
- **Patterns** in your behavior, thinking and collaboration
- **Skills evolution** over time

You create an **evidence base** that shows your actual development. This approach helps you not only understand yourself better, but also make your value and growth visible to others.

## 🗂️ Structure

```
notes/
├── .cursor/
│   └── rules/                 # AI Coach configuration and rules
│       ├── ai-coach-personality.mdc  # Personality and character of your AI coach
│       ├── ai-coach-role.mdc         # Role and functions of your AI coach
│       ├── general-rules.mdc         # Project structure and workflow
│       ├── userprofile.mdc           # Reference to profile directory
│       ├── journalling-rules.mdc     # Daily journalling workflow
│       ├── reflection-rules.mdc      # End of day reflection methodology
│       └── evaluation-rules.mdc      # Weekly evaluation approach
├── profile/                   # Personal assessments and profiles (optional)
│   ├── big-five.md            # Big Five personality assessment
│   ├── disc.md                # DISC behavioral analysis  
│   ├── human-design.md        # Human Design body graph
│   ├── neurodivergence.md     # Neurodivergent traits
│   └── professional.md        # Professional background and expertise
├── work-evaluations/          # Performance reviews and growth plans (optional)
│   ├── [DATE]-annual-review.md            # Annual reviews
│   ├── [DATE]-half-year-checkin.md        # Half-year check-ins
│   └── persoonlijke-groei-plan-[YEAR].md  # Growth plans
├── journal/                   # Daily journalling and reflection
│   ├── [YEAR]/                # Year directory (e.g. 2025/)
│   │   └── [WEEK]/            # Week directory (e.g. 45/)
│   │       ├── 1-monday-[YEAR]-[MONTH]-[DAY].md
│   │       ├── 2-tuesday-[YEAR]-[MONTH]-[DAY].md
│   │       ├── 3-wednesday-[YEAR]-[MONTH]-[DAY].md
│   │       ├── 4-thursday-[YEAR]-[MONTH]-[DAY].md
│   │       ├── 5-friday-[YEAR]-[MONTH]-[DAY].md
│   │       ├── week-evaluation.md        # Weekly reflection
│   │       └── checkin.md (optional)     # For conversations with supervisor
│   ├── daily-journal-template.md         # Template for daily entries
│   ├── weekly-review-template.md         # Template for week evaluations
│   └── checkin-template.md               # Template for check-in reports
├── projects/                  # Project context and documentation (optional)
│   ├── _template.md           # Template for new projects
│   └── [project-name].md      # Project details and reflections
└── people/                    # Colleagues and collaboration partners (optional)
    ├── _template.md           # Template for new people
    └── [name].md              # Notes about individuals
```

### 📅 Week Structure Example

Each week follows a consistent structure within `journal/[YEAR]/[WEEK_NUMBER]/`:

```
journal/2025/45/
├── 1-monday-2025-11-03.md
├── 2-tuesday-2025-11-04.md
├── 3-wednesday-2025-11-05.md
├── 4-thursday-2025-11-06.md
├── 5-friday-2025-11-07.md
└── week-evaluation.md
```

Week numbers follow the ISO 8601 standard (use `date +%V` on Unix systems).

## 🚀 Getting Started

### 1. Configure Your AI Coach
Adjust the AI Coach configuration in `.cursor/rules/`:
- **`ai-coach-personality.mdc`** - Define the character and emotional attitude of your AI coach
- **`ai-coach-role.mdc`** - Determine the function and activities of your AI coach within this project
- **`general-rules.mdc`** - Basic project structure and workflow (adjust to your situation)
Many placeholders are in [square brackets], adjust those especially (except for template files).

### 2. (Optional) Fill In Your Profiles
The `profile/` directory helps your AI coach understand you better:
- **`big-five.md`** - Big Five personality assessment
- **`disc.md`** - DISC behavioral analysis  
- **`human-design.md`** - Human Design body graph
- **`neurodivergence.md`** - Neurodivergent traits
- **`professional.md`** - Professional background and expertise

The more context your AI coach has, the better the guidance!

### 3. Start Journalling
Start your first daily journal entry:
1. Create a directory structure: `journal/[YEAR]/[WEEK_NUMBER]/`
2. Use `journal/daily-journal-template.md` for your first entry
3. Share your thoughts, experiences and events with your AI coach
4. Reflect together at the end of the day

### 4. Weekly Evaluation
At the end of each week:
1. Use `journal/weekly-review-template.md` for your weekly evaluation
2. Analyze patterns and insights with your AI coach
3. Link experiences to your growth goals (if applicable)
4. Prepare check-ins with supervisors (if desired)

### 5. (Optional) Use People & Projects
- **`people/`** - Document colleagues, collaboration patterns and team dynamics
- **`projects/`** - Keep project context and link to journal entries
- **`work-evaluations/`** - Store performance reviews and growth plans

## 🤝 Collaboration with AI

This system is designed to work seamlessly with AI support (such as Cursor, ChatGPT, Claude):
- **Context-rich conversations** - Your profiles and history provide deeper understanding
- **Pattern recognition** - AI helps identify trends in your thoughts and growth
- **Personalized guidance** - Recommendations based on your specific situation
- **Structured reflection** - Frameworks for meaningful growth
- **Memory function** - Refer back to earlier notes and patterns

## 📝 Journalling Workflow

### Daily Routine
1. **Start your day** - Fill in the "🎯 Planned" section with your tasks
2. **Throughout the day** - Add events to "📝 Daily Flow"
3. **End of day** - Reflect together with your AI coach in "🔍 End of Day - Reflection"
4. **Tasks for Later** - Note what doesn't happen today

### Natural Flow
- **Be authentic** - share what's on your mind, without filter
- **No perfection needed** - rough thoughts are fine, structure comes naturally
- **Ask follow-up questions** - let your AI coach help with clarification
- **Make connections** - link to projects, people and earlier entries

### AI Coach Role
Your AI coach helps you with:
- Organizing thoughts into structured notes
- Asking clarifying questions to deepen insights  
- Making connections between events and growth patterns
- Recognizing patterns over time
- Making senior skills and competencies visible

## 🔍 Tips & Best Practices

### Cross-Referencing
- **Link to projects**: `([Project](../../projects/project.md))` in headers and tasks
- **Link to people**: `[Name](../../people/name.md)` in your notes
- **Link to earlier entries**: Refer to patterns and earlier moments

### Consistency
- Use the templates for daily and weekly entries
- Follow the week structure: `journal/[YEAR]/[WEEK_NUMBER]/`
- File naming: `[DAY_NUMBER]-[day]-[YEAR]-[MONTH]-[DAY].md`

### Depth
- Be specific in your observations - concrete examples work better than general statements
- Ask follow-up questions with your AI coach if something is unclear
- Link events to your growth goals (if applicable)

## 🌱 Philosophy

This journalling approach is built on:
- **Safety** - this is your safe space for growth and reflection
- **Honesty** - authentic sharing without filter or judgment
- **Patience** - growth takes time, small steps count
- **Curiosity** - keep learning and discovering, ask questions
- **Visibility** - make invisible growth explicit and tangible

---

## 🎯 Adapting For Your Situation

This template is a **starting point** - adapt it to your needs:
- Add extra sections to the daily template that work for you
- Create custom directories for your specific context
- Adjust the AI coach rules to your preferences
- Experiment with what works and what doesn't

**Most important tip**: Start simple, iterate and refine as you learn more about what you need!

---

*Good luck with your growth journey! 🚀✨*
