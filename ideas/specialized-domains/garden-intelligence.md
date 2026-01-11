# Garden Intelligence

## Use Case

Garden planning, plant care tracking, pest management, and harvest optimization. Bring systematic observation and learning to gardening with records that accumulate wisdom over seasons.

## Execution Difficulty

**Level**: Medium

**Rationale**: Seasonal cycles and multiple plants to track. Benefits from consistent logging but not complex.

## Suggested Folder Structure

```
├── garden/
│   ├── layout.md                # Garden zones
│   ├── soil.md                  # Soil conditions
│   └── climate.md               # Microclimate details
├── plants/
│   └── [plant-name]/
│       ├── profile.md           # Requirements
│       └── care-log/            # Care history
├── calendar/
│   ├── planting/                # Planting schedule
│   └── harvest/                 # Harvest timing
└── outputs/
    └── seasonal-plans/          # Season planning docs
```

## Key Workflows

- Document plants with care requirements and observations
- Log care activities and plant responses
- Track issues (pests, diseases) and treatments
- Plan seasonal activities based on climate and history
- Analyze what worked and didn't across seasons

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/log-observation` | Record plant observation or care activity |
| `/diagnose-issue` | Identify and research plant problem |
| `/plan-season` | Generate seasonal planting and care plan |
| `/harvest-check` | Check what's ready for harvest |

## Suggested Agents

| Agent | Role |
|-------|------|
| `plant-doctor` | Diagnoses plant issues and suggests treatments |

## Why This Works as a Claude Space

- Garden wisdom accumulates over seasons
- Care logs reveal patterns invisible in the moment
- Plant profiles become personalized care guides
