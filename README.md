# UI Skills

Opinionated UI constraints extracted from the best design systems. Use these skills to help AI agents build pixel-accurate, consistent interfaces.

## Installation

### Claude Code / Cursor / Copilot

```bash
npx skills add ihlamury/design-skills
```

### Manual Installation

```bash
# Clone the repo
git clone https://github.com/ihlamury/design-skills.git

# Copy a skill to your project
cp -r design-skills/skills/linear ~/.claude/skills/
```

### Direct Download

Download individual `SKILL.md` files from the `skills/` directory.

## Available Skills

| Skill | Style | Description |
|-------|-------|-------------|
| [airbnb](./skills/airbnb/) | Light | Travel platform with warm tones, coral accents |
| [anthropic](./skills/anthropic/) | Light | AI company with warm cream aesthetic |
| [discord](./skills/discord/) | Light | Community platform with signature blurple |
| [github](./skills/github/) | Dark | Developer platform with dark UI |
| [linear](./skills/linear/) | Dark | Developer tool aesthetic with Inter font, 4px grid |
| [mercury](./skills/mercury/) | Dark | Modern banking with lavender accents |
| [notion](./skills/notion/) | Light | Productivity app with clean, minimal design |
| [openai](./skills/openai/) | Light | AI company with clean white aesthetic |
| [robinhood](./skills/robinhood/) | Dark | Fintech with signature green accents |
| [slack](./skills/slack/) | Light | Enterprise messaging with aubergine accent |
| [spotify](./skills/spotify/) | Dark | Music platform with dark charcoal theme |
| [stripe](./skills/stripe/) | Light | Payment platform with blue accents |
| [vercel](./skills/vercel/) | Light | Developer platform with minimal black/white |

## What's Inside Each Skill

Each skill contains:
- **Colors** - Semantic tokens (surface, text, border colors)
- **Typography** - Font families, sizes, weights, text styles
- **Spacing** - Grid system and spacing scale
- **Borders** - Border radius and width scales
- **Layout** - Viewport and component patterns
- **Components** - Button, input, card specifications
- **Interactive States** - Hover, focus, disabled states
- **Animation** - Timing and performance guidelines

## Constraint Hierarchy

- **MUST** - Absolute requirements
- **SHOULD** - Strong recommendations
- **NEVER** - Explicit prohibitions

## Usage with AI Agents

Include the skill in your prompt or project context:

```
Use the Linear UI Skills when building this dashboard interface.
Follow the color tokens, typography, and spacing constraints exactly.
```

## Contributing

Want to add a new design system? Open a PR with:
1. Create `skills/{company}/SKILL.md` with YAML frontmatter
2. Add `skills/{company}/metadata.json`
3. Update this README

## License

MIT
