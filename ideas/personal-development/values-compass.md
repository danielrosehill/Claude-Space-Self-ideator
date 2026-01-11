# Values Compass

## Use Case

Clarify and operationalize personal values. When facing decisions, understand which values are in tension and how past decisions aligned with stated values. Build a lived understanding of what you actually prioritize versus what you say you prioritize.

## Execution Difficulty

**Level**: Easy

**Rationale**: Simple structure focused on reflection and logging. The depth comes from accumulated entries rather than complex workflows.

## Suggested Folder Structure

```
├── values/
│   ├── core-values.md           # Defined and prioritized values
│   ├── definitions.md           # What each value means specifically
│   └── conflicts.md             # Known tensions between values
├── decisions/
│   ├── log/                     # Past decisions and value alignment
│   └── pending/                 # Decisions being contemplated
└── outputs/
    ├── alignment-reports/       # How well life aligns with values
    └── decision-guidance/       # Value-based decision frameworks
```

## Key Workflows

- Define and refine personal values with specific behavioral definitions
- Log significant decisions and analyze which values influenced them
- Identify recurring value conflicts and develop resolution strategies
- Periodic alignment check: are you living your stated values?

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/clarify-value` | Deep dive into defining what a specific value means to you |
| `/log-decision` | Record a decision and analyze its value alignment |
| `/check-alignment` | Generate report on how life choices match stated values |

## Suggested Agents

None required - this space works well with direct Claude interaction.

## Why This Works as a Claude Space

- Values clarification is an ongoing process, not a one-time exercise
- Decision log becomes a rich dataset for pattern recognition
- Seeing past decisions helps calibrate future choices
