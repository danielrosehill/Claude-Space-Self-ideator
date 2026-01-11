# Learning Lab

## Use Case

Structured self-directed learning with spaced repetition, comprehension testing, and knowledge integration. Transforms passive consumption of learning materials into active, testable understanding with connections across subjects.

## Execution Difficulty

**Level**: Medium

**Rationale**: Requires organization of multiple subjects and implementation of review scheduling, but individual workflows are straightforward.

## Suggested Folder Structure

```
├── subjects/
│   └── [subject-name]/
│       ├── source-materials/    # Books, articles, courses
│       ├── notes/               # Processed notes
│       └── questions/           # Comprehension questions
├── reviews/
│   ├── due/                     # Items due for review
│   └── completed/               # Review history
└── outputs/
    ├── summaries/               # Subject summaries
    └── connections/             # Cross-subject links
```

## Key Workflows

- Add new learning materials and generate comprehension questions
- Spaced repetition review sessions based on forgetting curve
- Generate "teach it back" explanations to verify understanding
- Identify connections between subjects and synthesize knowledge
- Track mastery progression over time

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/add-material` | Process new learning material and generate questions |
| `/review-session` | Run a spaced repetition review |
| `/teach-back` | Generate explanation as if teaching someone else |
| `/find-connections` | Identify links between subjects |

## Suggested Agents

| Agent | Role |
|-------|------|
| `question-generator` | Creates comprehension and application questions from source material |
| `knowledge-integrator` | Finds connections across subjects and synthesizes insights |

## Why This Works as a Claude Space

- Learning effectiveness depends on spaced repetition over time
- Questions and connections accumulate into valuable knowledge base
- Version control tracks learning progression
