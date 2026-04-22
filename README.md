# Create Effective Skills

Two production-ready AI skills for building skills that actually work — not just prompt-guessing.

## Quick Start (For AI Agents)

If an AI agent is reading this repo, here's what to do:

```bash
# === OpenCode ===
cp -r signal-skill-framework ~/Library/Application\ Support/opencode/skills/
cp -r skill-creator ~/Library/Application\ Support/opencode/skills/

# OR === Claude Code (.claude/) ===
cp -r signal-skill-framework ~/.claude/skills/
cp -r skill-creator ~/.claude/skills/

# OR === Agents (.agents/) ===
cp -r signal-skill-framework ~/.agents/skills/
cp -r skill-creator ~/.agents/skills/
```

Then use:
- `/signal-skill-framework` — Plan what to build
- `/skill-creator` — Build and test it

---

## What's Included

### 1. Signal Skill Framework (`signal-skill-framework/`)

Strategic thinking partner using the SIGNAL methodology:

| Phase | Meaning |
|------|---------|
| **S**pot | Identify soul-sucking repetitive tasks |
| **I**ntegrate | Select minimal tools needed |
| **G**uide | Train the AI step-by-step |
| **N**ail | Achieve gold-standard runs |
| **A**utomate | Codeify the skill |
| **L**oop | Test → Fail → Fix → Repeat |

**Triggers:** `/signal-skill-framework`, "create a skill", "build an automation"

### 2. Skill Creator (`skill-creator/`)

Execution layer for building and testing skills:

- Write/edit SKILL.md files
- Run test cases and benchmarks  
- Create evaluation viewers
- Package skills for distribution

**Triggers:** `/skill-creator`, "build this skill", "create skill from"

---

## Installation by System

| System | Skills Folder | Command |
|--------|------------|---------|
| **OpenCode** | `~/.opencode/skills/` | `cp -r * ~/Library/Application\ Support/opencode/skills/` |
| **Claude Code** | `.claude/skills/` | `cp -r * ~/.claude/skills/` |
| **Agents** | `.agents/skills/` | `cp -r * ~/.agents/skills/` |

### By OS

```bash
# === macOS ===
# OpenCode
cp -r signal-skill-framework ~/Library/Application\ Support/opencode/skills/
cp -r skill-creator ~/Library/Application\ Support/opencode/skills/
# Claude Code
cp -r signal-skill-framework ~/.claude/skills/
cp -r skill-creator ~/.claude/skills/
# Agents
cp -r signal-skill-framework ~/.agents/skills/
cp -r skill-creator ~/.agents/skills/

# === Linux ===
# OpenCode
cp -r signal-skill-framework ~/.local/share/opencode/skills/
cp -r skill-creator ~/.local/share/opencode/skills/
# Claude Code
cp -r signal-skill-framework ~/.claude/skills/
cp -r skill-creator ~/.claude/skills/
# Agents
cp -r signal-skill-framework ~/.agents/skills/
cp -r skill-creator ~/.agents/skills/

# === Windows (PowerShell) ===
# OpenCode
Copy-Item -Recurse signal-skill-framework "$env:APPDATA\opencode\skills\"
Copy-Item -Recurse skill-creator "$env:APPDATA\opencode\skills\"
# Claude Code
Copy-Item -Recurse signal-skill-framework "$env:USERPROFILE\.claude\skills\"
Copy-Item -Recurse skill-creator "$env:USERPROFILE\.claude\skills\"
# Agents
Copy-Item -Recurse signal-skill-framework "$env:USERPROFILE\.agents\skills\"
Copy-Item -Recurse skill-creator "$env:USERPROFILE\.agents\skills\"
```

Then restart your AI tool.

---

## The Workflow

```
[Have a repetitive task] → /signal-skill-framework → /skill-creator → test → iterate → package
```

| Step | Skill | What it does |
|------|-------|-------------|
| 1 | Signal Framework | Clarify what to build and why |
| 2 | Skill Creator | Execute, write SKILL.md, test |
| 3 | Iterate | Improve based on feedback |
| 4 | Package | Export as distributable |

---

## Skill Anatomy (For Reference)

```
skill-name/
├── SKILL.md              # Required - triggers and instructions
├── prompts/              # Optional - additional prompt files  
├── scripts/              # Optional - executable code
├── references/          # Optional - documentation
└── assets/              # Optional - templates, icons
```

### SKILL.md Required Fields

```markdown
# Skill Name

**Trigger phrases:** /skill-name, "when I say X"

**Description:** What this skill does (1-2 sentences)

## When to use
- Situation 1
- Situation 2

## How it works
Step-by-step instructions...

## Example prompts
- "Do X"
- "Do Y"
```

---

## Requirements

- Any AI tool with skills support (OpenCode, Claude Code, Agents, etc.)
- Python 3.x (for evaluation scripts)
- Subagents enabled (optional, for parallel tests)

---

## Support

- **signal-skill-framework** → strategic planning ("what to build")
- **skill-creator** → execution ("how to build it")

Both work together. Start with Signal Framework, then hand off to Skill Creator.

---

## License

Apache 2.0 — See LICENSE file

---

## Repo Structure

```
create-effective-skills/
├── README.md                    # This file
├── LICENSE                     # Apache 2.0
├── INSTALL_PROMPT.md           # Copy-paste install instructions for AI agents
├── signal-skill-framework/    # Skill 1: Strategic planning
│   ├── SKILL.md
│   └── prompts/
│       └── signal_skill_architect.md
└── skill-creator/             # Skill 2: Execution & testing
    ├── SKILL.md
    ├── scripts/              # Python evaluation scripts
    ├── agents/               # Grader, comparator, analyzer prompts
    ├── eval-viewer/          # HTML evaluation viewer
    ├── references/          # Schemas and documentation
    └── assets/              # Templates
```