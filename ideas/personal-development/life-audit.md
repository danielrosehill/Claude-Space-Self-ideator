# Life Audit

## Use Case

Periodic comprehensive review of all life domains - career, relationships, health, finances, personal growth, creativity, contribution. Based on the "wheel of life" framework but with AI-assisted deep analysis and trend tracking over time.

## Execution Difficulty

**Level**: Medium

**Rationale**: Covers many domains but each follows a similar assessment pattern. The challenge is maintaining consistency in periodic reviews.

## Suggested Folder Structure

```
├── domains/
│   ├── career.md
│   ├── relationships.md
│   ├── health.md
│   ├── finances.md
│   ├── personal-growth.md
│   ├── creativity.md
│   └── contribution.md
├── audits/
│   ├── quarterly/               # Quarterly life audits
│   └── annual/                  # Annual deep reviews
├── goals/
│   └── by-domain/               # Domain-specific goals
└── outputs/
    ├── scorecards/              # Satisfaction scores over time
    └── action-plans/            # Concrete next steps
```

## Key Workflows

- Quarterly structured review of each life domain with scoring
- Trend analysis showing domain trajectories over time
- Goal alignment checks across domains
- Action plan generation with prioritization
- Annual comprehensive review with year-over-year comparison

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/quarterly-audit` | Run full quarterly life assessment |
| `/update-domain` | Quick update to a single domain |
| `/visualize-progress` | Generate trend visualization across domains |
| `/align-goals` | Check goal coherence across life areas |

## Suggested Agents

| Agent | Role |
|-------|------|
| `life-coach` | Asks probing questions and identifies blind spots in self-assessment |

## Why This Works as a Claude Space

- Life trends only visible with longitudinal data
- Version control shows personal evolution over years
- Structured format enables meaningful comparison across time periods
