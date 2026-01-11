# Creative Project Manager

## Use Case

Manage creative projects (writing, art, music, video) with ideation, iteration tracking, feedback integration, and process documentation. Brings structure to inherently messy creative work without killing spontaneity.

## Execution Difficulty

**Level**: Medium

**Rationale**: Multiple projects with multiple iterations each. Requires discipline in tracking but individual operations are simple.

## Suggested Folder Structure

```
├── projects/
│   └── [project-name]/
│       ├── concept.md           # Project vision
│       ├── iterations/          # Versions and drafts
│       ├── feedback/            # External feedback
│       └── status.md            # Current phase
├── pipeline/
│   ├── ideation/                # Ideas being explored
│   ├── active/                  # In progress
│   └── completed/               # Finished projects
└── outputs/
    ├── portfolio/               # Finished work
    └── process-docs/            # Creative process documentation
```

## Key Workflows

- Initiate new projects with clear vision and success criteria
- Track iterations with notes on what changed and why
- Integrate external feedback systematically
- Move projects through pipeline stages
- Document creative process for future reference

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/new-project` | Initialize a new creative project |
| `/log-iteration` | Record a new version with change notes |
| `/integrate-feedback` | Process and incorporate external feedback |
| `/retrospective` | Document lessons from completed project |

## Suggested Agents

| Agent | Role |
|-------|------|
| `creative-critic` | Provides structured feedback on work in progress |

## Why This Works as a Claude Space

- Creative work involves many iterations
- Feedback integration benefits from structured process
- Process documentation enables future creative growth
