# AI Agent Prompt: Install Skills Package

Run this prompt to tell the AI agent how to install the skills into your OpenCode system.

---

## Copy and paste the following into your AI conversation:

---

**SYSTEM PROMPT / INSTRUCTIONS FOR AI:**

I have downloaded a skill package called "Create Effective Skills" that contains two skills:
- `signal-skill-framework`
- `skill-creator`

These two skills are located in the folder: **[PATH TO EXTRACTED FOLDER]**

For example, the full path might look like:
- `/Users/YOURNAME/Desktop/create-effective-skills/signal-skill-framework`
- `/Users/YOURNAME/Desktop/create-effective-skills/skill-creator`

Please install both skills into my OpenCode skills directory so I can use them.

Here's what I want you to do:

1. **Find my OpenCode skills folder** - Check common locations:
   - macOS: `~/Library/Application Support/opencode/skills/`
   - Linux: `~/.local/share/opencode/skills/`
   - Windows: `%APPDATA%\opencode\skills\`

2. **If it doesn't exist, create it** - Run: `mkdir -p` with the correct path

3. **Copy both skills into the folder**:
   ```bash
   cp -r [PATH_TO_EXTRACTED_FOLDER]/signal-skill-framework [PATH_TO_SKILLS_FOLDER]/
   cp -r [PATH_TO_EXTRACTED_FOLDER]/skill-creator [PATH_TO_SKILLS_FOLDER]/
   ```

4. **Verify installation** - Confirm the files are copied correctly

5. **Tell me to restart OpenCode** - After restart, both skills will be available

The two skills work together:
- Use `/signal-skill-framework` first to plan skill creation
- Then use `/skill-creator` to build and test

---

## How to fill in [PATH TO EXTRACTED FOLDER]

Before running this prompt, replace the placeholder with your actual folder path:

**On Mac:**
- If you extracted to Desktop: `/Users/YOURNAME/Desktop/create-effective-skills`
- If you extracted to Downloads: `/Users/YOURNAME/Downloads/create-effective-skills`
- If you extracted to Documents: `/Users/YOURNAME/Documents/create-effective-skills`

**On Linux:**
- If you extracted to Home: `~/create-effective-skills`
- If you extracted to Downloads: `~/Downloads/create-effective-skills`

**On Windows:**
- If you extracted to Desktop: `C:\Users\YOURNAME\Desktop\create-effective-skills`
- If you extracted to Downloads: `C:\Users\YOURNAME\Downloads\create-effective-skills`

---

## Example of what to paste (filled in):

---

**SYSTEM PROMPT / INSTRUCTIONS FOR AI:**

I have downloaded a skill package called "Create Effective Skills" that contains two skills:
- `signal-skill-framework`
- `skill-creator`

These two skills are located in the folder: `/Users/YOURNAME/Desktop/create-effective-skills`

Please install both skills into my OpenCode skills directory so I can use them.

Here's what I want you to do:

1. **Find my OpenCode skills folder** - Check common locations:
   - macOS: `~/Library/Application Support/opencode/skills/`
   - Linux: `~/.local/share/opencode/skills/`
   - Windows: `%APPDATA%\opencode\skills\`

2. **If it doesn't exist, create it** - Run: `mkdir -p` with the correct path

3. **Copy both skills into the folder**:
   ```bash
   cp -r /Users/YOURNAME/Desktop/create-effective-skills/signal-skill-framework ~/Library/Application\ Support/opencode/skills/
   cp -r /Users/YOURNAME/Desktop/create-effective-skills/skill-creator ~/Library/Application\ Support/opencode/skills/
   ```

4. **Verify installation** - Confirm the files are copied correctly

5. **Tell me to restart OpenCode** - After restart, both skills will be available

The two skills work together:
- Use `/signal-skill-framework` first to plan skill creation
- Then use `/skill-creator` to build and test

---

## After Installation Testing

Once installed, you can verify by starting a new conversation and typing:
- `/signal-skill-framework` (should load the strategic framework skill)
- `/skill-creator` (should load the skill creator execution skill)

If they respond with their descriptions, you're ready to start building!