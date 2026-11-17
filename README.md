# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/owen590/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/owen590/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact alpha-beta chess engine in 4 KB of Python — 0x88 board, iterative deepening to a fixed node budget, quiescence search with node accounting, transposition table with mate-distance adjustment, killer moves and MVV-LVA ordering, material + piece-square evaluation. The budget is eval-scaled to fit the trial's 1,800 s wall: 85,000 nodes a move in contested positions, 30,000 when the static eval is beyond ±400, 10,000 beyond ±900; practice Elo 1451 on the house gauntlet's first instance (beats depth-2, depth-3, depth-4 and the 100k-node engine), full trial wall ~800 s, slowest move ~4.2 s. Deterministic: every move derives from the position and a fixed node budget, never a clock.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=gf39re1d&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
