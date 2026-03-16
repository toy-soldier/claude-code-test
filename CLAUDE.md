# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Running the App

Open `tictactoe.html` directly in a browser, or use the pre-configured command:

```bash
cmd.exe /c start "" "$(pwd)/tictactoe.html"
```

No build step, package manager, or server required.

## Architecture

The entire application is a single self-contained file: `tictactoe.html`.

**Game state** (JS variables): `board` (9-cell array), `current` (active player), `gameOver`, `vsComputer`, `scores`.

**AI**: The computer plays O and uses a recursive minimax algorithm (`minimax()` in the script). It is unbeatable — O win scores +1, X win scores -1, draw scores 0. `bestMove()` iterates all empty cells and picks the highest-scoring move.

**Game flow**: X always moves first. After each human move, `play(index)` checks win/draw, then triggers `computerMove()` (300 ms delay) if in vs-computer mode. Winning cells are highlighted via `highlight(combo)` which adds a CSS class.
