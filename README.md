# 🏆 FIDE World Chess Championship 2026 — Home Assistant Card

A zero-dependency Home Assistant dashboard card that streams live moves, evaluation bar, last-move highlights, and game history for the 2026 FIDE World Chess Championship from Lichess.

## Features
- Chess.com-style Green & Cream board with crisp vector pieces
- Live evaluation bar (automatically locks to 0.0 on draws)
- Full move navigation (First, Previous, Next, Live/Last)
- Game selector dropdown (Game 1, Game 2, Game 3, etc.)
- Zero backend, Docker containers, or YAML sensors needed

## Installation
Via HACS:
1. Open HACS -> three dots (⋮) -> Custom repositories.
2. Paste this repository URL, pick Dashboard, and click Add.
3. Search for WCC 2026 Board Card -> Download -> Reload.

Manual:
1. Save wcc-board-card.js to /config/www/wcc-board-card.js.
2. Go to Settings -> Dashboards -> three dots (⋮) -> Resources -> Add Resource.
3. Set URL to /local/wcc-board-card.js?v=1 and type to JavaScript Module.

## Card YAML
type: custom:wcc-board-card
tournament_id: qfkdt8mn
refresh_seconds: 30
