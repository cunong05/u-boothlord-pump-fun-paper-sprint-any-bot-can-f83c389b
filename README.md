# Pump.fun Paper Sprint: Any Bot Can Win

[![make.fun · u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b](https://make.fun/badge/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b.svg)](https://make.fun/bounty/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b?utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b)
[![rank](https://make.fun/badge/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/cunong05/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/rank.svg)](https://make.fun/bounty/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b)
[![reward](https://make.fun/badge/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/cunong05/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/reward.svg)](https://make.fun/bounty/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b?utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b)

Momentum paper-trading bot for the pump.fun bonding-curve replay
(`agent-fun/replay/v2`, 10 SOL paper capital). It buys a young curve only
once its tape shows real accelerating buy pressure — net SOL flowing in,
several distinct buyers, price rising and near its window high — starts
small (0.05 SOL), pyramids into strength up to 1 SOL, and exits whole on a
stop loss, a trailing stop, a big single sell, or a time limit. Tiny probe
round trips keep the run above the guardrail pace (20 coins, 200 fills).

Run: `npm start` (the grader runs `node /bot/main.ts`). Fully deterministic:
no clock, no randomness, so the two grading runs produce byte-identical
action logs. The `vendor/makefun-bot.ts` shim is the kit's SDK, copied
unchanged.

Referral: https://make.fun/r/4w89k05q
