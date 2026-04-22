# Create Effective Skills

Two powerful skills to help you create production-ready AI skills that actually work.

## What's Included

### 1. Signal Skill Framework (`signal-skill-framework/`)

A strategic thinking partner that guides you through the SIGNAL methodology:

| Phase | Action | Purpose |
|-------|-------|---------|
| **S** | Spot the Bottleneck | Identify soul-sucking repetitive tasks |
| **I** | Integrate the Stack | Select minimal tools needed |
| **G** | Guide the Agent | Train the AI step-by-step |
| **N** | Nail the Standard | Achieve gold-standard runs |
| **A** | Automate the Logic | Codeify the skill |
| **L** | Loop Recursively | Test → Fail → Fix → Repeat |

**Use when:** You want to create a new skill or automate a workflow. It's your thought partner to move from "prompt-guessing" to "skill-architecting."

### 2. Skill Creator (`skill-creator/`)

The execution layer for building and testing skills:

- Write and edit SKILL.md files
- Run test cases and benchmarks
- Create evaluation viewers
- Optimize skill descriptions for better triggering
- Package skills for distribution

**Use when:** You're ready to build, test, and refine your skill.

---

## Installation

### Option A: Copy to OpenCode Skills Directory

1. Locate your OpenCode skills directory (typically `~/.opencode/skills/` or `~/Library/Application Support/opencode/skills/`)
2. Copy both folders into your skills directory:
   ```bash
   cp -r signal-skill-framework ~/Library/Application\ Support/opencode/skills/
   cp -r skill-creator ~/Library/Application\ Support/opencode/skills/
   ```
3. Restart OpenCode to load the new skills

### Option B: Reference Without Installing

You can reference these skills by their full path without copying:
- `signal-skill-framework`: `/path/to/create-effective-skills/signal-skill-framework`
- `skill-creator`: `/path/to/create-effective-skills/skill-creator`

---

## How to Use

### Step 1: Plan with Signal Framework

Start a conversation and invoke the signal skill:
```
/signal-skill-framework
```

The skill will walk you through each SIGNAL phase to clarify what you want to build and why.

### Step 2: Build with Skill Creator

When you're ready to execute, hand off to:
```
/skill-creator
```

This skill handles:
1. **Capturing intent** - What should the skill do? When should it trigger?
2. **Writing the SKILL.md** - Draft the skill file with proper structure
3. **Creating test cases** - Design realistic prompts to test against
4. **Running evaluations** - Execute tests with and without the skill
5. **Benchmarking** - Compare results quantitatively
6. **Iterating** - Improve based on feedback
7. **Packaging** - Export as a distributable skill file

### The Workflow

```
signal-skill-framework (plan) → skill-creator (build) → test → iterate → package
```

### What You Can Create

- **File transformation skills** - Convert between formats, extract data, batch process
- **Research skills** - Search, summarize, analyze content
- ** workflow automation** - Multi-step processes with APIs and tools
- **Code generation skills** - Scaffold projects, write tests, refactor
- **Documentation skills** - Generate docs from code, format output

---

## Skill Anatomy

Both skills follow the OpenCode skill structure:

```
skill-name/
├── SKILL.md           # Required - triggers and instructions
├── prompts/          # Optional - additional prompt files
├── scripts/         # Optional - executable code
├── references/      # Optional - documentation
└── assets/         # Optional - templates, icons
```

---

## Tips for Success

1. **Start small** - Don't try to automate everything at once
2. **Test relentlessly** - Run 5+ iterations before calling it done
3. **Use real prompts** - Test with prompts users would actually type
4. **Iterate on feedback** - Every failure teaches you something
5. **Generalize** - Build for a million use cases, not just your current one

---

## Requirements

- OpenCode (CLI or Code)
- Python 3.x (for benchmarking scripts in skill-creator)
- Subagents enabled (for parallel test execution)

---

## Support

These skills work together as a strategic + execution combo:
- Use **signal-skill-framework** first to plan
- Then **skill-creator** to build and test

The Signal Framework tells you *what* to build; Skill Creator shows you *how* to build it.