# Sloppify

Sloppify is a Codex skill for removing AI-generated padding from product copy, UI text, and interface structure.

It catches generic copy, duplicated CTAs, over-nested cards, empty affirmations, unnecessary explanations, and polished language that does not help the user.

## Install

Copy the skill into your Codex skills directory:

```sh
mkdir -p ~/.codex/skills/sloppify
cp skills/sloppify/SKILL.md ~/.codex/skills/sloppify/SKILL.md
```

Then restart Codex or reload skills.

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
