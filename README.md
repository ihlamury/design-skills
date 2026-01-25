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

## Usage

### With Claude Code

```bash
# Install all skills
npx skills add ihlamury/design-skills

# Then in your prompt:
# "Build a dashboard using the Linear UI skills"
```

### With Cursor / Copilot

1. Copy the skill file to your project:
```bash
curl -o .cursor/skills/linear.md https://raw.githubusercontent.com/ihlamury/design-skills/main/skills/linear/SKILL.md
```

2. Reference it in your prompt:
```
@linear.md Build a settings page following these design constraints
```

### With Claude.ai

1. Go to Project Knowledge in your Claude project
2. Upload the `SKILL.md` file
3. Claude will automatically follow the constraints

### With Any AI Agent

Copy the contents of any `SKILL.md` file directly into your prompt:

```
You are building a fintech dashboard. Follow these design constraints exactly:

[paste SKILL.md contents here]

Now build me a transaction history component.
```

---

## Example Prompts

**Dashboard:**
```
Using the Linear UI skills, build a project management dashboard with:
- Sidebar navigation
- Project list
- Task cards
```

**Landing Page:**
```
Using the Stripe UI skills, create a pricing page with:
- Three tier cards
- Feature comparison
- CTA buttons
```

**Dark Mode App:**
```
Using the Spotify UI skills, build a music player interface with:
- Album art display
- Playback controls
- Playlist sidebar
```

---

## What You Get

When an AI uses these skills, it will:

- Use the exact color tokens (`#080A0A` instead of arbitrary grays)
- Apply consistent typography (Inter, correct font sizes)
- Follow the spacing grid (4px or 8px increments)
- Match border radius and component styles
- Respect the constraint hierarchy (MUST/SHOULD/NEVER)

## Contributing

Want to add a new design system? Open a PR with:
1. Create `skills/{company}/SKILL.md` with YAML frontmatter
2. Add `skills/{company}/metadata.json`
3. Update this README

## License

MIT
