# AI Agent Prompt: Install Skills

Copy and paste this entire block into your AI conversation:

---

**SYSTEM PROMPT:**

I have a skill package called "Create Effective Skills" at this path:

`/Users/youtube/Documents/GitHub/public/create-effective-skills`

It contains two skills:
- `signal-skill-framework/` — Strategic planning
- `skill-creator/` — Build and test execution

Please install both into my skills folder.

**Steps to run:**

```bash
# Find skills directory and copy both skills
SKILLS_PATH="/path/to/your/skills/folder"

# OpenCode
mkdir -p ~/Library/Application\ Support/opencode/skills/
cp -r /Users/youtube/Documents/GitHub/public/create-effective-skills/signal-skill-framework ~/Library/Application\ Support/opencode/skills/
cp -r /Users/youtube/Documents/GitHub/public/create-effective-skills/skill-creator ~/Library/Application\ Support/opencode/skills/

# Verify
ls ~/Library/Application\ Support/opencode/skills/
```

---

## Installation by System

| System | Skills Folder | How to Copy |
|--------|------------|------------|
| **OpenCode** | `~/.opencode/skills/` or `~/Library/Application Support/opencode/skills/` | `cp -r skill ~/.opencode/skills/` |
| **Claude Code** | `.claude/skills/` in your project or home | `cp -r skill ~/.claude/skills/` |
| **Agents** | `.agents/skills/` in your project or home | `cp -r skill ~/.agents/skills/` |
| **OpenAI Agents** | `agents/` in repo root | `cp -r skill ./agents/` |

### Quick Commands by System

```bash
# === OpenCode (macOS) ===
cp -r signal-skill-framework ~/Library/Application\ Support/opencode/skills/
cp -r skill-creator ~/Library/Application\ Support/opencode/skills/

# === OpenCode (Linux) ===
cp -r signal-skill-framework ~/.local/share/opencode/skills/
cp -r skill-creator ~/.local/share/opencode/skills/

# === OpenCode (Windows) ===
xcopy signal-skill-framework %APPDATA%\opencode\skills\
xcopy skill-creator %APPDATA%\opencode\skills\

# === Claude Code (.claude/skills/) ===
cp -r signal-skill-framework ~/.claude/skills/
cp -r skill-creator ~/.claude/skills/

# === Agents (.agents/skills/) ===
cp -r signal-skill-framework ~/.agents/skills/
cp -r skill-creator ~/.agents/skills/

# === Project-specific (in repo root) ===
mkdir -p skills
cp -r signal-skill-framework skills/
cp -r skill-creator skills/
```

---

## After Installation

**Restart your AI tool, then use:**

| System | Trigger Command |
|--------|---------------|
| OpenCode | `/signal-skill-framework` then `/skill-creator` |
| Claude Code | Import skill then invoke by name |
| Agents | `@skill-name` or direct invoke |

---

## What These Skills Do

| Skill | Trigger | Purpose |
|-------|---------|---------|
| **signal-skill-framework** | `/signal-skill-framework` | Think through WHAT to build before building |
| **skill-creator** | `/skill-creator` | Build, test, and package the skill |

Use them together: Plan first with Signal Framework, then build with Skill Creator.

---

## Directory Structure

The skills follow standard structure:

```
signal-skill-framework/
├── SKILL.md              # Triggers and instructions
└── prompts/             # Additional prompts

skill-creator/
├── SKILL.md              # Triggers and instructions
├── scripts/             # Python evaluation scripts
├── agents/              # Grader prompts
├── eval-viewer/         # HTML viewer
└── references/         # Documentation
```