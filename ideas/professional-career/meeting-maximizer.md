---
name: "Meeting Maximizer"
category: "professional-career"
description: "Prepare for meetings, capture outcomes, and track action items"
duration: "ongoing"
difficulty: "easy"
---

# Meeting Maximizer

## Use Case

Prepare for meetings, capture outcomes, track action items, and analyze meeting patterns. Transform meetings from time sinks into productive interactions with clear outcomes and follow-through.

## Execution Difficulty

**Level**: Easy

**Rationale**: Each meeting is a self-contained unit. Simple logging and retrieval patterns.

## Suggested Folder Structure

```
├── meetings/
│   └── [meeting-id]/
│       ├── agenda.md            # Meeting agenda
│       ├── preparation.md       # Pre-meeting prep
│       ├── notes.md             # Meeting notes
│       └── action-items.md      # Assigned actions
├── recurring/
│   └── [meeting-name]/
│       └── history/             # Past meeting records
├── action-items/
│   └── mine/                    # My action items
└── outputs/
    └── patterns/                # Meeting effectiveness analysis
```

## Key Workflows

- Prepare for meetings with research and agenda review
- Capture notes and action items during/after meetings
- Track action items to completion
- Maintain history for recurring meetings
- Analyze meeting patterns to improve effectiveness

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/prepare-meeting` | Generate preparation brief for upcoming meeting |
| `/capture-notes` | Structured note capture during/after meeting |
| `/extract-actions` | Pull action items from meeting notes |
| `/meeting-audit` | Analyze meeting patterns and effectiveness |

## Suggested Agents

None required - straightforward workflows that work well with direct interaction.

## Why This Works as a Claude Space

- Meeting preparation benefits from past context
- Recurring meetings need accessible history
- Action item tracking prevents dropped balls
