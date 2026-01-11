---
name: "Travel Planner"
category: "specialized-domains"
description: "Comprehensive trip planning from research through execution and memory capture"
duration: "time-limited"
difficulty: "medium"
---

# Travel Planner

## Use Case

Comprehensive trip planning from research through execution and memory capture. Consolidate the scattered process of travel planning into one workspace that remembers your preferences and past trips.

## Execution Difficulty

**Level**: Medium

**Rationale**: Multiple phases per trip (research, planning, execution, memories) but well-defined workflows for each.

## Suggested Folder Structure

```
├── trips/
│   └── [trip-name]/
│       ├── research/            # Destination research
│       ├── itinerary/           # Day-by-day plans
│       ├── bookings/            # Confirmation details
│       └── memories/            # Post-trip photos/notes
├── preferences/
│   ├── accommodation.md
│   └── activities.md
└── outputs/
    └── itineraries/             # Shareable itineraries
```

## Key Workflows

- Research destinations with structured comparison
- Generate itineraries based on interests and constraints
- Organize booking confirmations and travel documents
- Create shareable itineraries for travel companions
- Capture trip memories and lessons for future trips

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/plan-trip` | Initialize new trip planning |
| `/research-destination` | Structured destination research |
| `/generate-itinerary` | Create day-by-day itinerary |
| `/trip-debrief` | Post-trip capture of memories and lessons |

## Suggested Agents

| Agent | Role |
|-------|------|
| `itinerary-builder` | Generates balanced itineraries based on interests and logistics |

## Why This Works as a Claude Space

- Preferences carry across trips
- Past trips inform future planning
- All trip info consolidated in one searchable place
