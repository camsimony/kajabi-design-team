# Kajabi Design Framework

How we build at Kajabi. A shared lens for assessing quality.

At Kajabi, everyone contributes to design. Not just designers — engineers, PMs, data, CX, marketers. Because design isn't how something looks. Design is how it works. And we're all shaping how Kajabi works, every day.

Kajabi is powerful and complex under the hood. Our job is to make that power feel simple and trustworthy.

---

## 1. The 80/20 Model

Here's a question that changes everything: what kind of work are you doing?

Not all work deserves the same level of investment. If you treat everything the same, you end up either over-investing in things that don't matter, or under-investing in the things that do.

Everything we build falls into one of two buckets.

### The 80%: System Patterns

The backbone. List views, forms, settings, edit pages. The predictable, repeatable stuff. Think of it like investing in an index fund — boring, reliable, compounds over time. You're not trying to beat the market. You're trying to be consistent.

Once system patterns are in place, the 80% should almost build itself. Developers read a pitch and start building immediately — no Figma mockup, no prototype. They reach for system patterns and start working. Designers do a QA pass and polish. We don't delay building to wait for designs.

The 80% gives Heroes structure.

### The 20%: Magic Experiences

Where the magic happens. The flows Heroes will actually remember:
- Onboarding with Co-Founder
- Generating a website
- Launching a product
- Making a first sale
- Going live with members

This is like a concentrated bet on a company you believe in. Riskier, demands more attention, but when it pays off, it really pays off.

These flows must feel human, guided, and deeply intentional. If it doesn't feel right, it doesn't ship. We're comfortable delaying these projects to get the experience right.

The 20% gives Heroes momentum.

### The Effort Flip

- 80% of work (system patterns) → 20% of effort (routine maintenance)
- 20% of work (magic experiences) → 80% of effort and craft

### How to apply

Before any project, ask: **Is this 80% or 20%?**

- If 80%: reach for existing patterns, move fast, aim for consistency
- If 20%: slow down, sweat the details, this is where we earn trust

### Failure modes

- Treating 80% work like 20% work — over-designing CRUD workflows, creating custom Figma prototypes for basic list views, delaying builds for designs that aren't needed
- Treating 20% work like 80% work — rushing magic moments, shipping flows that don't feel right because "we can iterate later"
- Not asking the question at all — defaulting to the same level of effort for everything

---

## 2. Get to the Truth Faster

Here's something that happens in product teams every day. Everyone sits in a room. They talk about the thing they're going to build. Everyone nods. Everyone thinks they agree.

Then someone actually builds something. And suddenly it turns out that everyone had a completely different picture in their heads.

This is what happens when we stay in the abstract too long. We think we agree because we're using the same words. But we're actually imagining totally different things.

**Concrete work reveals the truth.**

The moment something becomes real — something you can actually click through and react to — that's when:
- Assumptions collapse
- Hidden disagreements surface
- Feasibility becomes obvious
- Scope becomes clear

This is why we don't stop at mockups. We build small, complete slices — working code you can feel. Something that makes real progress toward the full journey.

**Mockups are guesses. Working software is truth.**

### How to apply

- Don't spend time crafting decks or debating abstractions
- Build something real, get feedback, iterate
- Ask: What's the smallest complete slice we could ship this week?

### Failure modes

- Staying in the abstract too long — endless discussions, decks, and debates without building anything concrete
- Perfecting mockups before validating the approach — polishing Figma files that will change once real constraints surface
- False alignment — everyone nodding in agreement while imagining completely different things
- Waiting for certainty before starting — when building is what creates certainty

---

## 3. Make Complexity Feel Simple

Kajabi is inherently complex. There's a lot happening under the hood. But here's the thing: complexity isn't the enemy. **Confusion is.**

Our job is to absorb complexity so Heroes don't have to deal with it.

**The Slack example:** A few years ago, a diagram went viral showing how Slack decides whether to send a push notification. Presence detection, device fallbacks, notification rules, override logic, timing heuristics. Incredibly complex.

But users experience none of it. They just think: "It notifies me at the right time on the right device."

Slack does the hard work so users don't have to. That's our job too.

### How to apply

When building something, ask: **Are we doing the hard work, or are we pushing it onto Heroes?**

- Hide the complexity, expose the clarity
- Make powerful features feel effortless
- Do the thinking so Heroes don't have to

### Failure modes

- Exposing system internals — making Heroes understand how things work under the hood to use them
- Configuration overload — showing all options and settings because "power users might want them"
- Pushing decisions onto Heroes that the product could make for them
- Confusing complexity with power — assuming more options means more value

---

## 4. Build Taste Through Practice

Taste has become a buzzword, but developing taste is incredibly important. It's what allows us to stand out in a world full of AI slop. It's what allows you to make good judgment calls without needing a rule for every situation.

There's no shortcut. Taste comes from practice. It's a muscle.

If we're in the business of software, we have to be obsessed with good software.

### How to apply

- Study products that feel great: Linear, Raycast, Notion, Apple, Airbnb, Ramp
- When something delights you — or frustrates you — pause and ask why
- What did they do here? What did they choose not to do? Where does the clarity come from?
- Write it down. Share it with the team. This is how we build shared standards.

The more you notice these details, the more naturally you'll apply them to your own work.

### Failure modes

- Not studying other products — staying in our own bubble, only looking at competitors
- Noticing but not reflecting — feeling delight or frustration without pausing to understand why
- Keeping observations private — not sharing learnings with the team, missing the chance to build shared standards
- Expecting taste to appear without practice — waiting for inspiration instead of actively building the muscle

---

## 5. Live the Product

This is maybe the most important one.

We build perspective by living in the product alongside our Heroes. Some people call this dogfooding — but "living the product" gets closer to what we mean.

This means: create a site, build products and offers, send broadcasts, run automations, explore the admin intentionally. Feel what Heroes feel on a day-to-day basis. See the inconsistencies. Notice what feels good, what feels hard, what feels broken.

Living the product builds intuition and empathy. It puts your taste to work in a real context.

**You should always feel slightly discontent about the Kajabi experience.** Not discouraged — energized. "This is good... but how could it be great?"

That's the mindset of world-class product teams. Our work is never complete.

### How to apply

- Create and maintain your own Kajabi site
- Build real products and offers
- Send broadcasts, run automations
- Explore the admin intentionally, not just the areas you work on

### Failure modes

- Only using the parts you build — not experiencing the full Hero journey
- Surface-level testing — clicking through flows without actually using them for real tasks
- Losing the beginner's mind — becoming so familiar with workarounds that you stop noticing friction
- Complacency — feeling satisfied with "good enough" instead of asking "how could it be great?"

---

## The Checklist

When you're writing a pitch, reviewing a prototype, or testing a solution, ask:

1. Is this 80% work or 20% work?
2. What's the smallest complete slice we could ship this week?
3. Are we doing the hard work, or pushing it onto Heroes?
4. Can a Hero clearly predict what happens next?
5. Would I be proud to show this to someone I admire?

---

## The Through Line

These five ideas connect:

- **80/20** tells you where to invest your effort
- **Get to truth faster** keeps you honest about what you're building
- **Make complexity simple** is the craft itself
- **Build taste** sharpens your judgment
- **Live the product** grounds your taste in reality

When we build this way, Kajabi becomes easier to trust, more human, and the operating system that helps real experts move their businesses forward.
