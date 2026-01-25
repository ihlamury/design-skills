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
| [linear](./skills/linear/) | Dark mode | Developer tool aesthetic with Inter font, 4px grid |

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
