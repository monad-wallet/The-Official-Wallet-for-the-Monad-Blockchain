# Monad Wallet  
Official non-custodial wallet for the Monad blockchain

[![EVM Compatible](https://img.shields.io/badge/EVM-Compatible-blue)]()

---

## Overview

[Monad wallet](https://mymonad.xyz) is the official wallet for interacting with the Monad Layer-1 blockchain.  
It provides a secure, high-performance interface for managing assets, connecting to dApps, and participating in the Monad ecosystem.

Monad is a high-throughput, EVM-compatible blockchain designed for scalability and low-latency execution. Monad Wallet enables safe and efficient access to all core network features.

---

## Features

### Security
- Fully non-custodial architecture  
- Local key encryption  
- Secure signing and isolated execution  
- Support for hardware wallets (Ledger integration planned)

### Performance
- Optimized for Monad’s low-latency transaction lifecycle  
- Fast account operations and RPC handling  
- Efficient transaction simulation

### Asset Support
- Native MON token  
- ERC-20 fungible tokens  
- ERC-721 and ERC-1155 digital assets

Applications can interface with Monad using standard EVM tooling.

### Staking and Governance

- Stake MON
- Delegate to validators
- View rewards
- Participate in governance proposals

### ⚙️ Usage
Link: [MONAD Web3 Wallet](https://mymonad.xyz)

#### Create a New Wallet
1. Install Monad Wallet
2. Click Create Wallet
3. Write down your 12/24-word recovery phrase
4. Set a password

### Import an Existing Wallet

Supports:

* Recovery phrase (BIP-39)
* Private key
* JSON keystore

### Send & Receive MON

1. Open the Assets tab
2. Select MON
3. Enter recipient address
4. Adjust gas (optional — Monad fees are extremely low)
5. Confirm

### Cross-Platform Availability

- Browser extension (Chrome, Firefox, Brave)
- Mobile applications (iOS, Android)
- Desktop application (macOS, Windows, Linux)

### 🛠️ Developer Guide
Add Monad to a Web3 App

```js
await provider.request({
  method: "wallet_addEthereumChain",
  params: [{
    chainId: "0xMON", 
    chainName: "Monad Mainnet",
    rpcUrls: ["https://rpc.monad.xyz"],
    nativeCurrency: { name: "Monad", symbol: "MON", decimals: 18 },
    blockExplorerUrls: ["https://explorer.monad.xyz"]
  }]
});




