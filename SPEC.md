# MyWebGames — Project Spec

## Overview
A collection of classic browser-based games, each built as a **single self-contained HTML file** with no external dependencies. All games share a consistent dark theme and are opened directly in a browser (`open <file>.html`).

## Design Constraints
- One file per game — HTML, CSS, and JS all inline
- No build step, no frameworks, no CDN links
- Self-contained: works offline, no server needed
- Consistent visual theme: dark background (`#1a1a2e`), gold accents (`#e2b96f`), `Segoe UI` font

---

## Games

### 1. 15 Puzzle (`15puzzle.html`)
Classic sliding tile puzzle on a 4×4 grid.

**Features:**
- 15 numbered tiles + 1 empty space
- Click adjacent tiles or use **arrow keys** to slide
- Move counter and timer (start on first move)
- Shuffle button (always generates a solvable board via inversion parity check)
- Reset button (returns to solved state)
- Win screen overlay showing moves and time

---

### 2. Tic Tac Toe (`tictactoe.html`)
3×3 Tic Tac Toe with two modes.

**Features:**
- **2 Players** mode (same device, take turns)
- **vs Computer** mode (unbeatable minimax AI)
- Score tracking across games (X / Tie / O), persists until Reset Scores
- Win line highlighted in green with pop-in animation
- New Game and Reset Scores buttons

---

### 3. Checkers (`checkers.html`)
Standard 8×8 American Checkers.

**Features:**
- **2 Players** mode or **vs Computer** mode
- Full standard rules: forced captures, multi-jump chains, king promotion (♛)
- Minimax AI with alpha-beta pruning (depth 5) — plays Black
- Click a piece to select; valid destinations highlighted with a gold dot
- Last move highlighted on the board
- Live piece counts for each side
- "Thinking…" overlay during AI computation
- Win detected when a player has no legal moves

---

## Repository
- **GitHub:** https://github.com/5k/MyWebGames
- **Branch:** `main`
- **Policy:** commit and push after every new game or significant change so git history serves as a rollback mechanism

## Upcoming / Ideas
_(add future game requests here)_
