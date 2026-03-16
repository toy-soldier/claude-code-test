# Conversation — 2026-03-16: Snake background blue & bigger board

## User
So tell me what do you know about this repository?

## Claude
Based on the CLAUDE.md and git history, this repository contains two browser-based games:

1. **Tic-Tac-Toe** (`tictactoe.html`) — A single-file app with an unbeatable AI using the minimax algorithm. X always goes first, computer plays O. Has vs-computer and vs-human modes with score tracking.
2. **Snake** (`snake.html`) — A Nokia-style Snake game, added more recently. The snake was made slower and the board bigger for easier gameplay.

Both are self-contained HTML files — no build tools, no server, no dependencies. Just open in a browser.

---

## User
For the snake game can you make the background blue? And board even bigger.

## Claude
Made the following changes to `snake.html`:
- **Background**: page background changed from dark grey (`#1a1a1a`) to blue (`#1a3a6e`)
- **Board**: increased from 20×20 cells (360px) to 28×28 cells (560px), with slightly larger cells (18→20px)
- Snake starts at center of the new grid (14,14)

---

## User
Did you push this to GitHub?

## Claude
No, I didn't — and I should have. Also noted that the conversation export should be included in the same commit per saved feedback memory.

---

## User
What I want you to do is whenever you make changes to code, you push the conversation export to GitHub.

## Claude
Understood. Writing conversation export and pushing now.
