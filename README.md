[![Claude Code Repos](https://img.shields.io/badge/Claude%20Code-Repos%20Index-blue?style=flat-square&logo=github)](https://github.com/danielrosehill/Claude-Code-Repos-Index)

# Claude Space Self-Ideator

An ideation workspace for generating new Claude Space concepts - using a Claude Space to brainstorm Claude Spaces.

## What's a Claude Space?

A **Claude Space** is a version-controlled repository that functions as a miniaturized agentic workspace. It uses folder structure, system prompts (`CLAUDE.md`), slash commands, and sub-agents to create a focused environment for human-AI collaboration on specific domains or problems.

The core insight: a code repository's folder structure can serve as a simple, transparent, and portable way to manage AI context - no databases, embeddings, or complex infrastructure required.

### Why This Pattern Works

See [the-idea.md](the-idea.md) for a detailed explanation from the author on why this approach is uniquely powerful:

- **Miniaturized agentic systems**: A repository provides approximate boundaries for agents and humans to work within, achieving what otherwise requires complicated infrastructure
- **Lightweight RAG**: Using Markdown files as context provides a simple alternative to formal vectorization or retrieval-augmented generation at the prototype level
- **Template-driven iteration**: GitHub's template structure allows significant upfront investment in workflow design that can be reused as suitable projects arise
- **Domain-agnostic**: The pattern works equally for systems administration, code generation, technical writing, or entirely non-coding projects
- **Version-controlled workflows**: Git's history provides an instructive model for workflow management with applications far beyond software development

## Repository Contents

### `/ideas/` - New Claude Space Concepts

Organized by category, each idea follows a consistent template:

| Category | Ideas |
|----------|-------|
| `personal-development/` | Habit Laboratory, Life Audit, Values Compass |
| `learning-skills/` | Learning Lab, Skill Tracker |
| `relationships-social/` | Relationship Nurture, Difficult Conversations |
| `creativity-projects/` | Idea Incubator, Creative Project Manager |
| `home-life-management/` | Home Operations, Meal Intelligence |
| `professional-career/` | Career Architect, Meeting Maximizer |
| `mental-emotional-wellbeing/` | Anxiety Workbench, Gratitude Practice |
| `specialized-domains/` | Travel Planner, Garden Intelligence, Pet Care, Emergency Preparedness |

### `/examples/` - Existing Claude Spaces

Summaries of working Claude Spaces with links to their repositories:

- Budget Workspace Template
- Debugging Workspace
- Health Helper
- Decision Evaluation Framework
- Deep Research Template

### `/docs/` - Pattern Documentation

- **claude-perspective.md** - Claude's own analysis of what makes the pattern work
- **agent-portability.md** - Using these patterns with other agentic CLIs (Codex, Aider, etc.)
- **development-pattern.md** - The six-step formula for building Claude Spaces

## Using This Repository

Run `/develop-idea` with your concept, and this workspace will generate a structured idea document following the standard template - including suggested folder structure, workflows, commands, and agents.

## The Claude Space Pattern (Summary)

1. `CLAUDE.md` as foundational system prompt
2. Initiation command for user customization
3. `inputs/` and `outputs/` folders to segregate human and AI content
4. Slash command and agent libraries in `.claude/`
5. Explicit folder structure definition in `CLAUDE.md`
6. Sub-agents reference the same guidance document for consistency

---

*For more Claude Code projects, visit my [Claude Code Repos Index](https://github.com/danielrosehill/Claude-Code-Repos-Index).*
