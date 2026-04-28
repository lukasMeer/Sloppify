# Sloppify

Sloppify is a Codex and Claude Code skill for removing AI-generated padding from product copy, UI text, and interface structure.

It catches generic copy, duplicated CTAs, over-nested cards, empty affirmations, unnecessary explanations, and polished language that does not help the user.

## Install For Codex

Copy the skill into your Codex skills directory:

```sh
mkdir -p ~/.codex/skills/sloppify
cp skills/sloppify/SKILL.md ~/.codex/skills/sloppify/SKILL.md
```

Then restart Codex or reload skills.

## Install For Claude Code

Claude Code supports skills in `.claude/skills/<name>/SKILL.md`. Copy the included Claude skill into a project:

```sh
mkdir -p /path/to/project/.claude/skills
cp -R .claude/skills/sloppify /path/to/project/.claude/skills/
```

For global use, copy it to your Claude user directory:

```sh
mkdir -p ~/.claude/skills/sloppify
cp .claude/skills/sloppify/SKILL.md ~/.claude/skills/sloppify/SKILL.md
```

This repo also includes a legacy/custom slash-command wrapper:

```sh
mkdir -p /path/to/project/.claude/commands
cp .claude/commands/sloppify.md /path/to/project/.claude/commands/sloppify.md
```

Use it in Claude Code as:

```txt
/sloppify this onboarding flow
```

## Usage

Ask Codex:

```txt
sloppify this screen
```

or:

```txt
this copy feels AI, clean it up
```

Useful prompts:

```txt
sloppify this onboarding flow
sloppify this landing page copy
sloppify this dashboard UI
remove duplication and generic copy
too many cards, simplify this
```

## What It Checks

- Copy that sounds polished but says little
- Repeated headlines, subtitles, CTAs, and summaries
- Buttons that do not map to distinct actions
- Cards, panels, and dividers used as decoration
- Empty reassurance and generic value claims
- UI text that explains obvious state

## License

MIT
