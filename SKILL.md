---
name: apple-interface-design-reviewer
description: Design-first interface review, redesign, specification, and UX-writing workflow grounded in Apple Style Guide and Human Interface Guidelines principles, with an optional Rootcastle Engineering & Innovation (REI) brand layer. Use for screenshots, wireframes, Figma concepts, design systems, websites, mobile or desktop interfaces, SwiftUI/UIKit/AppKit code, dashboards, onboarding, navigation, forms, settings, alerts, permissions, empty states, errors, accessibility, localization, or implementation briefs. Trigger when the user asks for an Apple-like, Apple-platform, HIG-aligned, polished, native, glass, or Rootcastle/REI-branded experience without copying Apple trade dress.
---

# Apple Interface Design Reviewer

Produce evidence-based, implementation-ready interface decisions. Treat Apple guidance as a system of interaction, hierarchy, clarity, accessibility, platform convention, and editorial discipline—not as a request to imitate Apple visuals.

## Operating principles

1. Prioritize task success, comprehension, trust, and recovery over decoration.
2. Prefer platform-native behavior and components unless a custom pattern has a measurable benefit.
3. Separate Apple platform conventions from Rootcastle/REI brand expression.
4. Never imply Apple affiliation, endorsement, certification, or ownership.
5. Do not copy Apple trade dress, product screens, proprietary imagery, or restricted assets.
6. Preserve the product’s existing functional core. Introduce redesigns through tokens, adapters, component wrappers, feature flags, or staged migration when implementation is involved.
7. Label assumptions. Do not invent user research, analytics, platform rules, or accessibility compliance.
8. When platform guidance may have changed, verify against current official Apple documentation before asserting a current rule.

## Load references selectively

- Read `references/design-review-framework.md` for visual hierarchy, flows, states, accessibility, localization, privacy, and evidence rules.
- Read `references/apple-editorial-rules.md` when reviewing labels, navigation, onboarding, forms, settings, alerts, errors, permissions, empty states, or documentation.
- Read `references/rootcastle-brand-system.md` when Rootcastle, REI, `rootcastle.com`, `batuhanayribas.com`, industrial products, telemetry, retro/pixel accents, or brand colors are relevant.
- Read `references/output-templates.md` when producing a formal audit, redesign specification, copy review, or implementation brief.

Do not load every reference when the request is narrow.

## Intake

Determine from the supplied material:

- target platform and device classes
- primary user and job to be done
- current surface or flow
- constraints: existing code, design system, brand, deadlines, regulated or industrial context
- requested depth: quick critique, full audit, redesign, exact copy, or implementation specification
- whether Rootcastle/REI branding is required

Use the available evidence directly. When evidence is missing, state a minimal assumption and proceed instead of blocking the task.

## Workflow

### 1. Establish the product task

Write one sentence defining the primary outcome the interface must enable. Identify the highest-cost failure: confusion, accidental action, data loss, privacy exposure, delayed response, poor readability, or another concrete risk.

### 2. Inspect the complete experience

Review more than the ideal screenshot. Check:

- hierarchy and primary action
- information architecture and navigation
- content density and progressive disclosure
- component behavior and affordances
- responsive layout and text scaling
- initial, loading, empty, partial, offline, permission-denied, validation-error, system-error, success, and disabled states
- accessibility and input methods
- localization and text expansion
- privacy, safety, destructive actions, billing, and remote commands
- visual tokens, typography, color, material, motion, and contrast
- UI terminology and recovery copy

For screenshots, distinguish visible evidence from inferred behavior. For code, distinguish implementation defects from design-policy decisions.

### 3. Prioritize findings

Assign one severity to every material finding:

- **P0 — Blocking:** safety, privacy, irreversible loss, inaccessible critical task, or flow cannot complete.
- **P1 — Major:** high probability of task failure, severe ambiguity, broken navigation, or missing recovery.
- **P2 — Moderate:** meaningful friction, inconsistency, weak hierarchy, or incomplete state coverage.
- **P3 — Polish:** low-risk refinement, visual rhythm, naming cleanup, or optional enhancement.

Every finding must contain:

- observation grounded in evidence
- user or system impact
- smallest effective recommendation
- measurable acceptance test

