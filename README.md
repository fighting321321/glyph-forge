# GlyphForge

**Programmatic font engineering for building consistent Latin and CJK typefaces.**

GlyphForge is an experimental software-engineering project that explores how font design—especially Chinese font design—can be made more scalable through reusable glyph components, explicit style rules, and code-assisted generation.

## Motivation

This project started from a practical problem encountered while making a small game.

For English text, manually creating or importing a custom typeface is still manageable. For Chinese, however, the size of the character set makes fully manual production unrealistic for an individual project. Existing fonts are plentiful, but it is often difficult to find one that precisely matches the visual language of a specific game or interface.

GlyphForge explores a different workflow: instead of treating every Chinese character as an isolated drawing task, represent reusable strokes, radicals, components, geometric constraints, and style parameters in code, then use them to assist glyph construction while keeping human control over the final visual style.

## Core Goals

- Explore reusable representations for Latin and CJK glyph construction.
- Reuse strokes, radicals, components, and structural rules where practical.
- Maintain visual consistency across a large character set.
- Automate repetitive parts of font building, export, and validation.
- Keep the designer in control of style rather than pursuing fully automatic generation.

## Current Status

**Phase 0 — research and architecture exploration.**

The project is intentionally not committed to a single generation strategy yet. Early work should focus on small, testable prototypes and on understanding the font-engineering problem before scaling to large character sets.

## Documentation

- [Vision](docs/VISION.md) — why the project exists and what problem it aims to solve.
- [Roadmap](docs/ROADMAP.md) — proposed development phases.
- [Architecture](docs/ARCHITECTURE.md) — initial technical boundaries and design questions.
- [References](docs/REFERENCES.md) — useful projects, tools, papers, and design references.
- [Decisions](docs/DECISIONS.md) — durable project decisions and their rationale.
- [AGENTS.md](AGENTS.md) — project context and working rules for Codex/AI coding agents.

## License

Source code is released under the [MIT License](LICENSE).

Any font files produced by GlyphForge may use a font-specific license such as the **SIL Open Font License 1.1 (OFL-1.1)**. Font licensing will be decided explicitly before distributable font assets are added.
