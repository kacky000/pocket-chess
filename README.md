# pocket-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/kacky000/pocket-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/kacky000/pocket-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in under 4,096 bytes of Python. `main.py` is the whole engine,
packed with `makefun compress`: a 10x12 mailbox board that is flipped after
every move, an exact move generator (perft-checked), principal variation
search with a transposition table, null move, late move reductions and a
capture search, and piece-square evaluation. It searches a fixed number of
nodes per move and never reads a clock, so the same game always plays the
same moves.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 -P -s main.py
```

It plays every game the env at `MAKEFUN_ENV_URL` serves and exits when all are over.

---

<sub>Entered on [make.fun](https://make.fun/?ref=9ykrm1qx&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
