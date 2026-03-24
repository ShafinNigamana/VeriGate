# 🛡️ VeriGate

<p align="center">
  <strong>The Decentralized Web3 Access Protocol</strong><br>
  <em>Earn access through proof. Complete challenges, mint your credential, and unlock exclusive on-chain content.</em>
</p>

## 📖 Introduction
Traditional gatekeeping relies on centralized databases and paywalls. VeriGate transforms this paradigm by introducing **proof-of-knowledge access control**. Users don't just log in; they prove their understanding of Web3 concepts to earn an on-chain NFT credential, which seamlessly unlocks premium decentralized applications.

## 🚨 The Problem
- **Meaningless Access Models:** Current Web3 access often relies purely on capital (buying NFTs/tokens).
- **Lack of Education:** Users interact with protocols they don't understand, leading to loss of funds and poor security practices.
- **Static User Experiences:** Many dApps feel lifeless, mimicking traditional Web2 forms rather than embracing dynamic, interactive paradigms.

## 💡 The Solution
VeriGate combines interactive education with on-chain credentials:
1. **Learn & Prove:** Users complete an interactive, anti-cheat challenge.
2. **Earn Credential:** Successful users mint a non-transferable `VeriGate NFT`.
3. **Unlock Value:** The protocol verifies ownership and grants access to premium, gated content.

## 🎯 Objectives
- Implement a **secure, client-side challenge protocol** using cryptographic hashing (SHA-256) to prevent tampering.
- Create a **premium, glassmorphism-driven UI/UX** that feels highly interactive, replacing standard forms with reactive panels.
- Frictionlessly **integrate smart contract interactions** (minting, balance checks) via Ethers.js and Wagmi.

## 🏗️ Architecture
- **Frontend Framework:** Next.js 14 (App Router) + React
- **Styling:** Tailwind CSS + Custom Animations & Glassmorphism Utilities
- **Web3 Integration:** Wagmi (Wallet Connection) + Ethers.js (Contract Interaction)
- **Smart Contract:** Custom ERC-721 Stylus Contract deployed on Arbitrum Sepolia
- **Security:** In-browser cryptographic hashing (`ethers.keccak256`) for anti-cheat quiz evaluation.

## 🚀 Step-by-Step Setup Guide

### 1. Requirements
- Node.js (v18+)
- pnpm (recommended) or npm
- MetaMask or another injected Web3 wallet

### 2. Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/ShafinNigamana/VeriGate.git
cd VeriGate
pnpm install
```

### 3. Environment Configuration
Navigate to the web app directory and create an environment file:
```bash
cd apps/web
cp .env.example .env
```
Ensure your `apps/web/.env` contains the required variable for your contract:
```env
NEXT_PUBLIC_CONTRACT_ADDRESS=0xe2a8cd01354ecc63a8341a849e9b89f14ff9f08f
```

### 4. Running the Development Server
Start the Next.js development server:
```bash
npm run dev
# or pnpm dev
```
Open **http://localhost:3000** in your browser.

## 🏁 Conclusion
VeriGate sets a new standard for Web3 onboarding. By demanding proof-of-knowledge instead of mere capital, it fosters an educated, engaged community while utilizing Arbitrum's high-performance rollups to ensure minting and verification are fast and securely scaled.
