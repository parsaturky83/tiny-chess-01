# tiny-chess-01

[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/parsaturky83/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/parsaturky83/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A 4 KB Python chess engine for the [make.fun](https://make.fun/bounty/tiny-chess-01) tiny-chess-01 bounty ($500).

`main.py` (3,957 bytes) is the whole engine: 0x88 mailbox, negamax with
alpha-beta + PVS, quiescence search, transposition table, killer and
history heuristics, tapered evaluation, fixed 50,000-node budget, and a
resignation rule for lost games. Original code, MIT licensed. v5
(2026-11-23) starts late-move reductions one move earlier; re-graded at
Elo 1,654 / 1,654 / 1,191 across the three local trials (mean ~1,499),
above the 1,154 final-qualification bar.

## Grade locally

With the competition dev kit:

```sh
makefun grade-local --kit . --bot <repository> --driver docker
```

## License

MIT — see LICENSE.
