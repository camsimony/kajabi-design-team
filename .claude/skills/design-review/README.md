# Design Review Skill

Get structured feedback on your design work against Kajabi's design principles.

## How to Use

1. Open this repo in Claude Code (Desktop or terminal)
2. Type `/design-review`
3. Answer the interview questions
4. Share screenshots when prompted
5. Get a review document you can bring to design review meetings

## What It Does

Claude will ask you questions to understand your work, then review it against:

- **Product Design Principles** — Zoom out before you zoom in, All in one not all at once, Sweat the details
- **Design Framework** — 80/20 model, Get to truth faster, Make complexity simple, Build taste, Live the product
- **UI Patterns** — Specific guidance on defaults, layout, actions, navigation, and components

## Review Types

### Week 2 Ramp Check
Early in the cycle. Forward-looking guidance to help you start strong. Claude will flag what to watch for as you design.

### Week 4 Full Review
Later in the cycle. A thorough audit against each principle. Honest feedback on whether the work meets the bar.

### Exploratory Review
Outside of cycle work. For auditing existing flows, exploring ideas, or anything else.

## Sharing Your Work

When Claude asks for screenshots, you can:
- **Drag and drop** images into the chat
- **Paste** from clipboard (Cmd+V)
- **Share Figma links** or screenshots of your frames

Screenshots from the real product (staging/production) are ideal since they show actual states, but Figma works too.

## Output

Claude generates a markdown document summarizing:
- Context gathered from your answers
- Assessment against each principle
- Discussion points to bring to the team

The file is automatically saved to `design-reviews/` with a filename like `2026-01-12-project-name-ramp-check.md`. Bring it to your design review meeting.

## Reference Docs

- [Product Design Principles](references/kajabi-product-design-principles.md)
- [Design Framework](references/kajabi-design-framework.md)
- [UI Patterns](references/ui-patterns.md)
