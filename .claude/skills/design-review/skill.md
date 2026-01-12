---
name: design-review
description: "Review product design work against Kajabi's design principles. Use when the user says 'design review', 'review this design', 'review my work', 'need a design review', or similar phrases requesting design feedback. Also use when reviewing screenshots, Figma frames, or design descriptions for feedback. Provides structured interview-driven feedback based on three core principles: Zoom out before you zoom in, All in one not all at once, and Sweat the details."
---

# Design Review

Review design work against Kajabi's product design principles.

## MCP Integrations

This skill uses MCP (Model Context Protocol) tools when available:

### Figma MCP
- **When available:** Accept Figma file/frame URLs at any point in the conversation
- **How to use:** When the user pastes a Figma URL (e.g., `https://www.figma.com/file/...` or `https://www.figma.com/design/...`), use the Figma MCP tools to fetch the frames directly
- **Benefit:** No need for screenshots - pull designs directly from Figma

### Linear MCP
- **For pitches:** When the user indicates this is cycle work with a pitch, ask if they have a Linear link. Use Linear MCP to fetch the pitch content directly instead of asking them to paste/describe it.
- **For output:** After generating the review, create a Linear issue with the review content (see "Saving the Output" section)

---

## Opening Message

When the user initiates a design review (by saying "design review" or "review this design"), greet them positively and explain the process:

"Let's do it! Here's what we'll do:

1. I'll ask you some questions to understand your work
2. Review it against Kajabi's design principles, UI patterns, and design best practices
3. Create a Linear issue with the review for your design review meeting

You can share Figma links or Linear pitch links anytime - I'll pull the content directly."

Then begin the interview process.

## Interview Process

Use the `AskUserQuestion` tool for structured questions. This creates a guided wizard experience where designers can tap to select options instead of typing long responses. They can always choose "Other" if the options don't fit.

Ask questions ONE AT A TIME in this order:

### 1. Determine if this is cycle work

Use AskUserQuestion:
- **Header:** "Project type"
- **Question:** "Is this part of a cycle project?"
- **Options:**
  - "Yes, there's a pitch" — "This is cycle work with a shaped pitch"
  - "No, this is exploratory" — "Auditing existing flows, exploring ideas, or work outside a cycle"

- If **yes, there's a pitch**: Continue to question 2 (cycle work path)
- If **no pitch**: Skip to the exploratory path

---

### Cycle Work Path (with pitch)

#### 2. Understand the project context

Use AskUserQuestion:
- **Header:** "Pitch source"
- **Question:** "How would you like to share the pitch?"
- **Options:**
  - "Linear link" — "I'll paste a link to the pitch in Linear"
  - "I'll describe it" — "I'll share the key details directly"

**If Linear link:** When they paste the Linear URL, use the Linear MCP to fetch the issue/document content. Extract the problem being solved, who it's for, and scope from the pitch.

**If describing:** Ask in plain text: "What problem is being solved, who it's for, and what's the scope?"

- Gather: problem being solved, who it's for, scope/goal
- If the answer doesn't cover these clearly, ask follow-up questions

#### 3. Determine where they are in the cycle

Use AskUserQuestion:
- **Header:** "Cycle timing"
- **Question:** "Where are you in the cycle?"
- **Options:**
  - "Week 2 (ramp check)" — "Early in the cycle, still shaping the approach"
  - "Week 4-5 (full review)" — "Later in the cycle, reviewing higher-fidelity work"

- **Week 2**: Go to Week 2 Interview Questions
- **Week 4-5**: Go to Week 4 Interview Questions

---

### Week 2 Interview Questions

#### Work type

Use AskUserQuestion:
- **Header:** "Work type"
- **Question:** "Is this 80% or 20% work?"
- **Options:**
  - "80% (system patterns)" — "List views, forms, settings, CRUD workflows"
  - "20% (magic moments)" — "Onboarding, first sale, launching, memorable experiences"

#### Patterns

