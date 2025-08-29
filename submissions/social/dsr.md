# vApp Submission: DSR

## Verification
```yaml
github_username: "ayoemanise"
discord_id: "911111087494144011"
timestamp: "2025-08-26"
```

---
category: social
github_username: ayoemanise
discord_id: ezie#6699
---

# Proposal Title
Decentralized Social Reputation (DSR) vApp

## Short Description
DSR is a vApp that enables users to build **on-chain social reputation** with privacy preserved through the Soundness Layer.  
Instead of storing the full history of user activities publicly, the system uses zk-proofs to verify social achievements (e.g., community contributions, event participation, or identity verification) **without exposing sensitive data**

## Technical Architecture
- **Frontend**: A simple web app (Next.js/React) where users can log in with their wallet and manage their reputation badges.  
- **Backend**: API service (Node.js/Express) to receive user requests, generate proofs, and relay them to the Soundness Layer.  
- **Proof Generation**:  
  - User action → generates a zk-proof via Soundness CLI.  
  - Proof is submitted to the Soundness Layer for validation.  
- **Storage**: Reputation metadata (badge ID, hashed activity) is stored on IPFS/Arweave, while only proofs are recorded on-chain.  
- **Workflow**:  
  1. User logs in → selects an event/activity to verify  
  2. System generates zk-proof → submits to Soundness Layer  
  3. If valid, user receives a private reputation badge  
  4. Badge can be shared publicly without revealing full activity details  

## Development Timeline
| Phase | Description | Duration |
|-------|-------------|----------|
| 1     | Architecture research & repo setup | 1 week |
| 2     | Proof integration with Soundness Layer (CLI & API) | 2 weeks |
| 3     | Frontend implementation (badge & reputation UI/UX) | 1 week |
| 4     | Storage integration (IPFS/Arweave) + internal testing | 1 week |
| 5     | Review, bug fixing, and finalization | 1 week |
| **Total** |  | **6 weeks** |

## Added Value
- Builds trust in social communities with **proof-based reputation** instead of unverifiable claims.  
- Preserves **user privacy** by storing only proofs, not raw activity data.  
- Extensible to other use cases: DAO voting, event participation proofs, and decentralized identity (DID).  
