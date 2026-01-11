# Claude Deep Research Template

**Repository**: [Claude-Deep-Research-Template](https://github.com/danielrosehill/Claude-Deep-Research-Template)

## Purpose
Structured approach to conducting comprehensive research using Claude Code. Supports iterative, deep research with context gathering, prompt planning, systematic execution, and synthesized output generation.

## Core Structure
```
├── context/              # Research context and source materials
│   ├── from-internet/   # Web research, papers, articles
│   ├── from-human/      # User-provided context and requirements
│   └── from-history/    # Previous conversation histories
├── prompts/             # Research prompts by stage
│   ├── drafting/        # Draft prompts
│   ├── queue/           # Prompts ready to execute
│   └── run/             # Executed prompts
│       ├── initial/     # Starting prompts
│       └── subsequent/  # Follow-up prompts
├── outputs/             # Research outputs
│   ├── individual/      # Single-topic outputs
│   ├── aggregated/      # Synthesized outputs
│   │   ├── pdf/        # PDF reports
│   │   └── mk-combined/# Combined markdown
│   └── reformatted/     # Alternative formats (TTS, SSML)
├── pipeline/            # Workflow automation
│   └── audio-dropoff/  # Audio processing queue
├── notes/              # Research notes and documentation
└── scratchpad/         # Working area for experiments
```

## Research Workflow
1. **Context Gathering**: Review materials in context directories
2. **Prompt Planning**: Draft and organize research prompts
3. **Research Execution**: Run initial prompts, generate follow-ups
4. **Output Generation**: Save individual findings, create aggregated reports
5. **Documentation**: Maintain research notes and methodology

## Output Formats
- Individual research findings
- Aggregated comprehensive reports
- PDF versions for sharing
- TTS-safe text for audio conversion
- SSML for voice synthesis

## Why This Works as a Claude Space
1. **Iterative Research**: Supports multi-session deep dives
2. **Context Preservation**: Sources, history, and findings persist
3. **Prompt Versioning**: Track how research questions evolve
4. **Multiple Outputs**: Same research → multiple formats
5. **Pipeline Integration**: Supports audio input workflows
