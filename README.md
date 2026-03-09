# ⬡ ERC-20 Staking Contract

Production-ready ERC-20 staking contract with real-time reward accrual, configurable lock periods, and emergency controls. Deployed on Base.

[![Solidity](https://img.shields.io/badge/Solidity-^0.8.20-363636?style=flat-square&logo=solidity)](.)
[![Hardhat](https://img.shields.io/badge/Built_with-Hardhat-F7DF1E?style=flat-square)](.)
[![License](https://img.shields.io/badge/License-MIT-7c3aed?style=flat-square)](.)

---

## Features

- **Flexible staking** — configurable APY and lock period
- **Real-time rewards** — accrues per second, claimable anytime
- **Emergency controls** — pause mechanism + emergency withdraw
- **Gas optimized** — struct packing, cached storage reads
- **Battle-tested** — full branch coverage with Hardhat tests

## Tech Stack

- Solidity 0.8.20 · Hardhat · OpenZeppelin · Base Mainnet

## Contract Architecture

```
StakingContract
├── stake(uint256 amount)
├── unstake(uint256 amount)
├── claimReward()
├── pendingReward(address user) → view
├── emergencyWithdraw()
└── Admin: setAPY, pause, unpause
```

## Security

- ReentrancyGuard on all state-changing functions
- Pausable for emergency stops
- AccessControl for admin functions
- 100% branch test coverage

---

**Need a staking contract built?**
→ [t.me/oxbobdev](https://t.me/oxbobdev) · [0xbob.vercel.app](https://0xbob.vercel.app)