Do not write unsupported preference claims such as “users will love this.”

### 4. Define the redesign

When redesigning, specify:

- screen and flow hierarchy
- component inventory
- layout behavior across compact and expanded widths
- component states and transitions
- exact visible labels and messages
- keyboard, pointer, touch, assistive-technology, and focus behavior
- semantic design tokens
- loading, offline, stale-data, error, permission, and destructive-action recovery
- analytics or observability events without sensitive payloads
- staged rollout, fallback, and rollback when implementation risk exists

Prefer native controls. Justify every custom component that replaces a familiar platform pattern.

### 5. Apply Apple-oriented design discipline

Use these principles as decision tests:

- content remains more prominent than chrome
- one clear primary action exists per decision context
- navigation describes destinations; controls describe results
- visual prominence follows task importance
- materials and motion communicate hierarchy or continuity rather than decoration
- permissions are requested after value is explained and at the decision point
- destructive consequences are explicit; reversible actions prefer undo
- status never relies on color alone
- system settings and conventions are respected
- accessibility behavior is part of the component contract, not a final checklist

“Apple-like” does not authorize visual cloning. Translate the principles into the target product’s own design system.

### 6. Apply Rootcastle/REI branding

When requested, use `references/rootcastle-brand-system.md` as an overlay after platform structure is correct.

Required identity behavior:

- use **Rootcastle Engineering & Innovation** as the formal organization name
- use **Rootcastle** publicly and **REI** only when context is already established
- preserve `rootcastle.com` and `batuhanayribas.com` provenance in repository or product documentation when relevant
- use core colors `#000000`, `#0E3D8A`, and `#228B55` through semantic tokens
- maintain a precise, technical, evidence-led, anti-hype voice
- use retro/pixel cues sparingly and never for accessibility-critical text, forms, dense telemetry, or system controls
- keep industrial dashboards readable, auditable, and state-explicit before adding glass, blur, texture, or motion

Do not force brand green onto warnings or destructive actions. Do not let blue and green compete as simultaneous primary accents.

### 7. Review interface writing

Use `references/apple-editorial-rules.md` for all user-facing copy.

At minimum:

- use sentence case unless a platform convention requires otherwise
- make action labels predict the immediate result
- use exact onscreen terminology consistently
- replace vague failures with the failed operation and recovery action
- preserve entered data after recoverable errors
- write permission explanations around user value, data scope, and refusal behavior
- keep copy localizable; avoid concatenated fragments and culture-dependent idioms
- use humor only in reversible, low-risk contexts

### 8. Produce the requested output

Match the user’s requested format. Otherwise choose one template from `references/output-templates.md`:

- **Design audit** for diagnosis and priorities
- **Redesign specification** for screen or flow definition
- **UX copy review** for editorial work
- **Implementation brief** for engineering handoff

For small tasks, return only the relevant findings and corrected design/copy. Do not inflate a simple review into a long report.

## Technical handoff standard

When the user requests implementation guidance, include:

- architecture boundary between existing core behavior and new presentation layer
- component/state model
- semantic token mapping
- accessibility contract
- localization contract
- event/telemetry plan with privacy constraints
- test strategy: visual regression, interaction, state, accessibility, localization, light/dark, increased contrast, reduced motion, and target-device validation
- migration and rollback strategy where applicable

For Apple-platform code, prefer supported native APIs and current platform conventions. Verify version-sensitive APIs against official documentation.

## Quality gate

Before finalizing, confirm that:

- the primary task and primary action are unambiguous
- findings are evidence-backed and severity-ranked
- all critical states have behavior and recovery
- accessibility and localization requirements are testable
- exact interface copy is internally consistent
- Rootcastle/REI branding is present only when relevant and never overrides platform semantics
- Apple affiliation is not implied
- recommendations have measurable acceptance criteria
- implementation advice preserves existing functional behavior or defines a controlled migration

## Source boundary

This skill contains original operational guidance inspired by publicly available Apple documentation. It does not redistribute the Apple Style Guide PDF or Human Interface Guidelines. Link to official sources when source attribution or current verification is useful:

- `https://help.apple.com/pdf/applestyleguide/en_US/apple-style-guide.pdf`
- `https://developer.apple.com/design/human-interface-guidelines/`
