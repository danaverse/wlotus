# W Lotus

Burnable white lotus on [eCash](https://e.cash) — offered in memory of the dead, and as dana to the living.

| | |
|---|---|
| App | https://wlotus.org |
| Explorer | https://danaverse.org |
| Ticker | **WLOTUS** |
| Token id | `154d229bab3cf228a2d40b507e1fc5f21a09542ec66776d3e797b455ab77a091` |
| Covenant | mint **108** = **102** miner + **6** temple |
| Clock | base **0** bits; +1 bit / **500** days; cap **128** |

This repository is a **public snapshot** of the live covenant and the offerings web UI. It is not the full desk (mint-api, deploy, historical experiments stay private).

Snapshot from `d9d05d5` (`d9d05d503e4c67ae9bee9d156fbeee9c48825276`).

## Layout

```
contracts/WlotusPowRemintMooreTipTemple.spedn   # on-chain covenant
src/covenant/                                   # TypeScript loaders for that covenant
src/params/wlotusMint.ts                        # 102 / 6 / 108
apps/web/                                       # offerings PWA source (reference)
```

The web tree expects those `src/` paths (same as the private monorepo). It talks to the live desk at wlotus.org; it is not a complete local stack.

## License

MIT — see [LICENSE](./LICENSE).
