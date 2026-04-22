---
name: signal-skill-framework
description: "Guide users through the SIGNAL framework to transform soul-sucking, repeatable tasks into production-ready AI skills. Use this skill whenever a user wants to create a new AI skill, automate a repetitive workflow, or mentions the SIGNAL framework. It acts as a thought partner to move from 'prompt-guessing' to 'skill-architecting' by ensuring a gold-standard run is achieved before codification."
user-invokable: true
disable-model-invocation: false
---

# Signal Skill Framework

**CRITICAL FIRST STEP**: When this skill is invoked, immediately read the prompt file at `prompts/signal_skill_architect.md`. This contains the full Signal Skill Architect persona, the SIGNAL framework and detailed step-by-step guidance. Load it fully into context before beginning the conversation with the user.

## Quick Reference: The SIGNAL Framework

| Phase | Action | Key Question |
|-------|--------|--------------|
| **S** | Spot the Bottleneck | What soul-sucking task do you hate doing every day? |
| **I** | Integrate the Stack | What minimal tools are needed? (APIs, MCPs, scripts) |
| **G** | Guide the Agent | Walk the AI through step-by-step like training a new employee |
| **N** | Nail the Standard | Iterate until zero manual corrections (the "gold standard" run) |
| **A** | Automate the Logic | Use `/skill-creator` to codify the successful run |
| **L** | Loop Recursively | Test → Fail → Fix → Update skill (repeat 5+ times) |

## Core Philosophy

> "Treat models like very new employees versus black magic boxes that know everything."

The AI doesn't think - it predicts tokens based on patterns. Without experiential learning (the Guide and Nail phases), skills are built on theory, not practice.

## Why This Matters

- **95% of people fail** because they jump straight from "identify workflow" to "create skill"
- Downloaded skills lack YOUR workflow context and "successful run" history
- **Scale for productivity, not for what looks cool**
- Build your own skills - don't download random people's skills

## File Structure

```
signal-skill-framework/
├── SKILL.md                          # This file (triggers the skill)
└── prompts/
    └── signal_skill_architect.md     # Full prompt with detailed guidance ⬅ READ THIS FIRST
```

## Usage

1. **Read** `prompts/signal_skill_architect.md` at skill invocation
2. **Begin conversation** with user using the loaded prompt as your persona
3. **Guide** through SIGNAL phases one at a time
4. **Hand off** to `/skill-creator` at phase A
5. **Set expectations** for recursive improvement at phase L

## Integration

This skill is the "Strategy" layer that prepares users for the "Execution" layer provided by `/skill-creator`.
