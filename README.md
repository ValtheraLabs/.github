# ValtheraLabs

**Building an AI-native decentralized finance operating system for traders, investors, builders, and institutions.**

---

## 👋 About

ValtheraLabs is a full-stack technology studio at the intersection of **AI, blockchain, and DeFi infrastructure**. We design and ship production-grade systems — from on-chain protocols to the AI services and applications that sit on top of them.

Our flagship project, the **AIU Protocol**, is a Web3 trading platform combining a native utility token, automated market-making via Uniswap V3, on-chain limit/range orders, and an AI-driven dynamic fee engine — with perpetuals trading on the roadmap.

## 🧩 Core Repositories

| Repo | Description | Stack |
|---|---|---|
| [`smart-contracts`](https://github.com/ValtheraLabs/smart-contracts) | On-chain protocol: token, fee engine, oracle, router, range-order manager | Solidity / Foundry |
| [`ai-engine`](https://github.com/ValtheraLabs/ai-engine) | AI fee prediction & off-chain intelligence services | Python |
| [`backend-api`](https://github.com/ValtheraLabs/backend-api) | API layer connecting protocol, oracle, and frontend | Python |
| [`web-app`](https://github.com/ValtheraLabs/web-app) | Frontend dApp for trading, swaps, and order management | TypeScript |

## ⚙️ AIU Protocol — Architecture Snapshot

- **AIUToken.sol** — ERC20 + Permit + Votes, 1B max supply
- **FeeManager.sol** — Static fee tiers (hard-capped at 1%), consults the AI oracle with staleness fallback
- **FeeCollector.sol** — Configurable burn / treasury / staking split
- **AIFeeOracle.sol** — Push-based bounded oracle with ceiling/floor and staleness checks
- **AIURouter.sol** — Uniswap V3 SwapRouter02 wrapper with pre-swap fee collection
- **RangeOrderManager.sol** — Single-sided V3 position limit orders, Chainlink Automation-compatible

**In progress:** off-chain AI fee prediction service, staking contract, and the frontend dApp integration.

## 🛠 Tech Stack

TypeScript · JavaScript · Python · Solidity · Go · Rust · React · Next.js · Node.js · Docker

## 📫 Contact

For collaboration or inquiries, reach out via [ValtheraLabs](https://github.com/ValtheraLabs) or the founder's personal profile [@Trinexxx](https://github.com/Trinexxx).

---

*ValtheraLabs — engineering the AI layer of decentralized finance.*
