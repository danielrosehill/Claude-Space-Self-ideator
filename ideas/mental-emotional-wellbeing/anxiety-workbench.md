# Anxiety Workbench

## Use Case

Structured anxiety management using CBT techniques - identifying triggers, challenging thoughts, planning exposures. Bring the tools of therapy into daily practice with consistent tracking and pattern recognition.

## Execution Difficulty

**Level**: Medium

**Rationale**: Requires honest self-reflection and consistent logging. The techniques are well-defined but application takes practice.

## Suggested Folder Structure

```
├── profile/
│   ├── triggers.md              # Known triggers
│   ├── patterns.md              # Anxiety patterns
│   └── coping-strategies.md     # What helps
├── episodes/
│   └── [date]/
│       ├── situation.md         # What happened
│       ├── thoughts.md          # Automatic thoughts
│       └── challenge.md         # Thought challenges
├── exposures/
│   ├── hierarchy.md             # Exposure hierarchy
│   └── completed/               # Exposure records
└── outputs/
    └── progress/                # Progress tracking
```

## Key Workflows

- Log anxiety episodes with situation, thoughts, and physical sensations
- Challenge automatic thoughts using CBT techniques
- Build and work through exposure hierarchy
- Identify patterns across episodes
- Track progress and update coping strategies

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/log-episode` | Record anxiety episode with structured prompts |
| `/challenge-thought` | Walk through cognitive restructuring |
| `/plan-exposure` | Design next exposure exercise |
| `/review-patterns` | Analyze patterns across episodes |

## Suggested Agents

| Agent | Role |
|-------|------|
| `thought-challenger` | Guides through cognitive restructuring process |

## Why This Works as a Claude Space

- Anxiety patterns only visible over time
- Progress tracking maintains motivation
- Highly private - must stay local
