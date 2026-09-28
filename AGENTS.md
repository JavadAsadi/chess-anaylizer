# Project handoff

Before implementing or changing application behavior:

1. Read [the application specification](.agents/design-docs/application-specification.md),
   including its acceptance criteria, scope boundaries, and implementation status.
2. Inspect the approved [desktop](.agents/design-docs/ui-example-desktop.png) and
   [mobile](.agents/design-docs/ui-example-mobile.png) previews.
3. Read the [HTML mockup](.agents/design-docs/ui-example.html) for layout and styling.

## How to use these documents

- The specification defines product behavior, architecture, and MVP scope.
- The mockup and screenshots define the approved visual direction. If a static
  example conflicts with specified behavior, implement the specification.
- The mockup is a design artifact. Its sample FEN, scores, depths, continuations,
  disabled controls, and preview labels must not become production behavior.
  Implement the board with Chessground, rules with chess.js, and real analysis
  with Stockfish as specified.
- The specification records the agreed product decisions. Choose routine
  implementation details within that scope and lock compatible dependency
  versions when scaffolding.

## Keeping the handoff useful

- Check the actual repository before assuming a feature is implemented. The
  specification's implementation-status section records the current milestone.
- Validate changes against the relevant acceptance criteria. Add accurate setup,
  run, and test commands to README.md when those commands exist.
- Update the documentation when behavior, scope, or implementation status changes.
  Keep sample previews clearly distinguished from the working application.
