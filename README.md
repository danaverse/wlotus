# W Lotus

Burnable white lotus on [eCash](https://e.cash) — offered in memory of the dead, and as dana to the living.

| | |
|---|---|
| App | https://wlotus.org |
| Explorer | https://danaverse.org |
| Ticker | **WLOTUS** |
| Token id | `f4e452ef78eaf61908d30ecbd804df5588c6bb6aeea61cf0cbe8bf2186764456` |
| Covenant | mint **108** = **102** miner + **6** temple |
| Clock | base **0** bits; +1 bit / **500** days; cap **128** |

This repository is a **public snapshot** of the live covenant and the offerings web UI. It is not the full desk (mint-api, deploy, historical experiments stay private).

Snapshot from `v26.8.6` (`71c0904f90fae9a6b9cd13ab73cbee5182b1d255`).

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
