# Changelog

All notable changes to the **Magic Robots TTY** theme.

Format is loosely based on [Keep a Changelog](https://keepachangelog.com/).

## [1.2.0] — Unreleased

### Changed
- Selection colors: red → muted dark green across editor, minimap, and terminal (`selectionBackground`, `inactiveSelectionBackground`).
- Word / hover / occurrence highlights unified in a coherent green family (was blue/teal defaults).
- Find match colors: current match keeps bright green; other matches moved from orange-red to a subtle dim green with a faint outline.
- Diff editor line backgrounds dimmed so selected text within a diff line stays readable.
- Editor cursor changed from red to bright green (`#00ff33`) with a dark-green ink color for block cursors.
- Palette de-yellowed: every color where R > B was shifted so B ≥ R, giving a cleaner green (no mustard cast) that stays readable on macOS displays.
- Interface dimmed: editor foreground, line numbers, sidebar, and status bar foreground all pulled back a step so syntax-highlighted tokens carry the visual weight.
- Editor background changed from `#000000` to `#010603` — a nearly imperceptible green tint that avoids the "hard slab" look of pure black on high-contrast displays.
- Structural borders (panel dividers, notifications, quick picker) unified in a dim green family instead of grays.
- Status bar mirrored to the active tab: same background, foreground, and a matching accent stripe on the editor-facing edge.
- Debug status bar tinted subtle blue (`#001f4d`) so an active debug session is visible without breaking the palette.
- Command palette selected row darkened so match-highlight characters stay readable.

### Fixed
- `markup.deleted.diff` was green (`#219b00`), nearly identical to `markup.inserted.diff`. Deletions now render red — patch/diff view is finally usable.
- `diffEditor.insertedLineBackground` / `removedLineBackground` were unset, so only inline character ranges were tinted. Whole changed lines now tint correctly.
- `diffEditorGutter`, `diffEditorOverview`, and `editorOverviewRuler.{added,modified,deleted}Foreground` were unset — the scrollbar / minimap change indicators now match the diff palette.
- 3-way merge headers had almost no contrast between `current` (gray) and `incoming` (near-black green). Now clearly green / cyan / gray.
- Added `mergeEditor.*` keys used by VS Code's newer merge editor.

## [1.1.0] — 2026-07-27

### Changed
- Forked and rebranded from Functional Matrix as **Magic Robots TTY**.
- Renamed theme file to `magic-robots-tty-color-theme.json`.
- Bumped publisher/author to `magicrobots`; repository points at this fork.

## [1.0.1] and earlier

Upstream **Functional Matrix** by clubcleaver.
See <https://github.com/clubcleaver/functional-matrix> for original history.
