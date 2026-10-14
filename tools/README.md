# Tools: reverse lookups

Once you connect external tools to your AI coach (through MCP or another integration), identifiers show up that mean nothing on their own: a project ID from your task manager, a ticket prefix, a service ID in your time tracking. Put one file per tool in this directory that maps such identifiers back to the matching project file in `projects/`. The agent checks this directory before asking you, and adds to it when new projects come along.

Example, `tools/tickets.md`:

```markdown
# Tickets: project key lookup

| Key | Project |
|---|---|
| `SHOP` | [Webshop](../projects/webshop.md) |
| `INT` | [Internal tools](../projects/internal-tools.md) |
```

Keep the files small: only the mapping and a note where it is not obvious (for example two keys that point to the same project). Remove this README once you have your own lookups, or leave it in as an explanation.
