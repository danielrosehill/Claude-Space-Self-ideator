# Claude Space Self-Ideator

## Repository Purpose

This repository serves as an ideation space for Claude Space concepts. It contains:
- Examples of existing Claude Spaces
- New ideas for Claude Spaces organized by category
- Documentation on the Claude Space pattern itself
- Guidance on agent portability

## Idea Document Format

When creating new Claude Space ideas in the `ideas/` folder, use this template:

```markdown
# [Space Name]

## Use Case

[2-3 sentences describing the problem this space solves and who would benefit from it]

## Execution Difficulty

**Level**: [Easy | Medium | Hard]

**Rationale**: [1-2 sentences explaining the difficulty rating]

- **Easy**: Simple folder structure, minimal agents, straightforward workflows
- **Medium**: Multiple workflows, 2-3 agents, some complexity in context management
- **Hard**: Complex multi-agent orchestration, sophisticated workflows, significant context engineering

## Suggested Folder Structure

```
[Folder tree diagram - keep to essential folders only, not exhaustive]
```

## Key Workflows

[3-5 bullet points describing the main workflows this space enables]

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/command-name` | Brief description |
| `/command-name` | Brief description |
| `/command-name` | Brief description |

[Include 3-5 essential commands, not exhaustive list]

## Suggested Agents

| Agent | Role |
|-------|------|
| `agent-name` | Brief description of specialization |
| `agent-name` | Brief description of specialization |

[Include 1-3 agents maximum - only if genuinely needed]

## Why This Works as a Claude Space

[2-3 bullet points on what makes this domain suitable for the Claude Space pattern]
```

## Folder Organization

Ideas are organized by category in the `ideas/` folder:

```
ideas/
├── personal-development/
├── learning-skills/
├── relationships-social/
├── creativity-projects/
├── home-life-management/
├── professional-career/
├── mental-emotional-wellbeing/
└── specialized-domains/
```

Each idea is a single markdown file within its category folder.

## Guidelines for Idea Generation

When generating new Claude Space ideas:

1. **Focus on domains with persistent context** - One-shot tasks don't need a space
2. **Identify clear input/output patterns** - What goes in, what comes out
3. **Consider version control value** - Is history useful here?
4. **Keep it practical** - Could someone actually use this?
5. **Avoid over-engineering** - Suggest minimal viable structure
6. **Think about privacy** - Many spaces handle sensitive data

## Difficulty Calibration

Use these benchmarks for difficulty ratings:

| Level | Folders | Agents | Commands | Example |
|-------|---------|--------|----------|---------|
| Easy | 3-5 | 0-1 | 2-4 | Gratitude Practice |
| Medium | 5-10 | 2-3 | 4-8 | Health Helper |
| Hard | 10+ | 3+ | 8+ | Decision Evaluation Framework |

## When Adding Examples

Examples from existing Claude Spaces go in `examples/`. Each should include:
- Link to the source repository
- Brief purpose statement
- Condensed folder structure
- Key agents and commands
- Why it works as a Claude Space
