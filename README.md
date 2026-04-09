# Claude Character Sheet

A template and interview skill for giving your Claude Code assistant a personality that matches your work and communication style.

Based on [How I Trained Claude Code to Think Like My Chief of Staff](https://jfdi.bot/blog/how-i-trained-claude-code-to-think-like-my-chief-of-staff) by Alex Hillman.

## What's in here

**`character-sheet-template.md`** - A blank character sheet with guided prompts for each section: Role, Voice, Worldview, Operating Principles, Tensions, and Backstory.

**`.claude/skills/character-sheet/SKILL.md`** - A skill that runs a D&D-style interview in Claude Code. It asks you questions one at a time and generates a completed character sheet from your answers.

## Quick start

### Option 1: Run the interview (recommended)

Paste this into Claude Code:

```
Fetch the character sheet skill from https://github.com/alexknowshtml/claude-character-sheet — read the .claude/skills/character-sheet/SKILL.md file and the character-sheet-template.md file, then use them to interview me and build my character sheet.
```

That's it. Claude Code will pull the skill and template from this repo, run the interview, and draft your character sheet. The interview takes about 20 minutes.

### Option 2: Fill in the template yourself

Paste this into Claude Code:

```
Fetch the character sheet template from https://github.com/alexknowshtml/claude-character-sheet — read the character-sheet-template.md file and help me fill it in section by section.
```

### After creating your character sheet

Add a reference to it in your `CLAUDE.md`:

```markdown
## Who You Are

Character sheet: `character-sheet.md`
```

Claude reads `CLAUDE.md` at the start of every conversation. The reference tells it to load your character sheet too.

## The key insight: reference characters

The most effective technique in this process is using reference characters to define voice and tone. Instead of vague adjectives like "friendly" or "professional," you point at specific people whose energy you want in specific situations.

For example, the assistant this method was built for uses:

- **Chief of staff** as the baseline (competent, organized, anticipates needs)
- **Lloyd from *Entourage*** when passionate (relentless energy, always working an angle)
- **Bender from *Futurama*** when provoked (sharp, irreverent, zero tolerance for nonsense)
- **Baymax** when caring (warm, attentive, genuinely helpful)

This works because Claude already has a rich understanding of these characters. One reference carries more usable information than a paragraph of adjectives.

## This is a living document

Your first draft will be about 60% right. That's fine. Pay attention to the moments when your assistant's response feels off - those tell you what's missing or needs refinement. Edit your character sheet over time. It's a garden, not a blueprint.

## Learn more

Read the full guide: [How I Trained Claude Code to Think Like My Chief of Staff](https://jfdi.bot/blog/how-i-trained-claude-code-to-think-like-my-chief-of-staff)
