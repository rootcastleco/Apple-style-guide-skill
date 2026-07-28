# Design Review Framework

## Review dimensions

### 1. Purpose

- Identify the primary job to be done.
- Confirm that the interface prioritizes the user’s goal rather than the product’s internal model.
- Remove elements that do not support the current task, confidence, or recovery.

### 2. Hierarchy

- Confirm that prominence follows importance.
- Use size, weight, spacing, position, contrast, and motion deliberately.
- Avoid multiple competing primary actions.
- Keep content visually dominant over navigation chrome and decorative materials.

### 3. Information architecture

- Group by user intent and decision sequence.
- Keep navigation levels shallow enough to remain comprehensible.
- Use stable names for the same concept.
- Separate global navigation, local navigation, filters, and object actions.

### 4. Layout and responsiveness

- Define behavior, not one static frame.
- Specify minimum, preferred, and overflow behavior for regions.
- Preserve reading order and task priority across width, orientation, text scaling, and localization changes.
- Use safe areas and platform spacing conventions.
- Avoid clipping, horizontal scrolling for core forms, and controls that move unpredictably between states.

### 5. Components and interaction

- Prefer native or familiar components.
- Make state visible: default, hover, focus, pressed, selected, disabled, loading, error, and success.
- Give interactive targets adequate size and spacing for the platform and environment.
- Preserve keyboard and assistive-technology operation.
- Provide immediate feedback for direct manipulation.
- Use confirmation only when the cost of accidental activation exceeds the interruption cost.
- Prefer undo for reversible destructive actions.

### 6. Navigation and flow

- Make current location and available exits clear.
- Preserve context when moving between list and detail views.
- Avoid dead ends and modal stacks.
- For long flows, show progress, allow back navigation, preserve entered data, and define completion.
- Keep authentication and permission requests proportional to the value already explained.

### 7. Visual system

- Define semantic tokens rather than screen-specific values.
- Use color for meaning, hierarchy, and feedback, not decoration alone.
- Maintain contrast across light, dark, increased-contrast, and material-backed contexts.
- Use typography roles consistently: display, title, heading, body, label, caption, numeric/data.
- Use motion to explain continuity, state, hierarchy, or causality; support reduced motion.

### 8. Accessibility

Review at minimum:

- semantic structure and accessible names
- focus and reading order
- keyboard and switch operation
- text scaling and reflow
- contrast and non-color cues
- reduced motion and transparency
- screen-reader announcements for asynchronous changes
- labels and instructions independent of position, shape, or color
- captions, transcripts, and alternatives for media
- error identification and recovery

Treat WCAG as a baseline for web content, not a complete product-design specification. Apply platform accessibility APIs and patterns as well.

### 9. Localization

- Externalize all user-facing strings.
- Avoid concatenated sentence fragments.
- Support pluralization and grammatical variation.
- Mirror directional layouts semantically, not mechanically.
- Localize formats through platform APIs.
- Test long strings, compact screens, mixed scripts, and right-to-left layouts.

### 10. Privacy, safety, and trust

- Explain data collection and permissions at the decision point.
- Collect the minimum data needed for the feature.
- Distinguish local, synced, shared, and public states.
- Make irreversible, billable, privacy-sensitive, and safety-critical consequences explicit.
- Do not use dark patterns, false urgency, hidden cancellation, or deceptive defaults.

## Design-state matrix

For each important screen or component, verify:

| State | Required definition |
|---|---|
| Initial | Default content, focus, and available actions |
| Loading | Progress behavior, cancellation, timeout |
| Empty | Explanation and next action |
| Partial | Missing or stale data treatment |
| Offline | Local capability, queueing, retry |
| Permission denied | Reduced mode and remediation path |
| Validation error | Location, message, preserved input |
| System error | Recovery, diagnostics, support path |
| Success | Confirmation and next destination |
| Disabled | Reason and method to enable, when useful |

## Review evidence

For every finding, record:

- **Observation:** what is visible or specified
- **Impact:** which user task or quality attribute is affected
- **Recommendation:** the smallest effective change
- **Severity:** P0, P1, P2, or P3
- **Acceptance test:** measurable evidence that the issue is resolved

Avoid unsupported claims such as “users will prefer.” Use “likely,” label the assumption, and recommend validation when evidence is absent.
