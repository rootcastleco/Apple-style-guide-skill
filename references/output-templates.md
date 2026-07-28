# Output Templates

## A. Design audit

# Design audit: [surface or flow]

## Executive assessment
[Two to four sentences on task success, major design risk, and overall direction.]

## Context and assumptions
- Platform:
- Primary user:
- Primary task:
- Constraints:

## Findings

### [P0–P3] [Finding title]
- **Observation:**
- **Impact:**
- **Recommendation:**
- **Acceptance test:**

## Proposed hierarchy
1. Primary content or action
2. Supporting content or actions
3. Secondary and advanced controls

## State coverage
[Initial, loading, empty, partial, offline, permission, error, success, disabled.]

## Accessibility and localization
[Concrete requirements and tests.]

## Rootcastle/REI brand application
[Tokens, material, typography, and restrained brand cues. Omit when not requested.]

## Next three actions
1.
2.
3.

## B. Redesign specification

# Redesign specification: [screen or flow]

## Goal
[User outcome and business/system constraint.]

## Information architecture
[Navigation, regions, grouping, and object hierarchy.]

## Layout behavior
[Responsive behavior, safe areas, density, overflow, and text scaling.]

## Components

### [Component name]
- Purpose:
- Content:
- States:
- Interaction:
- Accessibility:
- Analytics event:

## Exact interface copy
| Element | Copy | Notes |
|---|---|---|

## Failure and recovery
[Validation, offline, timeout, permission, destructive action, and retry behavior.]

## Acceptance criteria
- [Measurable criterion]

## C. UX copy review

# UX copy review: [surface]

| Element | Current | Proposed | Reason |
|---|---|---|---|

## Terminology decisions
- Preferred term:
- Avoided term:
- Capitalization rule:
- Input verb rule:

## Missing states
[List missing empty, error, permission, offline, success, or destructive-action copy.]

## D. Implementation brief

# Implementation brief: [feature]

## Component architecture
[Native/system components first; custom components only with justification.]

## Design tokens
[Semantic tokens, not screen-specific aliases.]

## State machine
[States, events, transitions, guards, and recovery.]

## Accessibility contract
[Names, roles, values, focus, announcements, scaling, contrast, reduced motion.]

## Observability
[Task completion, failure, latency, cancellation, retry, and drop-off events. Do not log sensitive content.]

## Rollout
[Feature flag, migration, fallback, and rollback plan when relevant.]

## Tests
- visual regression
- interaction/state tests
- accessibility tests
- localization and text expansion
- light/dark/high-contrast/reduced-motion modes
- real-device or target-environment validation