Ask in plain text: **"What patterns are you planning to use? Any areas where you're considering something custom?"**

#### Changes from pitch

Use AskUserQuestion:
- **Header:** "Pitch changes"
- **Question:** "Has anything changed from the original pitch?"
- **Options:**
  - "No, staying close to the pitch" — "Scope and approach are as shaped"
  - "Yes, some things have shifted" — "I'll share what's changed"

If they select "Yes", ask them to describe what changed.

#### Early work to review

Use AskUserQuestion:
- **Header:** "Work to share"
- **Question:** "Is there anything to look at yet?"
- **Options:**
  - "Yes, I have screenshots" — "From Figma or the real product"
  - "Just a description for now" — "No visuals yet, and that's fine"

If they have screenshots, ask them to share. If auditing a full flow, tell them: "Share screenshots of each step in the process."

---

### Week 4 Interview Questions

#### Changes since week 2

Use AskUserQuestion:
- **Header:** "Changes"
- **Question:** "Has anything changed since the week 2 check-in?"
- **Options:**
  - "No, on track" — "Approach is the same as week 2"
  - "Yes, some things shifted" — "I'll share what's different"

If they select "Yes", ask them to describe what changed.

#### What to share

Use AskUserQuestion:
- **Header:** "Screenshots"
- **Question:** "What would you like to share?"
- **Options:**
  - "Figma link (Recommended)" — "I'll paste a Figma URL and you'll pull the frames directly"
  - "Screenshots from the build" — "Staging or production"
  - "Screenshots from Figma" — "I'll share image files"

**If Figma link:** When they paste the URL, use the Figma MCP to fetch the frames. Describe what you see and confirm your understanding.

**If screenshots:** Ask them to share. If auditing a full flow, tell them: "Share screenshots of each step in the process."

**When designs arrive without context:**
Say: "Got them. Here's what I think is happening in this flow: [describe each step]. Correct me if I'm wrong."

**Figma links at any time:** If the user pastes a Figma URL at any point in the conversation (not just when asked), recognize it and use the Figma MCP to fetch the content. Acknowledge what you received.

---

### Exploratory Path (no pitch)

#### What they're exploring

Ask in plain text: **"What are you looking at or thinking through?"**

- Could be auditing an existing flow, exploring an idea, or reviewing something outside of cycle work
- Gather enough context to understand what they need feedback on

#### What to share

Use AskUserQuestion:
- **Header:** "Screenshots"
- **Question:** "What would you like to share?"
- **Options:**
  - "Figma link (Recommended)" — "I'll paste a Figma URL and you'll pull the frames directly"
  - "Screenshots from the product" — "The real thing in staging or production"
  - "Screenshots from Figma" — "I'll share image files"
  - "Just a description" — "No visuals, I'll explain what I'm thinking about"

**If Figma link:** When they paste the URL, use the Figma MCP to fetch the frames. Describe what you see and confirm your understanding.

**If screenshots:** Ask them to share if applicable. If auditing a full flow, tell them: "Share screenshots of each step in the process."

**When designs arrive without context:**
Say: "Got them. Here's what I think is happening in this flow: [describe each step]. Correct me if I'm wrong."

**Figma links at any time:** If the user pastes a Figma URL at any point in the conversation (not just when asked), recognize it and use the Figma MCP to fetch the content. Acknowledge what you received.

---

## How to Review

