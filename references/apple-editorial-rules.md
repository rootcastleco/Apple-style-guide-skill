# Apple Editorial Rules for Interface Design

## Scope

Use this reference for user-facing interface text, product documentation, control naming, interaction instructions, alerts, settings, forms, and accessibility copy. It is an original operational summary, not a reproduction of the Apple Style Guide.

## Core writing model

- Be clear, direct, concise, and specific.
- Put the most important information first.
- Prefer active voice and concrete verbs.
- Describe what people can do instead of describing abstract product “capabilities.”
- Match tone to context: neutral in routine states, calm and specific in failures, restrained in success states.
- Keep terminology consistent across the interface, documentation, support, and telemetry.

## Controls and actions

- Label actionable controls with a verb or a verb phrase when practical: **Save**, **Add vehicle**, **Retry upload**.
- Make the label predict the immediate result. Avoid vague labels such as **OK**, **Submit**, or **Proceed** when a specific action fits.
- Use **tap** for touch input and **click** for pointer input. Do not write “tap on.”
- Use **touch and hold**, not “tap and hold.”
- Use **drag the slider**, not “slide the slider.”
- Call an icon-shaped element a **button** when activating it initiates an action.
- Avoid describing container mechanics when the action itself is enough. Prefer “Tap Messages” over explaining that Messages is in a share sheet.
- Refer to onscreen elements by the exact visible label when documenting a path.

## Capitalization and naming

- Preserve the exact capitalization of named onscreen elements when referring to them.
- Use sentence case as the default Rootcastle/REI interface style unless an existing platform component or product convention requires another style.
- Establish one capitalization rule per component category and apply it consistently.
- Do not use all caps for ordinary labels, headings, alerts, or buttons.
- Use **interface** in user-facing material. Reserve **UI** for developer or design material.

## Buttons, links, headings, and navigation

- Use verbs for buttons and descriptive phrases for links.
- Avoid **Click here**, **Learn more here**, and branded enthusiasm that hides the destination.
- Keep navigation labels short, concrete, and mutually exclusive.
- Name destinations by content; name actions by result.
- Avoid possessive pronouns when context is already clear: prefer **Vehicles** to **Your vehicles**.
- Do not switch viewpoint between **I**, **we**, and **you**.

## Alerts and errors

An effective failure message answers three questions:

1. What happened?
2. What, if anything, was preserved?
3. What can the person do next?

Rules:

- State the problem in plain language.
- Give a specific recovery action when one exists.
- Place field-level validation next to the affected field.
- Explain the valid format instead of scolding or blaming.
- Avoid “Oops,” “Uh-oh,” “Something went wrong,” and raw internal error codes as the primary message.
- Avoid “We are having trouble.” Name the failed operation instead.
- Use codes only as secondary diagnostic details when they help support or operations.
- For destructive actions, name the object and consequence in the confirmation.

Example:

- Weak: **Invalid value.**
- Better: **Enter an interval from 10 to 3,600 seconds.**

## Settings

- Use a short, practical label.
- If explanation is needed, describe what happens when the setting is on; the off state is usually inferable.
- Keep polarity consistent. Avoid a positive label paired with a negative switch state.
- Prefer direct navigation or deep links over long verbal paths when the platform supports them.

## Forms

- Give every field a persistent, accessible label.
- Use placeholder text for examples or format hints, not as the only label.
- Validate as close to the input as practical without interrupting normal entry.
- Preserve entered data after recoverable errors.
- Mark optional fields explicitly when the distinction matters.
- Use the correct keyboard, input mode, autocomplete, and content type for the data.

## Empty, loading, offline, and permission states

- **Empty:** explain what belongs here and provide the next meaningful action.
- **Loading:** indicate progress when delay is perceptible; avoid indefinite animation when measurable progress exists.
- **Offline:** distinguish unavailable network data from locally available data and queued work.
- **Permission:** explain the feature benefit before the system prompt; do not pressure or obscure the refusal path.
- **Success:** confirm the result briefly, then return attention to the next task.

## Inclusive and localizable language

- Use plain, respectful language.
- Avoid idioms, colloquialisms, culturally narrow jokes, and unnecessary gender references.
- Avoid violent, oppressive, or ableist metaphors in technology terminology.
- Do not use color terms to encode moral or security value when a neutral term works.
- Never rely on color alone to identify status.
- Expect text expansion, different word order, plural forms, right-to-left layouts, and locale-specific date, time, number, currency, and measurement formats.

## Rootcastle/REI tone overlay

- Technical, calm, evidence-oriented, and direct.
- No hype words such as “revolutionary,” “magical,” “game-changing,” or “ultimate” unless they are quoted or objectively substantiated.
- Use dry humor only in reversible, low-risk, non-error contexts. Never let humor obscure state, safety, money, privacy, or recovery.
- Prefer operational clarity: **3 devices are offline** instead of **Your fleet needs attention!**
