---
name: add-project
description: Add a project to the repo. Use when the user starts a new project or wants to record an existing project in `projects/`. First asks whether it is a new or an existing project and routes accordingly.
---

# Add Project

Workflow for creating a project file in `projects/`, connecting it to external tools and recording the working agreements.

## When

- The user starts a new project or engagement
- The user wants to document an existing (ongoing) project after all
- The user explicitly asks to add a project

## Steps

### 1. New or existing?

First ask explicitly: **is this a new project (we are starting the engagement now) or an existing project (it is already running and we are recording it after all)?**

This mainly determines how step 5 (working agreements) is filled in:
- **New**: we *shape* the working agreements together, before the engagement really starts.
- **Existing**: we *record* which working agreements already exist, so the coach can remind the user of them later.

### 2. Purpose & basic details

- **Project name** (and the file name in kebab-case, e.g. `new-client.md`)
- **Purpose**: what is the software trying to solve? The core of why this project exists.
- **Type**: web application, API, plugin, etc.
- **Involvement**: since when, in which role
- **Status**: ongoing, new, on hold, etc.

### 3. People

- **Team members**: who from the user's own organization is on it and in which role, plus the user's own role. (Colleagues have a file in `people/`.)
- **Contacts (client)**: the external stakeholders: name, role, and how the collaboration goes. These belong under the `## External Contacts` section in the project file, not in `people/`.

### 4. Sensitive data (optional)

If the organization works with ISO, the GDPR or comparable frameworks, ask explicitly: **does this project process sensitive information? (yes/no)**. If yes: briefly note what kind (personal data, client data, credentials). This is a flag, not a full analysis, but something that has to be visible as soon as the project comes up in that context.

### 5. Working agreements (Way of Work)

*These agreements are reference information the coach uses to remind the user of things later when the project is discussed. So record them for new and existing projects alike.* Clear agreements at the start of an engagement prevent most of the trouble later.

Go through the working agreements and record them under the **Way of Work** section in the project file:

- How do we treat each other?
- What do we expect in terms of how tickets are delivered?
- What can they expect from us in terms of advice and thinking along?
- How do we handle urgent bugs?
- Do we work in sprints, or deliberately not?

For a **new** project: use this as material for the conversation to sharpen the agreements; mark what is not known yet as an open point to align with the client. For an **existing** project: record what the actual agreements are now. Do not tick boxes mechanically.

### 6. Links & integrations

- **Tickets**: project key and link to the board
- **Chat**: the project channel or relevant DM context
- **Tasks**: which project in the task manager belongs to this? See `tools/` for the existing IDs.
- Any other relevant links (repository, environments, documentation).

### 7. Create the project file

Create `projects/[name].md` based on `projects/_template.md`. Fill in the known sections, leave out optional sections that do not fit. Keep it brief: the project file is a dashboard with context and pointers; the details are in the journals.

### 8. Update the reverse lookups

Add the new identifiers (ticket key, project ID in the task manager) to the files in `tools/`, so the agent can place them on its own later.

## Loading context

At the start, read `AGENTS.md` (project structure, external contacts, task management) and `projects/_template.md`. Keep to the writing style: brief, concrete, no coined labels.
