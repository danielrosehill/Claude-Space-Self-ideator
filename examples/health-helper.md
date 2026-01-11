# Claude Health Helper

**Repository**: [Claude-Health-Helper](https://github.com/danielrosehill/Claude-Health-Helper)

## Purpose
Organized workspace for personal health documentation management. Helps users make the most of healthcare visits by organizing health information, converting transcripts to structured summaries, and preparing symptom lists for consultations.

## Core Structure
```
user-context/
├── params.md                    # Basic user parameters
├── meds.md                      # Current medications
├── conditions.md                # Known conditions
├── healthcare-providers/        # Directory of healthcare providers
├── medical-file/
│   ├── consultations/           # Consultation summaries and records
│   ├── imaging/                 # Imaging reports and results
│   └── test-results/            # Lab work and other test results
├── visit-prep/                  # Pre-visit symptom lists
├── transcripts/                 # Raw audio transcripts before processing
└── medication-references/       # Medication translations, legality checks
```

## Key Workflows
1. **Consultation Summaries**: Convert loosely formatted transcripts of doctor visits into structured records
2. **Visit Preparation**: Format symptom lists into organized outlines for consultations
3. **Medical Report Summarization**: Generate lay-person friendly summaries of medical reports
4. **Medication Documentation**: Track medications, translations, and legality checks

## Guardrails Built In
- **Not for diagnostics**: Clear boundary on what the AI can/cannot do
- **Not a healthcare substitute**: Emphasizes professional healthcare primacy
- **Verification reminders**: Outputs include notes to verify AI-generated summaries

## Data Preservation
- Original documents always preserved
- Summaries stored alongside source documents
- Clear audit trail of what was generated from what

## Why This Works as a Claude Space
1. **Holistic Context**: Knows your conditions, medications, providers
2. **Structured Data**: Standardized format for medical records
3. **Privacy-First**: Sensitive health data stays local
4. **Workflow Optimization**: Pre-visit prep, post-visit documentation
5. **Clear Boundaries**: Built-in guardrails prevent misuse
