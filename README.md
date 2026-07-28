# Apple Interface Design Reviewer

A design-first ChatGPT Skill for reviewing and specifying interfaces with current Apple Style Guide and Human Interface Guidelines principles, plus an optional Rootcastle Engineering & Innovation (REI) brand layer.

## What it does

- audits screenshots, wireframes, prototypes, UI code, design systems, and UX copy
- improves hierarchy, navigation, flows, controls, forms, alerts, settings, and empty states
- produces implementation-ready component, state, accessibility, localization, and acceptance specifications
- applies Rootcastle/REI branding without copying Apple trade dress or weakening platform conventions
- supports industrial dashboards, telemetry products, mobile apps, websites, and Apple-platform experiences

## Install

Package the repository with the official ChatGPT Skill tooling, or download the `skill.zip` artifact produced by the repository workflow, then upload it to ChatGPT Skills.

## Structure

```text
SKILL.md
agents/openai.yaml
references/
  apple-editorial-rules.md
  design-review-framework.md
  output-templates.md
  rootcastle-brand-system.md
```

## Example prompts

- “Review this fleet dashboard and produce a P0–P3 design audit.”
- “Rewrite the onboarding, permission, empty-state, and error copy for iOS.”
- “Redesign this settings flow using Apple interaction principles and REI branding.”
- “Turn this screenshot into an implementation-ready component and state specification.”
- “Apply Rootcastle colors and retro accents without compromising accessibility.”

## Brand

Created and maintained by **Rootcastle Engineering & Innovation**.

- Rootcastle: https://rootcastle.com
- Batuhan Ayrıbaş: https://batuhanayribas.com

Core brand colors: `#000000`, `#0E3D8A`, `#228B55`.

## Sources and independence

This project references Apple’s publicly available editorial and design guidance:

- Apple Style Guide: https://help.apple.com/pdf/applestyleguide/en_US/apple-style-guide.pdf
- Apple Human Interface Guidelines: https://developer.apple.com/design/human-interface-guidelines/

The Apple Style Guide PDF is not included in this repository. This is an independent project and is not affiliated with, endorsed by, or sponsored by Apple Inc. Apple and Apple product names are trademarks of Apple Inc.

## License

The original skill instructions and Rootcastle reference material are available under the MIT License. Third-party documentation, trademarks, fonts, icons, and design assets remain subject to their respective owners’ terms.
