# ⚡ **Dravik — Decentralized Digital Asset & Licensing Engine (Built on Story Protocol)**

### **A full-cycle IPFi forge for registering, fingerprinting, licensing & monetizing digital assets using Story Protocol.**

Dravik allows creators to upload any digital file, verify originality, store it on IPFS, register it as on-chain IP, optionally link it with **PizzaDAO IP**, license it to buyers, and earn revenue — all inside a beautiful, fast, full-stack application.

Built from scratch with:

* **React + Tailwind (Frontend)**
* **Node.js + Express (Backend)**
* **Pinata IPFS**
* **Story Protocol SDK**
* **SQLite DB**
* **Dynamic wallet authentication**
* **BAV — Blockchain Asset Verification Layer**

---

# 🔥 **1. Overview**

Dravik is a next-generation IPFi engine that empowers creators to:

* Register digital assets on-chain
* Prove ownership via hashing + BAV
* Store content on IPFS
* License IP using Story Protocol
* Claim revenue from a unified dashboard
* Sync assets with Story Explorer
* Optionally attach **PizzaDAO IP metadata**

Perfect for:

✔ Solo creators
✔ Indie devs
✔ Musicians, artists, filmmakers
✔ AI model / dataset publishers
✔ Web3 IP entrepreneurs

---

# 🧩 **2. Key Components**

## 🔹 A. Asset Registration Engine

* SHA-256 fingerprinting
* BAV verification
* Optional **PizzaDAO IP attach**
* Story Protocol IP registration
* IPFS pinning
* Returns: **IP ID**, metadata, proofs

## 🔹 B. Licensing Marketplace

Creators can:

* List assets
* Set license price
* Define custom license-terms JSON

Buyers can:

* Browse marketplace
* Purchase licenses in SEP ETH
* View license metadata

## 🔹 C. Revenue & Claims Center

* Integrated WIP model (Story Protocol)
* Track royalties
* Claim withdrawable revenue
* Clear UI for income history

## 🔹 D. Secure Backend Layer

* JWT login + wallet pairing
* SQLite database
* IPFS + Pinata integration
* Asset hashing + originality logging

## 🔹 E. Clean UI Dashboards

* Asset Library
* IPFi Dashboard
* Marketplace
* Claims & Revenue
* License Viewer
* Story Explorer sync panel

---

# 🔥 **NEW — 3. BAV: Blockchain Asset Verification Layer**

*(Brand new section you requested)*

Dravik includes a lightweight BAV system:

### **BAV Responsibilities**

✔ Stores SHA-256 hash
✔ Verifies asset hasn't been tampered
✔ Prevents duplicate uploads
✔ Matches hash against database + Story chain data
✔ Tracks proof history

### **BAV Flow**

1. User uploads a file
2. System generates SHA-256 fingerprint
3. BAV checks:

   * Hash exists?
   * Linked with Story IP ID?
   * Any similar assets (future AI feature)?
4. If unique → continue to register

---

# 🛣️ **4. End-to-End User Journey**

## **Creator Flow**

1. Signup / Login
2. Go to **Registration Form**
3. Upload file
4. BAV verifies hash
5. IPFS upload
6. Register on Story Protocol
7. (Optional) Attach **PizzaDAO IP metadata 🍕**
8. List in marketplace
9. Earn revenue + claim monthly

## **Buyer Flow**

1. Login
2. Browse **Marketplace**
3. Buy license (SEP ETH)
4. Backend registers license on-chain
5. Buyer Access asset + metadata
6. View license on chain + Story Explorer


# 🔥 **UNIQUE ADDITION — Optional PizzaDAO Integration 🍕**

During asset registration, the creator can toggle:

> **“Attach PizzaDAO IP metadata?”**
> ✔ If enabled → Pizza DAO’s CC0-style metadata + PNG logo is injected into the asset metadata.

Use cases:
🍕 Community-backed IP
🍕 PizzaDAO derivative collections
🍕 Fun branding on Story Explorer

This makes every registered asset optionally part of a playful Creative Commons movement.

---

# 🚀 **5. Why Dravik? — Value Proposition**

### 🧾 Verified Ownership

Hashing + BAV + Story Protocol = tamper-proof provenance.

### 🌐 Decentralized Storage

All assets stored permanently via IPFS.

### 🧩 Rich IP Metadata

Custom terms + PizzaDAO IP + Fingerprints.

### 🔗 Built Natively on Story Protocol

Everything syncs with Story Explorer.


# 🏗️ **6. System Architecture**

```
                       +----------------------+
                       |  React Frontend UI   |
                       +----------+-----------+
                                  |
                                  v
                      +-----------------------+
                      |  Node.js Backend      |
                      |  - BAV Layer          |
                      |  - IPFS Upload        |
                      |  - Story SDK          |
                      |  - License Engine     |
                      +----------+------------+
                                 |
                                 v
             +-------------------------------------------+
             |          Story Protocol Network           |
             |    - IP Registration                      |
             |    - License Tokens                       |
             |    - WIP Revenue                          |
             +-------------------------------------------+
                 +---------------------------+
                 |        Pinata IPFS       |
                 +---------------------------+
```
---

# ⚙️ **7. Tech Stack**

### **Frontend**

* React
* TypeScript
* Tailwind CSS
* React Router
* Axios
* Wallet-based auth

### **Backend**

* Node.js
* Express
* TypeScript
* SQLite
* Multer
* Pinata SDK
* Story Protocol TypeScript SDK
* JWT Auth

### **Blockchain**

* Story Protocol (Sepolia testnet)
* IP registration
* License minting
* Revenue accounting

---

# 📁 **8. Repository Structure**

```
/
│── README.md                      <-- Main project documentation
│
├── backend/                       <-- Backend + Story SDK scripts
│   ├── src/
│   │   ├── server.ts              <-- Express server & all API routes
│   │   ├── story/                 <-- Story protocol workflows
│   │   ├── pinata/                <-- IPFS utilities
│   │   ├── db/                    <-- SQLite helpers
│   │   └── auth/                  <-- JWT login / signup
│   ├── public/
│   └── README.md                  <-- Full backend documentation
│
└── sp-frontend/                   <-- React + TypeScript + Tailwind
    ├── src/
    │   ├── pages/
    │   ├── components/
    │   ├── hooks/
    │   └── utils/
    └── README.md                  <-- Full frontend documentation
```

---

# 📘 <a name="backend-docs"></a> **8. Backend Documentation**

Complete backend documentation is available at:

👉 **`/backend/README.md`**

Includes:

* Full architecture
* Story Protocol scripts
* Register IP workflows
* Mint license workflows
* SQLite schema
* API routes
* .env config
* How backend communicates with Story Protocol

---

# 💻 <a name="frontend-docs"></a> **9. Frontend Documentation**

Detailed UI documentation is available at:

👉 **`/sp-frontend/README.md`**

Includes:

* Page structure
* API usage
* Asset explorer
* Marketplace design
* Revenue claims page
* Wallet integration

---

# 🔧 **10. Setup Instructions**

### Clone repo

```bash
git clone https://github.com/yourname/dravik.git
cd dravik
```

---

## 🖥️ Backend Setup

```
cd backend
npm install
cp .env.example .env
npm run dev
```

---

## 🎨 Frontend Setup

```
cd sp-frontend
npm install
npm run dev
```

---


# 📜 **12. License**

MIT License — free for all usage.

👉 **“Generate frontend README”**
