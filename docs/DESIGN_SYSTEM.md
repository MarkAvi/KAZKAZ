# Design System

The app interface should feel like an operational logistics command center.

## Direction

- Dark command-center surface.
- Dense but readable operational panels.
- Strong status visibility.
- Clear mode separation: auto, air, rail, multimodal.
- Tables and operation rows for repeat workflows.
- Minimal decoration.

## Current UI Sources

Design references live in:

```txt
stitch_design_system_blueprint/
```

Important references:

- `command_center_logistics/DESIGN.md`
- `rfq_ru_en/`
- `kaztranscargo_ru_en/`
- `ru_en_1/` through `ru_en_5/`

## Component Patterns

Use existing components before creating new ones:

- `PageShell`
- `MetricGrid`
- `StatusBadge`
- `OperationsList`
- `ModeCoverage`
- logistics workflow boards

## CSS Patterns

Current app-level visual utilities include:

- `glass-panel`
- `command-panel`
- `metric-card`
- `operation-row`
- `data-value`
- `mode-tile`
- `route-radar`
- `command-strip`

## UX Rules

- Keep dashboards operational, not promotional.
- Do not expose internal finance data on customer screens.
- Prefer real workflow controls over explanatory text.
- Keep text compact enough for Russian and English UI.
- Avoid large decorative landing-page sections inside `/app`.
