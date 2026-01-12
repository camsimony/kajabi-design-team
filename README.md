# Kajabi Design Team

AI-powered tools and skills for the Kajabi design team.

## Setup

### Option 1: Claude Code Desktop (recommended for beginners)

1. **Download Claude Code Desktop**
   - Go to [claude.ai/download](https://claude.ai/download)
   - Download and install Claude for Desktop
   - Sign in with your Kajabi enterprise account

2. **Clone this repo**
   - Open GitHub Desktop (download from [desktop.github.com](https://desktop.github.com) if needed)
   - File → Clone Repository
   - Paste: `https://github.com/croswell/kajabi-design-team`
   - Clone to your computer (remember where you saved it)

3. **Open in Claude Code**
   - Open Claude Code Desktop
   - Click the **Code** tab (not Chat)
   - Click **Open folder** and select your `kajabi-design-team` folder

4. **Run a skill**
   - Type a skill command like `/design-review` and press Enter

### Option 2: Claude Code in Terminal

For those comfortable with the terminal:

1. **Install Claude Code**
   ```bash
   npm install -g @anthropic-ai/claude-code
   ```

2. **Clone and open**
   ```bash
   git clone https://github.com/croswell/kajabi-design-team.git
   cd kajabi-design-team
   claude
   ```

3. **Run a skill**
   ```
   /design-review
   ```

## Getting Updates

When skills are updated:

**Desktop:** Open GitHub Desktop → Fetch origin → Pull

**Terminal:**
```bash
git pull
```

## Available Skills

| Skill | Command | Description |
|-------|---------|-------------|
| [Design Review](.claude/skills/design-review/) | `/design-review` | Get feedback on your work against Kajabi's design principles |

## Questions?

Reach out to Sam if you run into any issues.
