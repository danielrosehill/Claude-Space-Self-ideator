# Claude Debugging Workspace

**Repository**: [Claude-Debugging-Workspace](https://github.com/danielrosehill/Claude-Debugging-Workspace)

## Purpose
A workspace for systematic debugging of persistent problems - technical, process-related, personal, or creative. The methodology applies to any problem that benefits from forming hypotheses, testing them, excluding causes, and documenting progress.

## Core Structure
```
.
├── inputs/
│   ├── logs/              # System logs, error logs, application logs
│   ├── screenshots/       # Visual evidence of the problem
│   ├── recordings/        # Screen recordings or audio context
│   └── data/              # Text data, configuration files
├── outputs/
│   ├── analysis/          # Analysis documents and findings
│   ├── attempts/          # Documentation of remediation attempts
│   └── resolution/        # Final documentation when resolved
├── context/               # Summary and background information
└── debug-log/             # Chronological debugging efforts
```

## Types of "Bugs" This Addresses
- **Technical**: Software errors, system failures, configuration issues
- **Process**: Workflow inefficiencies, recurring bottlenecks
- **Life/Personal**: Persistent problems requiring systematic investigation
- **Creative**: Stuck projects, recurring blockers

## Key Commands
- `/onboarding` - Start a new debugging session
- `/status` - Get current status of debugging effort
- `/hypotheses` - Review current hypotheses and their status
- `/summarize` - Generate a summary of progress to date

## Debugging Protocol
1. Maintain chronological log of debugging efforts
2. Document suspected causes as hypotheses to be tested
3. Mark excluded causes as debugging progresses
4. Always include dates to show chronological sequence
5. Create summaries for future reference

## Why This Works as a Claude Space
1. **Persistence**: Complex bugs span sessions - context survives
2. **Documentation**: Automatically tracks what was tried and excluded
3. **Methodology**: Forces systematic approach rather than random attempts
4. **Evidence Gathering**: Dedicated folders for logs, screenshots, data
5. **Generalizability**: The pattern works for any persistent problem
