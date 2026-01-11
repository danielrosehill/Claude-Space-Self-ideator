# Claude Budget Workspace Template

**Repository**: [Claude-Budget-Workspace-Template](https://github.com/danielrosehill/Claude-Budget-Workspace-Template)

## Purpose
Comprehensive household budget management using Claude Code CLI. Provides a structured environment for tracking income, expenses, savings goals, and financial health with AI-assisted analysis and reporting.

## Core Structure
```
.
├── .claude/
│   ├── agents/              # Specialized budget management agents
│   └── commands/            # Slash commands for budget operations
├── context/
│   ├── household/          # Household-specific context
│   ├── financial/          # Financial account details
│   └── goals/              # Financial goals documentation
├── prompts/                # Reusable prompts for budget tasks
├── outputs/
│   ├── budgets/           # Generated budget documents
│   ├── reports/           # Financial reports and analyses
│   └── visualizations/    # Charts and graphs
├── transactions/
│   ├── import/            # Raw transaction data for import
│   └── processed/         # Processed and categorized transactions
├── budgets/
│   ├── templates/         # Budget templates
│   └── monthly/           # Monthly budgets
├── financial-goals/
│   ├── active/            # Active financial goals
│   └── archived/          # Completed goals
└── context.md             # Main household context configuration
```

## Key Agents
- **budget-architect**: Creates comprehensive budgets based on income, history, and goals
- **expense-analyst**: Identifies spending patterns and optimization opportunities
- **goal-tracker**: Monitors progress toward financial goals
- **transaction-processor**: Imports and categorizes transaction data
- **financial-advisor**: Provides strategic guidance and scenario planning

## Representative Slash Commands
- `/create-monthly-budget` - Generate budget for upcoming month
- `/monthly-report` - Comprehensive monthly financial report
- `/analyze-spending` - Category breakdowns and patterns
- `/set-financial-goal` - Define new financial objectives
- `/debt-payoff-plan` - Strategic debt reduction planning

## Why This Works as a Claude Space
1. **Persistent Context**: Financial data, accounts, and goals remain accessible
2. **Version Control**: Track budget changes and financial decisions over time
3. **Privacy**: All sensitive data stays local
4. **Structured Workflows**: Clear paths for common financial tasks
5. **Agent Specialization**: Different agents for different financial concerns
