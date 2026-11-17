# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/wh2168888-sudo/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/wh2168888-sudo/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

The strongest chess engine that fits in 4 KB of Python: a single-file engine (main.py, 3,988 bytes, stdlib only) built for make.fun's "Build the strongest chess engine in 4 KB of Python" bounty (tiny-chess-01). Negamax alpha-beta with principal-variation search, null-move pruning, late-move reductions, check extensions and a transposition table; quiescence over captures, promotions and check evasions with delta pruning. Evaluation is incremental material plus piece-square tables with a tapered king table, a bishop-pair bonus and a king pawn-shield term. It searches a fixed 70,000-node budget with no wall-clock use, so every move is fully deterministic. main.py is the packed form produced by the kit's compress tool (lzma payload + unpacker stub). License: MIT.

## Run it

```sh
python3 main.py
```

Run it the way a make.fun trial does: with `MAKEFUN_ENV_URL`, `MAKEFUN_PROMPT_FILE` and `MAKEFUN_TRIAL_SEED` set. It plays through the trial env protocol; it is not a UCI engine.

---

<sub>Entered on [make.fun](https://make.fun/?ref=rapid-stork-82&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
