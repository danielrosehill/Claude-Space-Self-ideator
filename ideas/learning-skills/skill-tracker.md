# Skill Tracker

## Use Case

Track skill development across multiple competencies with deliberate practice planning and progress visualization. Moves beyond vague "I want to get better" to structured practice with measurable progress.

## Execution Difficulty

**Level**: Easy

**Rationale**: Simple logging structure with periodic assessment. Complexity comes from consistency, not architecture.

## Suggested Folder Structure

```
├── skills/
│   └── [skill-name]/
│       ├── current-level.md     # Self-assessment
│       ├── target-level.md      # Goals
│       └── practice-log/        # Session records
├── practice/
│   ├── scheduled/               # Planned sessions
│   └── completed/               # Completed sessions
└── outputs/
    └── progress-reports/        # Skill progression over time
```

## Key Workflows

- Define skills with clear level descriptions and targets
- Log deliberate practice sessions with specific focus areas
- Periodic self-assessment against defined criteria
- Identify plateaus and generate breakthrough strategies
- Celebrate milestones and update targets

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/assess-skill` | Run structured self-assessment for a skill |
| `/log-practice` | Record a deliberate practice session |
| `/identify-plateau` | Analyze recent progress and suggest interventions |

## Suggested Agents

None required - direct Claude interaction works well for this simple structure.

## Why This Works as a Claude Space

- Skill development is inherently long-term
- Practice logs become data for pattern recognition
- Seeing progress trajectory maintains motivation