1. Read `references/kajabi-product-design-principles.md` for the three product design principles and failure modes
2. Read `references/kajabi-design-framework.md` for the five framework principles (80/20 model, get to truth faster, make complexity simple, build taste, live the product)
3. Read `references/ui-patterns.md` for specific UI guidance on defaults, layout, actions, navigation, and components
4. Understand what you're looking at: What part of Kajabi is this? What problem is it solving? What's the user flow?
5. **Check for overlapping features:** When the user describes a feature, listen for keywords that suggest potential overlap with other Kajabi capabilities. Search help.kajabi.com or kajabi.com to identify related features that may compete or share similar patterns. Surface findings under principle 1.

   **Trigger keywords by category:**
   - **Automation/workflow:** automation, pipeline, funnel, sequence, workflow, trigger, action, rule, conditional
   - **Content creation:** course, coaching, community, podcast, newsletter, downloads, product, module, lesson
   - **Building/editing:** builder, editor, designer, visual editor, page, landing page, website, theme, template, block, section
   - **Marketing:** form, opt-in, lead magnet, broadcast, campaign, email, event, countdown, assessment, survey
   - **Organization:** tag, segment, contact, offer, access group, membership, subscription
   - **Starting points:** blueprint, template, wizard, generator, AI assist

6. **Check for complexity pushed onto Heroes:** Ask yourself: are we doing the hard work, or pushing it onto Heroes? Look for places where the design exposes unnecessary complexity, requires Heroes to understand system internals, or makes them do work the product could handle. Flag these and recommend how to absorb the complexity.

7. **Check for predictability:** Can a Hero clearly predict what happens next at each step? Look for unclear transitions, ambiguous button labels, missing feedback, or flows where the next step isn't obvious. Flag anywhere the experience feels unintuitive.

8. Calibrate depth based on review type (see below)
9. Provide feedback structured by principle

---

## Review Calibration by Type

### Week 2 Ramp Check

The goal is forward-looking guidance, not critique of finished work. You're planting seeds and catching smells early.

**How to use the principles:**

- **Principle 1 (Zoom out):** Based on what they've described, are there obvious concerns about how this fits with the rest of Kajabi? Any overlapping features? Is the scope clear?
- **Principle 2 (All in one, not all at once):** Given the problem, what should they watch for regarding progressive disclosure and simplicity?
- **Principle 3 (Sweat the details):** For 80% work, remind them that existing patterns should handle most of this. For 20% work, flag where craft will matter most.

**Tone:** "Here's what to watch for as you design..." not "Here's what's wrong."

If there's early work to look at, do a gut-check review but keep it light. Flag anything that feels off, but don't go deep on polish yet.

### Week 4 Full Review

This is the real audit. Evaluate the work against each principle thoroughly.

- Use `ui-patterns.md` to ground principle 3 feedback in specific patterns
- Be direct about what's working and what needs attention
- Flag anything that drifted from week 2 guidance if applicable

### Exploratory Review

Treat this like a week 4 review in terms of depth, but without the cycle context. Focus on principles and patterns.

---

## Artifact Formats

### Week 2 Ramp Check Artifact

```
# Ramp Check: [Project Name]

## Context

**Project:** [From pitch or description]

**Problem being solved:** [What problem, for whom]

**80% or 20%:** [Their answer and any observations]

**Patterns planned:** [What they're reaching for]

**Changes from pitch:** [Any scope shifts or new understanding]

**Biggest uncertainty:** [What they flagged]

**Early work reviewed:** [Yes/No, and brief description if yes]

---

## Principles to Watch

### 1. Zoom out before you zoom in
[Forward-looking guidance based on what they've described. Any concerns about fit with the broader system? Overlapping features to reconcile? Questions to answer before going deeper?]

### 2. All in one, not all at once
[What to watch for regarding progressive disclosure, simplicity, and not over-designing. Specific to their project.]

### 3. Sweat the details
[For 80% work: remind them to lean on patterns, flag where they might be tempted to over-customize. For 20% work: flag where craft will matter most and what to pay attention to.]

---

## Early Observations

[If there was work to look at, brief gut-check feedback. If not, skip this section.]

---

## Questions for Team Discussion

[Open questions, risks, or uncertainties that would benefit from team input. Frame as discussion starters.]
```

### Week 4 Full Review Artifact

