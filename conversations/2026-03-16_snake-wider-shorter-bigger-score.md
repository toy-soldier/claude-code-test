# Conversation — 2026-03-16: Snake wider/shorter board, bigger score display

## User
I cannot see the high score. Maybe it's because the screen is too big. So decrease the height and increase the width. And make the score obvious. I cannot see it.

## Claude
Changes to `snake.html`:
- Board resized from 28×28 (560×560px) to 36×20 cols/rows (720×400px) — wider and shorter
- Snake starting position updated to center of new grid (18,10)
- Score bar font increased from 13px to 22px, bold, white color for visibility
- Opened snake.html in browser via PowerShell
