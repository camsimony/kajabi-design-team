# UI Patterns

Specific guidance for common UI decisions. Use these patterns when evaluating design work against principle 3 (Sweat the details) and when assessing whether a design reduces cognitive load.

---

## Defaults & Mental Load

### Smart defaults over blank slates

Pre-fill forms and configurations with reasonable defaults so users edit rather than build from scratch. The system often knows enough to make a good guess.

**Do this:**
- Blueprint selects "Freebie Funnel" → pre-fill a form, auto-generate a tag name, suggest an offer
- Email subject line → pre-fill with something editable like "Your [product name] is ready"
- New page → start with a sensible template, not a blank canvas

**Not this:**
- Empty form fields showing as errors before the user has touched them
- Requiring users to name something before they know what it is
- Blank states that require configuration before you can see what you're building

**Why it matters:** Every blank field is a decision. Defaults reduce decisions and let users focus on what's actually unique to their situation.

---

### Incomplete vs. broken

Distinguish "you haven't done this yet" from "something is wrong." In-progress states aren't errors until you try to publish or save.

**Do this:**
- Show the next incomplete step as "Start here" or "Next up"
- Use neutral indicators (empty circles, gray states) for untouched steps
- Only show red/error states after the user has interacted with a field or tried to publish

**Not this:**
- Three red error dots on a flow you just started
- "Missing required input" on fields you haven't touched yet
- Disabled save buttons with no indication of what's blocking

**Why it matters:** Showing errors before users have had a chance to act creates anxiety and makes the product feel hostile.

---

## Content & Communication

### Show, don't tell

Use icons, diagrams, and visual differentiation instead of walls of text. When users are scanning a grid of options, visual distinctiveness matters more than descriptive copy.

**Do this:**
- Give blueprint categories distinct icons or illustrations
- Use color, iconography, or layout to differentiate items in a list
- Let the visual hierarchy do the explanatory work

**Not this:**
- 27 cards that all look identical except for their title and description
- Relying on users to read every description to understand differences
- Text-heavy explanations when a diagram would be clearer

**Why it matters:** Users scan before they read. If everything looks the same, nothing stands out.

---

### Text economy

Headlines should be scannable. Descriptions should be optional context, not required reading.

**Do this:**
- Headlines that communicate the core idea in 3-5 words
- Descriptions that add nuance for users who want it
- UI labels that are precise and minimal

**Not this:**
- Needing a paragraph to explain what a feature does
- Headlines that bury the point in qualifiers
- Redundant text that says the same thing the UI already shows

**Why it matters:** If users have to read carefully to understand what they're looking at, the design is making them work too hard.

---

## Actions & Hierarchy

### One primary action per view

Every screen has one thing you're supposed to do next. Secondary and tertiary actions exist but don't compete for attention.

**Do this:**
- One filled/primary button per view
- Secondary actions as outlined or text buttons
- Destructive actions visually distinct and positioned away from primary

**Not this:**
- Three buttons that all look equally important
- Primary actions buried in a menu
- "Save" and "Delete" styled the same and positioned next to each other

**Why it matters:** If everything is emphasized, nothing is. Users should know instantly what the expected next step is.

---

### Progressive disclosure for advanced features

Surface advanced options when users reach for them, not before. Most users don't need most options most of the time.

**Do this:**
- Hide "Add another trigger" until someone has configured the first one
- Put advanced settings in an expandable section or secondary view
- Default to the simple path, let power users dig deeper

**Not this:**
- Showing "Add trigger" next to an empty trigger on a flow that typically needs one
- Exposing every configuration option on the first screen
- Making users wade through advanced settings to complete basic tasks

**Why it matters:** Advanced features shown too early create confusion and suggest complexity that most users don't need to engage with.

---

## Navigation & Orientation

### Persistent wayfinding

In multi-step flows, users should always know where they are in the journey. Keep navigation visible while content changes.

**Do this:**
- Sidebar or stepper that shows all steps with current step highlighted
- Breadcrumbs for hierarchical navigation
- Mini-maps or progress indicators for linear flows

**Not this:**
- Flows where you lose context of the whole when editing a part
- Multi-step processes with no indication of how many steps remain
- Drilling into content and losing track of where you came from

**Why it matters:** Disorientation creates anxiety. Users should always be able to answer "where am I?" and "how do I get back?"

---

### Navigation depth limit

Three levels max before reconsidering the pattern. Deep hierarchies hide content and exhaust users.

**Do this:**
- Main nav → Section → Detail (three levels)
- Flatten hierarchies by using tabs, filters, or search instead of nesting
- Question whether a fourth level is actually necessary

**Not this:**
- Five clicks to reach a common destination
- Nested folders within nested folders
- Hierarchies that mirror backend data structures instead of user mental models

**Why it matters:** Every level of navigation is a decision and a potential wrong turn. Shallow structures are more forgiving.

---

## Component Choices

### Modal vs. drawer vs. inline

Choose the right container for the interaction.

**Modal:** Confirmations, focused decisions, interruptions that require resolution. User must act before continuing. Keep modals small and focused.

**Drawer (slide-in panel):** Editing something in context while keeping the main view visible. Good for forms that relate to a selected item. Can be dismissed without completing.

**Inline:** Anything that's part of the main flow. Expanding sections, inline editing, progressive disclosure within the page.

**Do this:**
- "Are you sure you want to delete?" → Modal
- Edit automation step details → Drawer
- Expand to show advanced settings → Inline

**Not this:**
- Complex multi-field forms in a modal
- Modals that require scrolling
- Drawers for simple confirmations

**Why it matters:** The wrong container makes simple tasks feel heavy and complex tasks feel cramped.

---

### Empty states are onboarding

Empty states should guide users toward their first action, not just acknowledge emptiness.

**Do this:**
- "Create your first automation to send emails when someone signs up"
- Include a clear CTA and optionally a brief explanation or illustration
- Consider linking to help content or examples

**Not this:**
- "No automations yet."
- Empty tables with just column headers
- Blank screens with only a "+" button

**Why it matters:** Empty states are a user's first impression of a feature. They're an opportunity to teach and motivate, not just a placeholder.
