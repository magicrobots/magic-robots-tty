# Magic Robots TTY

A dark, monochromatic green VS Code theme built for **long reading sessions and honest diffs**.

Fork of [Functional Matrix](https://github.com/clubcleaver/functional-matrix) by clubcleaver, rebalanced for daily driving on large codebases: readable diff/merge contrast, de-yellowed greens, and a quiet interface that gets out of the way of the code.

---

## Why this fork exists

The original Functional Matrix nailed the aesthetic but made a few colors that mattered for real work indistinguishable — most notably, **inserted and deleted lines in diffs were both green**, so PR review was a guessing game. This fork keeps the monochrome-green spirit and fixes the parts that got in the way of using it.

## What's different from Functional Matrix

- **Readable diffs.** Deletions are red, insertions are green, full-line backgrounds are set (not just inline character ranges), and the change gutter, minimap, and scrollbar overview ruler all agree.
- **Readable 3-way merges.** `current` / `incoming` / `common` are green / cyan / gray instead of near-identical shades, and the newer `mergeEditor.*` keys are set for VS Code's built-in merge editor.
- **De-yellowed palette.** Every color that leaned yellow has been shifted so blue ≥ red — brighter tokens read as green or off-white, never mustard.
- **Softer interface, louder code.** Sidebar, status bar, breadcrumbs, and line numbers were dimmed a step; the editor foreground is what your eye lands on first.
- **Symmetric top/bottom accents.** The active editor tab and the status bar share a common accent color and highlight stripe, sandwiching the editor.
- **Subtle green background.** `#010603` instead of pure black — reads better on macOS displays that render pure `#000000` as a hard black slab.
- **Green selection.** No more red text selection. Selection, find highlights, word occurrences, and hover highlights all live in a coherent muted-green family.
- **Green block cursor by default.** Set `"editor.cursorStyle": "block"` in your user settings to enable the block style — the theme colors the cursor bright green either way.

## Install

From the Marketplace (once published):

1. Open Extensions, search for **Magic Robots TTY**, click **Install**.
2. `Cmd+K Cmd+T` (or `Ctrl+K Ctrl+T`) → select **Magic Robots TTY**.

From a `.vsix`:

```bash
code --install-extension magic-robots-tty-<version>.vsix
```

## Recommended companion settings

```jsonc
{
  "editor.cursorStyle": "block",
  "editor.cursorBlinking": "solid",
  "editor.renderWhitespace": "boundary",
  "editor.bracketPairColorization.enabled": true,
  "workbench.colorTheme": "Magic Robots TTY"
}
```

## Feedback

Issues and PRs welcome at [github.com/magicrobots/magic-robots-tty](https://github.com/magicrobots/magic-robots-tty/issues).

## Credits

Based on **[Functional Matrix](https://github.com/clubcleaver/functional-matrix)** by clubcleaver. Released under the same MIT license (see [LICENSE](./LICENSE)).
