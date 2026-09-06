# W Lotus

Burnable white lotus on [eCash](https://e.cash) — offered in memory of the dead, and as dana to the living.

| | |
|---|---|
| App | https://wlotus.org |
| Explorer | https://danaverse.org |
| Ticker | **WLOTUS** |
| Token id | `a41bf9d03961a2be83f854c8cea0b3fddf7e275ff3695d9848046052d6db3df9` |
| Covenant | **WLotusCovenant** — mint **108** miner, no temple tax |
| Clock | base **0** bits; felt +1 bit / **500** days; cap **128** |

This repository is a **public snapshot** of the reference covenant and the offerings web UI. It is not the full desk (mint-api, deploy, historical experiments stay private). Forks that copy `WLotusCovenant` with the same economics and `genesisUnix` may exchange 1:1 value-wise.

Snapshot from `9b4b0b0` (`9b4b0b04cc2c00dc1e66bfc7b0ec404771c20ff1`).

## Layout

```
contracts/WLotusCovenant.spedn                  # reference remint (forks copy this)
contracts/WlotusPowRemintMooreTipTemple.spedn   # retired 102/6 temple covenant
src/covenant/                                   # TypeScript loaders
src/params/wlotusMint.ts                        # 108 felt / 102/6 temple constants
apps/web/                                       # offerings PWA source (reference)
```

The web tree expects those `src/` paths (same as the private monorepo). It talks to the live desk at wlotus.org; it is not a complete local stack.

## License

MIT — see [LICENSE](./LICENSE).
