# Claude Space Development Pattern

This document describes the standard pattern for building a Claude Space. Following this formula ensures consistent, reliable functionality across different domains.

## The Six-Step Formula

### Step 1: CLAUDE.md as Foundation

The `CLAUDE.md` file serves as the foundational system prompt. It defines:
- The purpose and scope of the workspace
- Behavioral guidelines and guardrails
- The complete folder structure (critically important)
- Available agents and their roles
- Available slash commands and their purposes

**Key principle**: Everything the agent needs to know about operating in this space should be in or referenced from `CLAUDE.md`.

### Step 2: Initiation Command

Create an onboarding/initiation command that:
- Welcomes the user to the space
- Collects user-specific context
- Customizes the workspace to their needs
- Populates initial context files

Example: `/onboard`, `/setup`, `/initialize`

This command transforms a generic template into a personalized workspace.

### Step 3: Input/Output Segregation

Create top-level folders to clearly separate human and AI content:

```
├── inputs/          # Human-provided content
│   ├── raw/         # Unprocessed inputs
│   └── data/        # Structured data
└── outputs/         # AI-generated content
    ├── drafts/      # Work in progress
    └── final/       # Completed outputs
```

This segregation:
- Makes clear what's source material vs generated
- Enables version control of both streams
- Simplifies backup and export workflows

### Step 4: Command and Agent Libraries

Create organized libraries:

```
.claude/
├── commands/        # Slash commands
│   ├── onboard.md
│   ├── analyze.md
│   └── report.md
└── agents/          # Sub-agent definitions
    ├── analyst.md
    ├── writer.md
    └── reviewer.md
```

Each command/agent should have:
- Clear, single purpose
- Defined inputs and outputs
- Reference back to CLAUDE.md for context

### Step 5: Folder Structure Definition in CLAUDE.md

**This is critical for reliable operation.**

CLAUDE.md must contain an explicit folder structure definition that:
- Lists every folder and its purpose
- Specifies where different content types belong
- Defines naming conventions for files
- Establishes the expected workflow through folders

Example:
```markdown
## Folder Structure

- `/inputs/raw/` - Drop raw materials here for processing
- `/inputs/data/` - Structured data files (CSV, JSON)
- `/context/` - Background information that persists
- `/outputs/drafts/` - Work in progress, may be incomplete
- `/outputs/final/` - Completed, reviewed outputs only
- `/archive/` - Processed inputs and superseded outputs
```

Without this explicit definition, the agent may create inconsistent folder usage.

### Step 6: Sub-Agent Coordination

When using multiple agents:
1. Each agent receives the same CLAUDE.md reference
2. Agents should be invoked in parallel where possible
3. Outputs from agents should land in designated folders
4. Main Claude coordinates and synthesizes agent outputs

Example workflow:
```
User runs /analyze-report

Main Claude:
1. Reads CLAUDE.md for context
2. Launches analyst agent (reads CLAUDE.md, analyzes data)
3. Launches summarizer agent (reads CLAUDE.md, creates summary)
4. Waits for both to complete
5. Synthesizes outputs into /outputs/final/
```

## Pattern Summary

```
┌─────────────────────────────────────────────────────────────┐
│                       CLAUDE.md                              │
│  (System prompt, folder structure, agent/command registry)   │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                    /onboard command                          │
│         (Customize workspace to user's context)              │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌──────────────────────┐     ┌──────────────────────┐
│      /inputs/        │     │      /outputs/       │
│  (Human materials)   │ ──▶ │   (AI generations)   │
└──────────────────────┘     └──────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                 .claude/commands/ + agents/                  │
│            (Specialized workflows and agents)                │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│               Parallel sub-agent execution                   │
│        (All agents reference CLAUDE.md for guidance)         │
└─────────────────────────────────────────────────────────────┘
```

## Why This Pattern Works

1. **Single source of truth**: CLAUDE.md contains all operating context
2. **Clear boundaries**: Input/output separation prevents confusion
3. **Customization**: Onboarding makes generic templates personal
4. **Scalability**: Agent pattern enables complex workflows
5. **Reliability**: Explicit folder definitions prevent drift
6. **Portability**: Pattern transfers across domains

## Common Pitfalls

- **Vague folder descriptions**: Be specific about what goes where
- **Missing CLAUDE.md reference in agents**: Agents lose context
- **No onboarding**: Users can't customize the space
- **Mixed input/output folders**: Creates confusion about provenance
- **Sequential agents when parallel is possible**: Slower than necessary
