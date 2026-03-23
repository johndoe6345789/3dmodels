# Contributing to 3D Print Models

Thank you for your interest in contributing! This guide explains how to add new models or improve existing ones.

## How to Contribute

1. **Fork** the repository and create a new branch for your model.
2. Add your model files under the appropriate category in the `models/` directory.
3. Update the `README.md` table to include your new model.
4. Submit a **Pull Request** with a clear description of the model.

## File Format

All models must be provided as **ASCII STL** files (`.stl`). Binary STL is also acceptable but ASCII is preferred for readability and diff-friendliness.

### Naming Convention

Use lowercase with hyphens for file names:

```
models/<category>/<model-name>.stl
```

Examples:
- `models/home/phone-stand.stl`
- `models/tools/hex-key-holder.stl`
- `models/basic-shapes/torus.stl`

## Categories

| Category | Description |
|----------|-------------|
| `basic-shapes/` | Geometric primitives and simple shapes |
| `home/` | Household items, organizers, clips, holders |
| `tools/` | Practical tools, fixtures, and workshop helpers |

If your model doesn't fit an existing category, propose a new one in your Pull Request.

## Design Guidelines

- Design for **FDM printing** unless otherwise noted.
- Models should be **manifold** (watertight) with no inverted normals.
- Use **millimeters (mm)** as the unit of measurement.
- Default layer height target: **0.2 mm**.
- Avoid unnecessary overhangs exceeding **45°** without support structures.
- Include a short description in a `README.md` within the model's folder if the model has multiple parts or complex print settings.

## Recommended Print Settings

When your model has specific requirements, document them in a comment block at the top of your STL or in a companion `<model-name>.md` file:

```
Material: PETG
Layer Height: 0.15 mm
Infill: 30%
Supports: Yes (touching build plate only)
```

## Code of Conduct

Be respectful and constructive in all interactions. We welcome contributions from all experience levels.
