# Claude Code — A Personal Guide for Frode Berven

> *"The truth is out there... and so is your next paper, your next grant, and your next 5kg torsk."*

---

**Welcome, Frode.**

This repo is your personal launchpad into Claude Code — an AI-powered coding assistant that lives in your terminal. I know what you're thinking: *"Terminal? I'm a proteomics professor, not a hacker."* Relax. You don't need to know how to code. Claude does that part. You just need to know what you want — and you've never had trouble with that.

Think of Claude Code as an absurdly capable research assistant who happens to also be a software engineer, writer, data analyst, and — unlike some of your conspiracy theories — actually backed by evidence.

This guide is built specifically for you. Not generic AI tutorial nonsense. *You* — Head of Department at Biomedicine, UiB. Professor. PROBE platform leader. 80+ publications. 5,500+ citations. Mass spec wizard. And, of course, **Havfisker'n 2025 Champion** (which I'm still not over, by the way).

Let's get you dangerous.

— *Simen*

---

## Table of Contents

1. [What Is Claude Code?](#what-is-claude-code)
2. [Getting Started (10 minutes)](#getting-started)
3. [Your First Conversation](#your-first-conversation)
4. [What Can It Actually Do?](#what-can-it-actually-do)
5. [Example Walkthroughs](#example-walkthroughs)
6. [The CLAUDE.md File (Your Secret Weapon)](#the-claudemd-file)
7. [Advanced Features](#advanced-features)
8. [Tips & Tricks](#tips--tricks)
9. [Quick Reference Cheatsheet](#quick-reference-cheatsheet)

---

## What Is Claude Code?

Claude Code is an AI assistant that runs in your Mac's Terminal. Unlike ChatGPT or regular Claude on the web, Claude Code can:

- **Read and write files** on your computer
- **Run commands** in your terminal
- **Build entire applications** from a description
- **Analyze data** — CSVs, datasets, whatever you throw at it
- **Search the web** for current information
- **Work with your existing files** — papers, data, documents

It's like having a PhD student who never sleeps, never complains, knows every programming language, and — here's the important part — **doesn't have conspiratorial tendencies about the deep state controlling peer review** (looking at you, Frode).

### How Is This Different From ChatGPT?

| Feature | ChatGPT/Web Claude | Claude Code |
|---------|-------------------|-------------|
| Chat about topics | Yes | Yes |
| Read your local files | No | **Yes** |
| Write and edit files | No | **Yes** |
| Run code and scripts | Limited | **Yes, fully** |
| Build applications | No | **Yes** |
| Work with your data | Upload only | **Direct access** |
| Remember project context | Limited | **Yes (CLAUDE.md)** |

---

## Getting Started

### Step 1: Open Terminal

Press `Cmd + Space`, type **Terminal**, press Enter. That's it. No conspiracy required.

### Step 2: Install Claude Code

If it's not already installed on your Mac, run:

```bash
npm install -g @anthropic-ai/claude-code
```

> If you get an error about `npm` not being found, you'll need Node.js first:
> ```bash
> # Install Homebrew (Mac package manager)
> /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
>
> # Install Node.js
> brew install node
>
> # Then install Claude Code
> npm install -g @anthropic-ai/claude-code
> ```

### Step 3: Launch It

```bash
claude
```

That's it. You'll be asked to log in the first time. After that, you're in.

### Step 4: Clone This Repo (Your Playground)

```bash
cd ~/Desktop
git clone https://github.com/FishCompNemis/claude-code-for-frode.git
cd claude-code-for-frode
claude
```

Now Claude Code knows about your CLAUDE.md file and all the examples in this repo. It knows who you are.

---

## Your First Conversation

Once Claude Code is running, just type naturally. No special syntax. No programming knowledge needed.

**Try these:**

```
> Summarize what files are in this project and what they're for
```

```
> Read the file sample-data/proteomics-sample.csv and tell me what's interesting about it
```

```
> Write a Python script that analyzes the sample dataset and creates a visualization of the protein expression levels
```

```
> Search the web for the latest papers on single-cell proteomics from 2025-2026
```

See [examples/01-first-conversation.md](examples/01-first-conversation.md) for a complete walkthrough.

---

## What Can It Actually Do?

Here's what's relevant to **your** world:

### For Research
- Analyze proteomics datasets (CSV, TSV, Excel)
- Search PubMed and summarize recent literature
- Draft methods sections based on your experimental protocols
- Generate publication-quality figures from data
- Write and debug R or Python analysis scripts
- Review and critique manuscripts

### For Administration
- Draft faculty communications, memos, and reports
- Summarize long documents or meeting notes
- Create structured plans for department initiatives
- Analyze budgets and enrollment data
- Generate presentation content

### For Teaching
- Create exam questions from learning objectives
- Build course materials and lecture outlines
- Design assessment rubrics
- Generate interactive teaching examples

### For Building Things (Yes, You)
- Create a simple website for your research group
- Build data dashboards
- Automate repetitive tasks
- Create tools that would take a developer weeks — in minutes

> *No, Frode, the government is not monitoring what you build. Probably.*

---

## Example Walkthroughs

Each example is a self-contained exercise. Start with #1 and work your way through:

| # | Example | What You'll Learn | Time |
|---|---------|------------------|------|
| 1 | [First Conversation](examples/01-first-conversation.md) | Basic interaction, reading files, asking questions | 10 min |
| 2 | [Research Assistant](examples/02-research-assistant.md) | Literature search, paper analysis, grant writing | 15 min |
| 3 | [Data Analysis](examples/03-data-analysis.md) | Analyze a proteomics dataset, create visualizations | 15 min |
| 4 | [Writing Partner](examples/04-writing-partner.md) | Academic writing, admin emails, reports | 10 min |
| 5 | [Build Something](examples/05-build-something.md) | Create a working tool from scratch — no coding needed | 20 min |
| 6 | [Advanced Tricks](examples/06-advanced-tricks.md) | Skills, agents, MCP servers, the deep stuff | 15 min |

---

## The CLAUDE.md File

This is your secret weapon. The `CLAUDE.md` file in any project directory tells Claude Code who you are and how to work with you. **It's loaded automatically every time you start Claude Code in that directory.**

This repo already has one configured for you. Check it out:

```bash
> Read the CLAUDE.md file and tell me what it says about me
```

You can create a `CLAUDE.md` in any folder on your Mac. Working on a grant application? Create a folder, add a `CLAUDE.md` that describes the grant, and Claude becomes a grant-writing specialist.

```markdown
# Grant Application: NFR Proteomics Infrastructure

## Context
- Applying to Norwegian Research Council
- Budget: 15M NOK over 4 years
- Focus: Next-gen mass spectrometry platform for clinical proteomics
- Deadline: September 15, 2026

## Writing Style
- Clear, evidence-based, no fluff
- Follow NFR's template structure
- Emphasize translational impact
```

---

## Advanced Features

### Skills (Slash Commands)

Claude Code has built-in skills you can invoke with `/`:

- `/help` — Get help with Claude Code features
- Other skills can be installed and customized

### Agents

Claude Code can spawn sub-agents — specialized workers that handle specific tasks in parallel. Think of it as delegating to multiple research assistants at once.

```
> Search for the 10 latest papers on CSF proteomics biomarkers AND simultaneously
> analyze my dataset for differentially expressed proteins
```

### MCP Servers (Connect to External Tools)

MCP (Model Context Protocol) lets Claude Code connect to external services — databases, APIs, smart home systems, you name it. This is the deep end of the pool. See [examples/06-advanced-tricks.md](examples/06-advanced-tricks.md) when you're ready.

### Plan Mode

For complex tasks, ask Claude to plan first:

```
> I want to build a website for my research group. Let's plan it out before writing any code.
```

Claude will create a structured plan, get your approval, then execute step by step.

---

## Tips & Tricks

### The Golden Rules

1. **Be specific about what you want.** "Analyze this data" is okay. "Analyze this proteomics dataset, find the top 20 differentially expressed proteins between groups A and B, and create a volcano plot" is better.

2. **Iterate, don't restart.** If Claude gives you 80% of what you want, tell it what to change. Don't start over.

3. **Use CLAUDE.md files.** They're the difference between a generic assistant and one that knows your exact context.

4. **Ask it to explain.** If Claude writes code and you want to understand it, just ask: "Explain what this code does, in simple terms."

5. **Don't be afraid to break things.** Claude Code works on your local files. You can always undo. Nothing explodes. *(Unlike certain conspiracy theories about 5G towers.)*

### Useful Phrases

| Say this... | To get this... |
|------------|---------------|
| "Read [file] and summarize it" | Quick understanding of any document |
| "Search the web for..." | Current information, latest papers |
| "Write a script that..." | Automated data analysis |
| "Create a website that..." | A working web application |
| "Draft an email to..." | Professional communication |
| "Explain this like I'm new to coding" | Clear explanations without jargon |
| "Make it better" | Iterative improvement |
| "Actually, change the approach to..." | Course correction |

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + C` | Cancel current operation |
| `Ctrl + L` | Clear the screen |
| `Up Arrow` | Previous message |
| `Escape` | Go back / cancel |

---

## Quick Reference Cheatsheet

See [cheatsheet.md](cheatsheet.md) for a printable one-page reference.

---

## One More Thing

Claude Code is a tool. A powerful one. But it's only as useful as the questions you ask it. The good news? You've spent your entire career asking good questions — about proteins, about disease mechanisms, about why that one fish got away.

The even better news? Unlike peer reviewers, Claude doesn't have an ego. Unlike grant committees, it responds in seconds. And unlike your fishing buddies, it won't question your conspiracy theories to your face.

Now go build something amazing. Or at least analyze that dataset you've been putting off.

**Tight lines and good commits,**
Simen

---

*P.S. — If Claude ever tells you something that sounds like a conspiracy theory, it's probably hallucinating. If YOU tell Claude something that sounds like a conspiracy theory... well, that's just Tuesday.*

*P.P.S. — Yes, I built this entire repo using Claude Code. The irony is not lost on me.*
