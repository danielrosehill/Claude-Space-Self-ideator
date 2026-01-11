# Pet Care

## Use Case

Comprehensive pet care management - health records, behavior tracking, routine management, and care coordination. Keep all pet information in one place with institutional memory that survives human forgetfulness.

## Execution Difficulty

**Level**: Easy

**Rationale**: Straightforward logging with clear categories. Simple structure, high value from consistency.

## Suggested Folder Structure

```
├── pets/
│   └── [pet-name]/
│       ├── profile.md           # Breed, age, traits
│       ├── health/
│       │   ├── records.md       # Vet visits
│       │   └── medications.md   # Current meds
│       ├── behavior/            # Behavior observations
│       └── diet.md              # Feeding schedule
├── vets/
│   └── [vet-name]/              # Vet contact and history
└── outputs/
    └── care-guides/             # Pet sitter instructions
```

## Key Workflows

- Maintain pet profiles with health history
- Log vet visits with diagnoses and treatments
- Track medications and vaccination schedules
- Observe and document behavior patterns
- Generate care instructions for pet sitters

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/log-vet-visit` | Record vet visit with details |
| `/track-behavior` | Log behavior observation |
| `/prepare-boarding` | Generate care instructions for sitter |
| `/health-check` | Review upcoming health needs |

## Suggested Agents

None required - simple structure works well with direct interaction.

## Why This Works as a Claude Space

- Health history essential for vet visits
- Behavior logs reveal patterns over time
- Care guides ensure consistent care from anyone
