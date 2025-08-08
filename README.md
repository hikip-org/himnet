# Himnet

**The Human-in-the-Middle Network**  
A decentralized protocol for human-in-the-loop work, fair labor markets, and crypto-native trust.

---

## 🌐 What is Himnet?

Himnet is a decentralized, open-source protocol where anyone can:
- **Post tasks** that require human judgment or subjective evaluation.
- **Earn a native token** (`HUM`) by completing tasks or serving as a juror.
- **Trust the results** through sealed-bid auctions, on-chain escrow, random juror arbitration, and non-transferable reputation.

Think: *Bitcoin + Mechanical Turk + Aragon Court*, reimagined as a public good.

---

## 🧱 Core Modules

- **Task Registry:** On-chain metadata + IPFS content addressing
- **Bidding Engine:** Reverse Vickrey auctions via commit–reveal
- **Escrow + Disputes:** Smart contract-secured payout system with juror-based arbitration
- **Juror Pool:** Random, staked participants selected via verifiable randomness (VRF)
- **Reputation System:** Soulbound NFT for worker/juror scores and unlocks
- **Token (`HUM`):** Native ERC-20 token for work, dispute fees, and staking

---

## 🔒 Anti-Collusion

Himnet prevents fraud and collusion with:
- Commit–reveal voting + bidding
- Random juror selection post-submission
- Slashing dishonest jurors
- Sampling audits of accepted work
- Split payout system (e.g., 80% on accept, 20% post-audit)

---

## 🪙 Token Use

- `HUM` is earned by:
  - Completing tasks (workers)
  - Resolving disputes (jurors)
- `HUM` is used for:
  - Funding task escrows
  - Staking for bidding / voting
  - Paying protocol fees
- Optional: accept BTC payments via bridge or manual swap

---

## 🧭 Roadmap

| Phase     | Goal                                       |
|-----------|--------------------------------------------|
| Phase 0   | Whitepaper + spec + repo scaffolding       |
| Phase 1   | Testnet MVP + basic smart contracts        |
| Phase 2   | Dispute engine, juror scaling, audits      |
| Phase 3   | DAO onboarding + grant programs + BTC bridge |

---

## 🛠 Tech Stack

| Layer      | Tooling                                |
|------------|-----------------------------------------|
| Chain      | EVM L2 (e.g., Base, Arbitrum, Optimism) |
| Storage    | IPFS / Arweave                          |
| Identity   | Wallet-based, optional uniqueness       |
| Indexing   | The Graph or custom subgraph            |
| Messaging  | libp2p, Matrix (optional)               |
| Clients    | Next.js (requester), RN (worker), CLI   |

---

## 📄 License

- **Code:** [AGPL-3.0](https://www.gnu.org/licenses/agpl-3.0.html)
- **Documentation:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

---

## 👥 Get Involved

We’re looking for:
- Solidity developers (contracts, auctions, dispute logic)
- Frontend/mobile contributors (Next.js, React Native)
- p2p engineers (relayers, nodes)
- Governance & cryptoeconomics researchers

See [`project-info.md`](./project-info.md) and [`whitepaper.md`](./whitepaper.md) to learn more.

---

> **Himnet** stands for **Human-in-the-Middle Network** — where humans aren't the bottleneck, they're the bridge.

