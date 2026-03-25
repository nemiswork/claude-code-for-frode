# Example 6: Advanced Tricks

> Time: ~15 minutes
> Goal: Learn the power features — skills, agents, plan mode, and MCP

## Plan Mode: Think Before Building

For complex projects, you want Claude to plan before it acts.

```
/plan I want to create a Python package that automates our standard
proteomics analysis pipeline — from MaxQuant output to publication figures.
Let's think through the architecture before writing any code.
```

Claude will:
1. Analyze the requirements
2. Propose an architecture with multiple approaches
3. Get your approval
4. Then execute step by step

This is how you build real, structured projects — not just one-off scripts.

## Agents: Parallel Workers

Claude can spawn sub-agents to work on multiple things simultaneously. This happens automatically when useful, but you can also request it:

```
I need you to do three things:
1. Search for recent papers on SMOC1 as an Alzheimer's biomarker
2. Analyze my sample dataset for SMOC1 expression
3. Draft an introduction paragraph about SMOC1's role in AD

Do all three in parallel.
```

Instead of doing these sequentially, Claude dispatches specialized agents that work simultaneously and combine results.

## Skills: Specialized Workflows

Skills are pre-built workflows that activate with `/` commands. Some useful ones:

```
/help          — Get help with Claude Code features
```

Skills can be installed and customized. Think of them as "expert modes" that Claude can switch into for specific types of work.

## CLAUDE.md Stacking

You can have multiple `CLAUDE.md` files at different levels:

```
~/.claude/CLAUDE.md              ← Global (applies everywhere)
~/Desktop/my-project/CLAUDE.md   ← Project-specific
~/Desktop/my-project/src/CLAUDE.md  ← Sub-directory specific
```

They stack. So you can have global preferences (language, style) plus project-specific context.

### Example: Global CLAUDE.md

Create `~/.claude/CLAUDE.md`:

```markdown
# Frode Berven — Global Preferences

## Who I Am
- Head of Department, Biomedicine, UiB
- Proteomics researcher
- New to coding — explain code clearly

## Preferences
- Python for data analysis
- R if specifically needed for Bioconductor packages
- Clean, commented code
- Prefer simple solutions over clever ones
```

This applies to **every** Claude Code session, regardless of directory.

## MCP: Connect to External Tools

MCP (Model Context Protocol) is how Claude Code connects to external services. It's like giving Claude superpowers by connecting it to databases, APIs, and tools.

**Examples of what MCP can connect to:**
- Databases (query your research database directly)
- Slack (read and send messages)
- GitHub (manage repositories, issues, PRs)
- Home automation systems
- Custom APIs

Setting up MCP is more advanced and requires some configuration. When you're ready, ask Claude:

```
How do I set up an MCP server to connect to a PostgreSQL database?
```

## Git Integration

Claude Code is deeply integrated with Git (the version control system used by developers). Even as a non-coder, this is valuable:

```
Show me what files have changed since I started this session
```

```
Create a git commit with all my changes and a descriptive message
```

```
Show me the history of changes to this file
```

Git means you can always go back. Every change is tracked. Nothing is permanently lost (unlike that 8kg torsk that got away from you on Havfiskern, Frode).

## Keyboard Efficiency

Once you're comfortable, these speed you up:

| Action | How |
|--------|-----|
| Submit a message | Enter (or Cmd+Enter for multi-line) |
| Cancel | Ctrl+C or Escape |
| Multi-line input | Shift+Enter for new line, then Enter to send |
| Clear screen | Ctrl+L |
| Exit | Type "exit" or Ctrl+D |

## The Meta-Move: Use Claude to Learn Claude

The most powerful thing you can do:

```
What are the most powerful features of Claude Code that I'm probably not using?
Give me specific examples relevant to an academic researcher.
```

Claude will teach you about itself. It knows its own capabilities better than any guide (even this one).

## What You Now Know

You've gone from "what is a terminal" to understanding:
- Basic interaction and file operations
- Research assistance and literature search
- Data analysis and visualization
- Academic and administrative writing
- Building working applications from scratch
- Advanced features: plans, agents, skills, MCP, Git

You're ready. Go build something that matters.

> *And remember: if anything seems too good to be true... it's probably not a conspiracy. It's just good engineering.*
>
> *But feel free to investigate. That's what scientists do.*

---

*Guide created with care (and Claude Code) by Simen Vikdal — your fishing rival, tech enabler, and friend who definitely didn't rig the Havfisker'n scoring system, no matter what you think.*
