# Claude Decision Evaluation Framework

**Repository**: [Claude-Decision-Evaluation-Framework](https://github.com/danielrosehill/Claude-Decision-Evaluation-Framework)

## Purpose
Structured system for analyzing major decisions through seven parallel analytical frameworks. Provides multiple perspectives on any significant decision without making the decision for you.

## Core Structure
```
.
├── decisions/
│   ├── queue/           # Decisions awaiting analysis
│   └── processed/       # Decisions that have been analyzed
├── frameworks/          # Framework definition files
│   ├── cost-benefit-analysis.md
│   ├── swot-analysis.md
│   ├── decision-matrix.md
│   ├── ice-framework.md
│   ├── risk-reward-assessment.md
│   ├── eisenhower-matrix.md
│   └── regret-minimization.md
└── outputs/             # Analysis reports
```

## The Seven Frameworks
1. **Cost-Benefit Analysis**: Economic and practical viability
2. **SWOT Analysis**: Strengths, Weaknesses, Opportunities, Threats
3. **Decision Matrix**: Multi-criteria weighted evaluation
4. **ICE Framework**: Impact, Confidence, Ease scoring
5. **Risk-Reward Assessment**: Potential gains vs potential losses
6. **Eisenhower Matrix**: Importance and urgency prioritization
7. **Regret Minimization**: Long-term regret projection

## How It Works
1. User places decision file in `/decisions/queue/`
2. Run `/analyze-decision`
3. Seven parallel subagents analyze using their respective frameworks
4. Each produces independent analysis and 0-100 score
5. Results aggregated into comprehensive report
6. User reviews multiple perspectives to inform their decision

## Key Principles
- **Parallel Analysis**: All frameworks run simultaneously
- **Independence**: Frameworks don't influence each other
- **No Composite Scores**: Individual scores preserved
- **Guidance, Not Answers**: The final decision remains human

## Why This Works as a Claude Space
1. **Multi-Agent Orchestration**: Demonstrates parallel subagent pattern
2. **Framework Preservation**: Methodologies stored and versioned
3. **Decision Archive**: Track decisions and analyses over time
4. **Reproducibility**: Same decision can be re-analyzed with same frameworks
5. **Objectivity**: Multiple lenses reveal different aspects
