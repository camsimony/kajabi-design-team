# Kajabi Design Framework

How we build at Kajabi. A shared lens for assessing quality.

At Kajabi, everyone contributes to design. Not just designers — engineers, PMs, data, CX, marketers. Because design isn't how something looks. Design is how it works. And we're all shaping how Kajabi works, every day.

Kajabi is powerful and complex under the hood. Our job is to make that power feel simple and trustworthy.

---

## 1. The 80/20 Model

Not all work deserves the same level of investment. If you treat everything the same, you end up either over-investing in things that don't matter, or under-investing in the things that do.

### The 80%: System Patterns

The backbone. List views, forms, settings, edit pages. The predictable, repeatable stuff. Think of it like investing in an index fund — boring, reliable, compounds over time.

Once system patterns are in place, the 80% should almost build itself. Developers read a pitch and start building immediately — no Figma mockup, no prototype. They reach for system patterns and start working. Designers do a QA pass and polish.

The 80% gives Heroes structure.

### The 20%: Magic Experiences

Where the magic happens. The flows Heroes will actually remember:
- Onboarding with Co-Founder
- Generating a website
- Launching a product
- Making a first sale
- Going live with members

This is like a concentrated bet on a company you believe in. Riskier, demands more attention, but when it pays off, it really pays off.

These flows must feel human, guided, and deeply intentional. If it doesn't feel right, it doesn't ship.

The 20% gives Heroes momentum.

### The Effort Flip

- 80% of work (system patterns) → 20% of effort (routine maintenance)
- 20% of work (magic experiences) → 80% of effort and craft

### How to apply

Before any project, ask: **Is this 80% or 20%?**

- If 80%: reach for existing patterns, move fast, aim for consistency
- If 20%: slow down, sweat the details, this is where we earn trust

### Failure modes

- Treating 80% work like 20% work — over-designing CRUD workflows, creating custom Figma prototypes for basic list views
- Treating 20% work like 80% work — rushing magic moments, shipping flows that don't feel right
- Not asking the question at all — defaulting to the same level of effort for everything

---

## 2. Get to the Truth Faster

Everyone sits in a room. They talk about what they're going to build. Everyone nods. Everyone thinks they agree.

Then someone actually builds something. And suddenly it turns out that everyone had a completely different picture in their heads.

**Concrete work reveals the truth.**

The moment something becomes real — something you can actually click through and react to — that's when:
- Assumptions collapse
- Hidden disagreements surface
- Feasibility becomes obvious
- Scope becomes clear

**Mockups are guesses. Working software is truth.**

### How to apply

- Don't spend time crafting decks or debating abstractions
- Build something real, get feedback, iterate
- Ask: What's the smallest complete slice we could ship this week?

### Failure modes

- Staying in the abstract too long
- Perfecting mockups before validating the approach
- False alignment — everyone nodding while imagining different things
- Waiting for certainty before starting — when building creates certainty

---

## 3. Make Complexity Feel Simple

Kajabi is inherently complex. There's a lot happening under the hood. But complexity isn't the enemy. **Confusion is.**

Our job is to absorb complexity so Heroes don't have to deal with it.

**The Slack example:** A diagram went viral showing how Slack decides whether to send a push notification. Presence detection, device fallbacks, notification rules, override logic, timing heuristics. Incredibly complex.

But users experience none of it. They just think: "It notifies me at the right time on the right device."

Slack does the hard work so users don't have to. That's our job too.

### How to apply

Ask: **Are we doing the hard work, or are we pushing it onto Heroes?**

- Hide the complexity, expose the clarity
- Make powerful features feel effortless
- Do the thinking so Heroes don't have to

### Failure modes

- Exposing system internals — making Heroes understand how things work under the hood
- Configuration overload — showing all options because "power users might want them"
- Pushing decisions onto Heroes that the product could make for them
- Confusing complexity with power — assuming more options means more value

---

## 4. Build Taste Through Practice

Taste is what allows us to stand out in a world full of AI slop. It's what allows you to make good judgment calls without needing a rule for every situation.

There's no shortcut. Taste comes from practice. It's a muscle.

### How to apply

- Study products that feel great: Linear, Raycast, Notion, Apple, Airbnb, Ramp
- When something delights you — or frustrates you — pause and ask why
- What did they do here? What did they choose not to do?
- Write it down. Share it with the team.

### Failure modes

- Not studying other products — staying in our own bubble
- Noticing but not reflecting
- Keeping observations private
- Expecting taste to appear without practice

---

## 5. Live the Product

We build perspective by living in the product alongside our Heroes.

This means: create a site, build products and offers, send broadcasts, run automations, explore the admin intentionally. Feel what Heroes feel. See the inconsistencies. Notice what feels good, what feels hard, what feels broken.

**You should always feel slightly discontent about the Kajabi experience.** Not discouraged — energized. "This is good... but how could it be great?"

### How to apply

- Create and maintain your own Kajabi site
- Build real products and offers
- Explore the admin intentionally, not just the areas you work on

### Failure modes

- Only using the parts you build
- Surface-level testing — clicking through without actually using
- Losing the beginner's mind
- Complacency — feeling satisfied with "good enough"

---

## The Checklist

When writing a pitch, reviewing a prototype, or testing a solution:

1. Is this 80% work or 20% work?
2. What's the smallest complete slice we could ship this week?
3. Are we doing the hard work, or pushing it onto Heroes?
4. Can a Hero clearly predict what happens next?
5. Would I be proud to show this to someone I admire?
