# Habit Laboratory

## Use Case

Systematic habit formation and tracking using behavioral science principles. Goes beyond simple habit tracking to understand why habits stick or fail, running experiments on behavior change with structured observation and iteration.

## Execution Difficulty

**Level**: Medium

**Rationale**: Requires thoughtful experiment design and multi-week tracking, but the core workflows are straightforward once established.

## Suggested Folder Structure

```
├── context/
│   ├── personal-profile.md      # Energy cycles, constraints, lifestyle
│   └── behavioral-triggers.md   # Known triggers and environments
├── experiments/
│   ├── active/                  # Currently running experiments
│   └── completed/               # Experiments with documented outcomes
├── tracking/
│   ├── daily-logs/              # Daily check-ins
│   └── weekly-reviews/          # Weekly analysis
└── outputs/
    ├── analyses/                # Pattern identification
    └── recommendations/         # Suggested adjustments
```

## Key Workflows

- Design and launch new habit experiments with clear success criteria
- Daily check-ins that capture context, not just completion
- Weekly reviews that identify patterns and adjust approach
- Post-mortem analysis of failed habits to extract lessons
- Environment design suggestions based on behavioral science

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/start-experiment` | Launch a new habit experiment with hypothesis and success criteria |
| `/daily-checkin` | Log today's habit performance with contextual notes |
| `/weekly-review` | Analyze the past week and generate insights |
| `/analyze-failure` | Deep dive into why a habit didn't stick |

## Suggested Agents

| Agent | Role |
|-------|------|
| `behavior-analyst` | Identifies patterns across experiments and suggests evidence-based interventions |
| `environment-designer` | Suggests environmental and contextual changes to support habit formation |

## Why This Works as a Claude Space

- Habit formation spans weeks/months - persistent context is essential
- Patterns only emerge from accumulated data over time
- The behavioral science literature provides rich frameworks for analysis