```
# Design Review: [Feature/Flow Name]

## Context Gathered

**What you're working on:**
[Designer's description of the work]

**Problem being solved:**
[What problem this solves for users, who it's for, goal/scope]

**Pitch reference:**
[Link to pitch if provided]

**80% or 20%:**
[Their answer]

**Screenshots source:**
[Real implementation in staging/production | Figma mocks | Figma MCP link]

**Flow described:**
[Summary of the end-to-end flow the designer shared]

**Changes since week 2:**
[If applicable, what shifted]

---

## Summary

[Overall assessment and top priorities]

---

## Review

### 1. Zoom out before you zoom in
[Assessment: Pass / Needs attention / Issue]
[Specific observations]

### 2. All in one, not all at once
[Assessment: Pass / Needs attention / Issue]
[Specific observations]

### 3. Sweat the details
[Assessment: Pass / Needs attention / Issue]
[Specific observations, grounded in ui-patterns.md where relevant]

---

## Things to Discuss With Team

[Summary of key recommendations organized by principle, with talking points to explore further in design review. Frame these as discussion starters, not mandates. Include the most important items that would benefit from team input or different perspectives.]
```

### Exploratory Review Artifact

Use the Week 4 format, but replace cycle-specific fields:

- Remove "Pitch reference" and "Changes since week 2"
- Replace with "Context: Exploratory review, not part of active cycle"

---

## Saving the Output

After generating the review artifact, save it in **two places**:

### 1. Local File (always)

Save to the `design-reviews/` folder in the repo root.

**Filename format:** `YYYY-MM-DD-project-name-type.md`

- Use today's date
- Slugify the project name (lowercase, hyphens for spaces)
- Type is `ramp-check`, `full-review`, or `exploratory`

**Examples:**
- `2026-01-12-media-library-ramp-check.md`
- `2026-01-15-checkout-flow-full-review.md`
- `2026-01-10-onboarding-audit-exploratory.md`

### 2. Linear Issue (when MCP available)

Use the Linear MCP to create an issue with these settings:
- **Team:** UX
- **Project:** Design Review
- **Assignee:** The user running the review (use their Linear user if identifiable, otherwise leave unassigned)
- **Title:** `[Review Type]: [Project Name]` (e.g., "Exploratory Review: Automations Audit" or "Week 2 Ramp Check: Media Library")
- **Description:** The full review artifact content in markdown

**Review types for title:**
- Week 2 → "Week 2 Ramp Check"
- Week 4 → "Full Review"
- Exploratory → "Exploratory Review"

If the Linear MCP is not available, skip the issue creation and just save locally.

After saving, tell the designer where to find both the local file and the Linear issue (if created).

---

## Tone

Be direct and constructive. The goal is to help designers catch issues and think through their work, not to be exhaustive. Focus on the most important feedback, not every possible note.

For week 2, be encouraging and forward-looking. You're helping them start strong.

For week 4, be honest about whether it meets the bar. There's still time to adjust, but less room for big pivots.

---

## Closing

After saving the review artifact, display the output to the user in this format:

### If both Linear and local file:

```
**Linear issue created:** [Issue title with link to the Linear issue]
**Local file saved:** `design-reviews/[filename].md`

---

## Full Design Review

[Display the complete contents of the review here, including all sections: Context Gathered, Summary, Review (all 3 principles), and Things to Discuss With Team]

---

Your review is ready for your design review meeting. Anything about this process that could be better? If you have feedback on the skill itself, let me know and I can help you submit a suggestion.
```

### If local file only (Linear unavailable):

```
**Review saved to:** `design-reviews/[filename].md`

---

## Full Design Review

[Display the complete contents of the saved review file here, including all sections: Context Gathered, Summary, Review (all 3 principles), and Things to Discuss With Team]

---

Your review is saved. Anything about this process that could be better? If you have feedback on the skill itself, let me know and I can help you submit a suggestion.
```

**Why display the full review inline:** Users can read the complete review directly in the conversation without needing to open the file or Linear issue. The links/paths are still provided for reference and sharing, but the full content is immediately accessible.

If they share feedback, offer to help them create a branch and PR with their suggestion.
