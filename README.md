[![Built for make.fun](https://make.fun/brand/mf-badge-built-for.svg)](https://make.fun?ref=rapid-stork-82)
[![Enter this bounty](https://make.fun/brand/mf-badge-enter.svg)](https://make.fun/c/tiny-chess-01?ref=rapid-stork-82)

# tiny-chess-4k

The strongest chess engine that fits in 4 KB of Python: a single-file engine (3,988 bytes, stdlib only) written for the make.fun tiny-chess-01 bounty.

**Play it / try it:** it plays through the make.fun trial env — run `python3 main.py` with `MAKEFUN_ENV_URL`, `MAKEFUN_PROMPT_FILE` and `MAKEFUN_TRIAL_SEED` set the way a trial does; it is not a UCI engine.
**How it works:** negamax alpha-beta with principal-variation search, null-move pruning, late-move reductions, check extensions and a transposition table; quiescence over captures, promotions and check evasions with delta pruning. Evaluation is incremental material plus piece-square tables with a tapered king table, a bishop-pair bonus and a king pawn-shield term. It searches a fixed 70,000-node budget with no wall-clock use, so every move is fully deterministic. main.py is the packed form produced by the kit's `compress` tool (lzma payload + unpacker stub).
**License:** MIT

<sub>Built with an AI agent for [make.fun](https://make.fun?ref=rapid-stork-82) · bounty [tiny-chess-01](https://make.fun/c/tiny-chess-01?ref=rapid-stork-82) · by [@wh2168888-sudo](https://github.com/wh2168888-sudo)</sub>
