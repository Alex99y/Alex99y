### Hey, I'm Alexander 👋

I like taking stuff apart to see how it works. Most of my side projects start as "wait, how does that actually work?" — usually something about exchanges, wallets, or crypto in general.

By day I'm a backend engineer, 6+ years in, mostly working with blockchain and crypto exchanges. Outside of that I'm into Bitcoin, markets, and reading about finance for fun.

🔭 Right now I'm learning **GCP** and finishing up `matching-engine` below. Getting a lot better at Go and picking up more DevOps along the way.

---

### Stuff I'm building

**[matching-engine](https://github.com/Alex99y/matching-engine)**
I wanted to understand how exchanges actually match orders, so I built one from scratch — no crypto stuff here, just the core matching logic. The DB is the source of truth, it handles about ~2000 ops per market, and it's built to survive crashes and retry properly instead of just breaking. Still a work in progress (tests and Grafana are next), but the core already works well: has its own SDK, a test web app, small bots for liquidity, and a REST API.
`Go` · `Fiber v3` · `TypeScript` · `NodeJS` · `RabbitMQ` · `PostgreSQL`

**[deposit-collector](https://github.com/Alex99y/deposit-collector)**
Basically a deposit/withdrawal module you can plug into an existing system. Each user gets their own address, deposits get tracked, and balances are kept in a DB until they want to withdraw. Works with Bitcoin and EVM chains right now, Solana and ERC-20 withdrawals are still in the works.
`Go` · `PostgreSQL` · `RabbitMQ`

**Smaller stuff**
- [ledger-p2wpkh](https://github.com/Alex99y/ledger-p2wpkh) — signs P2WPKH (bech32) Bitcoin transactions using a Ledger wallet
- [duplicate-files](https://github.com/Alex99y/duplicate-files) — a CLI that finds duplicate files in a folder, digs into subfolders too
- [go-list](https://github.com/Alex99y/go-list) — a simple generic list in Go
- [go-sudoku](https://github.com/Alex99y/go-sudoku) — solves Sudoku with plain old brute-force backtracking
