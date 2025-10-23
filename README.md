---
title: 'DanaBersama - Blockchain Crowdfunding DApp'
description: 'A simple, transparent crowdfunding platform built on XX Blockchain.'
---

# 🫱 DanaBersama

**DanaBersama** is a blockchain-based crowdfunding platform that makes donations transparent and traceable.  
Anyone can create a campaign, donate directly on-chain, and see total donations update in real time.

---

## 🚀 Overview

DanaBersama helps creators and communities raise funds for projects they care about.  
Each campaign includes a goal, deadline, and target address.  
Every donation is recorded on the blockchain, making the process fair and verifiable for everyone.

**Features:**

- Create and manage campaigns
- On-chain donation tracking
- Real-time total display
- Secure withdrawal for campaign owners
- Public donation history

---

## 🧩 Smart Contract Structure

| Variable        | Type      | Description                         |
| --------------- | --------- | ----------------------------------- |
| `campaignCount` | `uint`    | Total number of campaigns           |
| `campaigns[id]` | `mapping` | Stores each campaign’s details      |
| `donations[id]` | `mapping` | List of donations for each campaign |

### Functions

- `createCampaign(goal, deadline)`
- `donate(campaignId)` – payable
- `getCampaign(campaignId)` – view
- `getDonations(campaignId)` – view
- `withdraw(campaignId)`
- `cancelCampaign(campaignId)`

### Events

- `CampaignCreated`
- `DonationReceived`
- `Withdrawn`
- `CampaignCancelled`

---

## 🧠 Development Plan

1. **Smart Contract**

   - Define state variables and mappings for campaigns and donations.
   - Implement logic for creating, donating, and withdrawing.

2. **Security**

   - Add access control, reentrancy guard, and safe math checks.
   - Write unit tests for edge cases.

3. **Frontend**

   - Build with React + Web3 provider.
   - Components: Campaign list, details, donation modal, and wallet connect.

4. **Integration**

   - Connect contract events to frontend state.
   - Display live total donations.

5. **Deployment**
   - Deploy contract to **XX Testnet**.
   - Host frontend on **Vercel** or **Cloudflare Pages**.

---
