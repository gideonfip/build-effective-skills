# AI Agent Prompt: Install Skills

Copy and paste this entire block into your AI conversation:

---

**SYSTEM PROMPT:**

I have a skill package called "Create Effective Skills" at this path:

`/Users/youtube/Documents/GitHub/public/create-effective-skills`

It contains two skills:
- `signal-skill-framework/` — Strategic planning
- `skill-creator/` — Build and test execution

Please install both into my OpenCode skills folder.

**Steps to run:**

```bash
# 1. Find or create your OpenCode skills directory
mkdir -p ~/Library/Application\ Support/opencode/skills/

# 2. Copy both skills
cp -r /Users/youtube/Documents/GitHub/public/create-effective-skills/signal-skill-framework ~/Library/Application\ Support/opencode/skills/
cp -r /Users/youtube/Documents/GitHub/public/create-effective-skills/skill-creator ~/Library/Application\ Support/opencode/skills/

# 3. Confirm installation
ls ~/Library/Application\ Support/opencode/skills/
```

**After restart, use:**
- `/signal-skill-framework` — To plan what to build
- `/skill-creator` — To build and test it

---

## For Non-macOS

| OS | Skills Folder |
|----|---------------|
| macOS | `~/Library/Application Support/opencode/skills/` |
| Linux | `~/.local/share/opencode/skills/` |
| Windows | `%APPDATA%\opencode\skills\` |

---

## What These Skills Do

| Skill | Purpose |
|-------|---------|
| **signal-skill-framework** | Think through WHAT to build before building |
| **skill-creator** | Build, test, and package the skill |

Use them together: Plan first, then build.