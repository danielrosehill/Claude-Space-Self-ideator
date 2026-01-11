# Agent Portability

## The Pattern Is Agent-Agnostic

While this repository uses "Claude Spaces" as the terminology—reflecting the origin of this pattern with Claude Code CLI—the underlying architecture is not Claude-specific. The same structural patterns work with any agentic CLI or AI coding assistant.

## Core Principles That Transfer

The fundamental elements that make a Claude Space work are platform-independent:

| Element | Claude Code | Other Agents |
|---------|-------------|--------------|
| System Prompt | `CLAUDE.md` | Agent-specific config file (e.g., `AGENTS.md`, `.agent/config.md`) |
| Slash Commands | `.claude/commands/` | Equivalent command directory |
| Sub-agents | `.claude/agents/` | Equivalent agent definitions |
| Context Folder | `context/` | Universal - just folders |
| Input/Output Folders | `inputs/`, `outputs/` | Universal - just folders |
| Version Control | Git | Universal |

The magic is in the **folder structure and workflow patterns**, not the specific agent runtime.

## Compatible Agent Platforms

### Currently Compatible

These agentic CLIs can use the same workspace patterns:

- **Claude Code CLI** (Anthropic) - The origin of this pattern
- **Codex CLI** (OpenAI) - Uses similar repository-based context
- **Aider** - AI pair programming with repository awareness
- **Cursor** - IDE-integrated agent with folder awareness
- **Continue** - Open-source AI coding assistant
- **Cody** (Sourcegraph) - Repository-aware AI assistant

### Adaptation Requirements

When porting a Claude Space to another agent:

1. **Rename the system prompt file** to match the agent's convention
2. **Adjust command syntax** if the agent uses different slash command patterns
3. **Verify agent/sub-agent support** - not all agents support multi-agent orchestration
4. **Check tool availability** - some agents have different tool capabilities

## Using Claude to Bootstrap New Spaces

One powerful workflow is using Claude as a **space architect** to design workspaces for any agent:

### The Bootstrap Pattern

1. **Describe the domain** to Claude (e.g., "I want a workspace for tracking my garden")
2. **Claude generates the folder structure** based on the patterns in this repository
3. **Claude creates the system prompt** tailored to the domain
4. **Claude suggests commands and agents** appropriate to the workflows
5. **You adapt the output** for your preferred agent runtime

### Why Claude Excels at This

- Understands the meta-pattern of what makes workspaces effective
- Can reason about domain-specific needs and translate them to folder structures
- Has seen enough examples to suggest appropriate agents and commands
- Can iterate on designs based on feedback

### Example Prompt

```
Based on the Claude Space pattern, design a workspace for [DOMAIN].

Consider:
- What context needs to persist between sessions?
- What are the common workflows?
- What inputs will the user provide?
- What outputs should be generated?
- What specialized agents would be helpful?
- What slash commands would streamline common tasks?

Generate:
1. A folder structure diagram
2. A system prompt (CLAUDE.md or equivalent)
3. 3-5 key slash command definitions
4. 1-2 specialized agent definitions
```

## Portability Layers

### Layer 1: Pure Structure (100% Portable)
- Folder organization (`context/`, `inputs/`, `outputs/`)
- File naming conventions
- Markdown documentation patterns
- Git version control

### Layer 2: System Prompts (Easy Adaptation)
- Core instructions transfer directly
- Agent-specific features need adjustment
- Guardrails and behavior guidelines are universal

### Layer 3: Commands and Agents (Moderate Effort)
- Command concepts transfer; syntax may differ
- Multi-agent orchestration varies by platform
- Some agents don't support sub-agents at all

### Layer 4: Integrations (Platform-Specific)
- MCP servers (Claude-specific currently)
- IDE integrations
- External tool connections

## Future Considerations

As the agentic coding assistant landscape evolves:

1. **Standardization may emerge** - Common patterns for agent configuration
2. **Interoperability tools** - Converters between agent formats
3. **Universal workspace specs** - Shared standards for AI workspaces

For now, design for the structure layer first, and treat agent-specific features as adaptable overlays.

## Practical Recommendation

When creating a new space:

1. **Start with Claude Code** - It has the most mature workspace patterns
2. **Focus on folder structure** - This is the most portable element
3. **Document your workflows in markdown** - Universal and readable
4. **Keep agent-specific features modular** - Easy to swap out
5. **Version control everything** - Git works everywhere

The goal is to build cognitive infrastructure that outlasts any particular AI platform.
