# Conversation — 2026-03-16: Snake persistent high score

## User
Can you keep track of the score? Like, how many pellets that I was able to eat. Then open the new version in the browser so I can play.

## Claude
The game already showed score and high score on screen, but the high score reset on every page refresh. Added `localStorage` persistence so the high score is saved across sessions. The score (pellets eaten) was already tracked per game.

Changes to `snake.html`:
- Load high score from `localStorage` on page load
- Save to `localStorage` whenever a new high score is set

Then opened snake.html in the browser via PowerShell.
