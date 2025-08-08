
# Himnet: The Human-in-the-Middle Network

**Version:** 0.1 (Spec Draft)  
**Date:** August 2025  
**License:** CC BY 4.0

---

## Abstract

Himnet is an open protocol and decentralized marketplace for human-in-the-loop (HITL) tasks. It enables anyone in the world to earn a native currency by completing verifiable, dispute-resolvable tasks that require human judgment. Through sealed-bid auctions, escrowed payouts, juror-based arbitration, and soulbound reputation, Himnet builds a fair, trustless ecosystem for labor, collaboration, and computation.

---

## 1. Introduction

Large-scale AI systems, automation, and global connectivity have increased demand for human-in-the-loop work. However, today's systems—like Amazon Mechanical Turk—are centralized, opaque, exploitative, and closed-source. Himnet reimagines this model as a public good: permissionless, decentralized, and governed by its users.

Himnet is built for:
- Task requesters: who need subjective or human-sensitive results  
- Workers: who want to earn by doing valuable human work  
- Jurors: who verify, audit, and resolve disputes

---

## 2. Core Components

### 2.1 Task Registry
On-chain task creation with:
- IPFS-hosted specs and input files  
- Token escrow  
- Acceptance criteria  
- Auction rules and deadlines  

### 2.2 Bidding Engine
- Reverse sealed-bid auctions (commit-reveal)  
- Winner gets paid the second-lowest bid (Vickrey style)  
- Anti-sniping mechanisms built-in  

### 2.3 Submission & Verification
- Workers upload results to IPFS  
- Protocol verifies submission or routes to dispute system  

### 2.4 Dispute Resolution
- Jurors selected randomly (VRF)  
- Commit–reveal voting  
- Slashing dishonest jurors  
- Split payouts: e.g., 80% on acceptance, 20% after audit window  

### 2.5 Reputation
- Soulbound NFT (SBT) score based on accepted work and accurate voting  
- Reputation caps task frequency and priority  

---

## 3. Token Economics

### Native Token: HUM
- Earned via work and verified voting  
- Used for task escrow, juror staking, dispute fees  

### Incentives
- Workers earn HUM from tasks  
- Jurors earn dispute resolution fees  
- Relayers (optional) earn small routing fees  

---

## 4. Anti-Collusion

Himnet enforces fairness through:
- Random juror selection after task submission  
- High staking + slashing risk  
- Commit–reveal vote security  
- Sampling audits for fraud detection  
- Multi-party verification  

---

## 5. Architecture

| Layer      | Technology                         |
|------------|-------------------------------------|
| Chain      | EVM-compatible L2 (Base, Arbitrum, OP) |
| Storage    | IPFS / Arweave                     |
| Identity   | Wallet-based, optional uniqueness proofs |
| Indexing   | The Graph or custom indexers       |
| Relayers   | libp2p (optional), Matrix for discovery |

---

## 6. Governance

- DAO-controlled parameters  
- Timelocked guardian role (early phase only)  
- Protocol Improvement Proposals (HIPs)

---

## 7. Roadmap

| Phase    | Goals                                         |
|----------|-----------------------------------------------|
| Phase 0  | Spec & Whitepaper, repo setup                 |
| Phase 1  | Testnet MVP, smart contracts, basic clients   |
| Phase 2  | Dispute engine, audits, juror pool scaling    |
| Phase 3  | DAO onboarding, grants, BTC bridge support    |

---

## 8. Conclusion

Himnet creates a permissionless work economy built on fairness, openness, and decentralization. It empowers humans to perform trust-critical tasks for machines, orgs, and each other—earning a sovereign currency in return. The long-term vision is a fully decentralized labor network secured not by trust, but by design.

---

## Appendix A: License

- Protocol & Contracts: AGPL-3.0  
- Documentation: CC BY 4.0  

---

## Appendix B: Name

**Himnet** stands for **Human-in-the-Middle Network** — where humans are not a bottleneck, but a bridge.
