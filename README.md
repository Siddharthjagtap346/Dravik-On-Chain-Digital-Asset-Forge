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

---

# 🔥 **UNIQUE ADDITION — Optional PizzaDAO Integration 🍕**

During asset registration, the creator can toggle:

> **“Attach PizzaDAO IP metadata?”**
> ✔ If enabled → Pizza DAO’s CC0-style metadata **plus the logo** is injected into the asset metadata:
<div align="center">
  <img src="https://github.com/user-attachments/assets/b11d4fbf-cf29-4bd1-9d5c-f6d36a9a3fbc" alt="PizzaDAO Logo" width="80" style="vertical-align:middle; margin-right:10px;" />
  <span style="font-size:1.1em; vertical-align:middle;">PizzaDAO metadata attached</span>
</div>

![pizzadao](https://github.com/user-attachments/assets/b11d4fbf-cf29-4bd1-9d5c-f6d36a9a3fbc)

### Use cases:

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

# 📸 **8. App Screens (UI Preview)**

*(Replace the placeholders with your actual screenshots in `/screenshots/`)*

## Landing Page

<img width="1755" height="3072" alt="image" src="https://github.com/user-attachments/assets/a5baaae0-184c-4471-ae46-d8b482a43ce7" />


## 🔐 Login Screen

A clean wallet + password login flow with JWT authentication.

<img width="1874" height="780" alt="image" src="https://github.com/user-attachments/assets/d7f65224-87ca-40a5-84c8-dce0a141dbd2" />


---

## 📝 Signup Screen

Simple signup with wallet + password + optional email.

<img width="1755" height="916" alt="image" src="https://github.com/user-attachments/assets/4fc86d6c-eb08-4054-8b78-693c377465e4" />


---

## 🏠 Main Dashboard

Shows user assets, marketplace shortcuts, revenue summary, and Story Protocol sync status.

<img width="1755" height="1142" alt="image" src="https://github.com/user-attachments/assets/36f222a6-5af7-4e83-b5bc-59521d17a87f" />


---

## 📤 Asset Registration Form

Creators upload any file → backend hashes it → uploads to Pinata → registers IP on Story Protocol.

<img width="1755" height="1830" alt="image" src="https://github.com/user-attachments/assets/7b270931-0b59-4f4d-a8c6-572e18f5acd6" />

Includes optional **PizzaDAO IP integration**:

> “Add to PizzaDAO Decentralized IP Registry (Optional)”
> ✔ If selected → pizzaDAO-logo.png rendered next to asset

<img width="1755" height="1963" alt="image" src="https://github.com/user-attachments/assets/33685fbe-0df8-4eff-b9eb-528af4cae510" />

---

## 🛒 Marketplace Screen

Beautiful asset cards showing:

* Image preview
* IP id
* Creator wallet address
* Price & license terms summary
* “Buy License” button

<img width="1870" height="1023" alt="image" src="https://github.com/user-attachments/assets/57dceb55-7154-4c66-8b25-a5f605f347dc" />


---

## 🧾 License Card UI (Purchased Licenses)

Shows:

* License ID
* Asset preview
* Full terms JSON
* Download asset button
* Revenue share details
* “View on Story Explorer” link
* Dynamic Story-chain sync badge (Green = synced)

<img width="1755" height="1278" alt="image" src="https://github.com/user-attachments/assets/584f5e73-0a31-44a4-b5ee-e07ed9f22df7" />


---

## 💰 IPFi Dashboard (Earnings + Claiming)

Includes:

* Claimable revenue
* Total earned
* Withdraw button (Story Protocol)
* Recent licensing activity

<img width="1755" height="1173" alt="image" src="https://github.com/user-attachments/assets/0186d7ad-ef59-48b4-8ba4-f0757e836b46" />



---

## 🌐 Story Dashboard (On-Chain View)

Integrates with Story Explorer:

* Shows registered IPs
* Shows license tokens
* “View on Story Explorer” button
* Status: Registered / Syncing / Minting / WIP revenue calculating

<img width="1755" height="1263" alt="image" src="https://github.com/user-attachments/assets/dcf840e2-d26c-4b6d-ac5f-2c0aa224fd3f" />


---


# 📁 **9. Repository Structure**

The Dravik repository is organized into two main sections: **frontend** (`sp-frontend`) and **backend** (`backend`). Below is a full breakdown of the folder structure and key files.

```
/
│── README.md                      <-- Main project documentation
│
├── backend/                       <-- Backend + Story Protocol SDK scripts
│   ├── src/
│   │   ├── server.ts              <-- Main Express server & all API routes
│   │   │                             (handles registration, licensing, royalty, dispute,
│   │   │                             Story Protocol, BAV verification, Pinata uploads, DB, auth)
│   │   ├── story/                 <-- Helper scripts for Story Protocol workflows
│   │   ├── pinata/                <-- IPFS upload utilities (Pinata integration)
│   │   ├── db/                    <-- SQLite helpers, schema, queries
│   │   └── auth/                  <-- JWT login & wallet pairing utilities
│   ├── public/                     <-- Public backend assets (optional)
│   ├── scripts/                    <-- Advanced workflows & registration/license scripts
│   │   ├── derivative/
│   │   ├── licenses/
│   │   └── registration/
│   └── README.md                  <-- Full backend documentation
│
└── sp-frontend/                   <-- React + TypeScript + Tailwind
    ├── src/
    │   ├── pages/                 <-- Main pages (Landing, Dashboard, RegisterAsset, etc.)
    │   ├── components/            <-- UI components (AssetCard, Sidebar, Footer, etc.)
    │   ├── hooks/                 <-- Custom React hooks
    │   └── utils/                 <-- Frontend utility functions
    └── README.md                  <-- Full frontend documentation
```

### **Key Points**

* **server.ts** is the main entry point for all backend functionality. Most "logic" lives here.
* Folders like `story/`, `pinata/`, `db/`, `auth/` are helpers or modules used by `server.ts`.
* `/scripts` contains all advanced scripts for registration, license minting, royalties, and derivative IP management.
* Frontend handles all UI, dashboards, marketplace, asset browsing, wallet auth, and API calls to backend.


---

# 📘 **10. Backend Documentation**

Got it! I can help you update your README to clearly include the **folder structure** details for both `sp-frontend` and `backend` with all the key files you listed. Here's a polished version you can paste into your current README, adding it after your existing **Repository Structure** section:

---

## **Backend — backend**

Node.js + Express backend with TypeScript powering API routes, Story Protocol interactions, BAV, IPFS upload, licensing, and royalty tracking.

```
backend/
├── src/
│   ├── server.ts                 <-- Main Express server & all API routes (register, license, royalty, dispute)
│   ├── story/                    <-- Story Protocol SDK scripts & workflows
│   ├── pinata/                   <-- IPFS & Pinata upload utilities
│   ├── db/                       <-- SQLite helpers & schema
│   ├── auth/                     <-- JWT login & wallet authentication
│   ├── types/                    <-- TypeScript declarations
│   │   ├── better-sqlite3.d.ts
│   │   ├── express.d.ts
│   │   └── registerDynamic.ts
│   ├── utils/                    <-- Backend utility functions
│   │   ├── abi/
│   │   │   ├── defaultNftContractAbi.ts
│   │   │   ├── licenseAttachmentWorkflowsAbi.ts
│   │   │   ├── licensingModuleAbi.ts
│   │   │   └── totalLicenseTokenLimitHook.ts
│   │   └── functions/
│   │       ├── createSpgNftCollection.ts
│   │       ├── mintNFT.ts
│   │       ├── uploadToIpfs.ts
│   │       ├── config.ts
│   │       └── utils.ts
├── database.db                   <-- SQLite database
├── .env
├── .env.example
├── .gitignore
├── .pre-commit-config.yaml
├── .prettierrc
└── scripts/                      <-- Advanced scripts for registration, licenses, royalty, derivative IP, disputes
    ├── derivative/
    │   ├── registerDerivativeCommercial.ts
    │   ├── registerDerivativeCommercialCustom.ts
    │   └── registerDerivativeNonCommercial.ts
    ├── licenses/
    │   ├── mintLicense.ts
    │   ├── oneTimeUseLicense.ts
    └── registration/
        ├── register.ts
        ├── registerCustom.ts
        └── registerDynamic.ts
```

### **Backend Responsibilities**

* REST APIs for asset registration & licensing
* SHA-256 fingerprinting + BAV validation
* IPFS uploads via Pinata
* Story Protocol interactions (IP registration & license minting)
* SQLite-based asset & license storage
* JWT wallet-based authentication
* Royalty tracking, one-time-use licenses, and derivative registrations

---

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

# 💻 **11. Frontend Documentation**

## **Frontend — sp-frontend**

React + TypeScript + Tailwind application handling the user interface, marketplace, dashboards, and wallet integration.

```
sp-frontend/
├── dist/                         <-- Production build output
├── node_modules/                 <-- Dependencies
├── public/                       <-- Public assets (favicon, index.html, logos, etc.)
├── src/
│   ├── assets/                   <-- Images, logos, icons, media
│   ├── components/               <-- React components
│   │   ├── AddToMarketplace.tsx
│   │   ├── AssetCard.tsx
│   │   ├── Dashboard.tsx
│   │   ├── Footer.tsx
│   │   ├── Header.tsx
│   │   ├── IPFiDashboard.tsx
│   │   ├── LandingPage.tsx
│   │   ├── LicenseMarketplace.tsx
│   │   ├── Login.tsx
│   │   ├── MyAssetsPage.tsx
│   │   ├── OwnedLicenseCard.tsx
│   │   ├── RegisterAsset.tsx
│   │   ├── RegisterAssetPage.tsx
│   │   ├── Sidebar.tsx
│   │   ├── Signup.tsx
│   │   └── ...other components
│   ├── App.tsx                   <-- Main React entry component
│   ├── App.css
│   ├── index.css
│   ├── main.tsx                  <-- App mounting
│   ├── TS global.d.ts            <-- TypeScript global declarations
│   └── utils/                    <-- Frontend utility functions
├── .gitignore
└── README.md                     <-- Frontend documentation
```

### **Frontend Responsibilities**

* Asset registration UI
* Marketplace browsing & license purchase
* Revenue & claims dashboard
* Wallet authentication
* Integration with backend APIs and Story Protocol SDK

---
Includes:

* Page structure
* API usage
* Asset explorer
* Marketplace design
* Revenue claims page
* Wallet integration

---

# 🔧 **12. Setup Instructions**

### Clone repo

```bash
git clone https://github.com/Siddharthjagtap346/dravik.git
cd dravik
```

---

## 🖥️ Backend Setup

```
cd backend
npm install
cp .env.example .env
npm run server
```

---

## 🎨 Frontend Setup

```
cd sp-frontend
npm install
npm run dev
```

---


# 📜 **13. License**

MIT License — free for all usage.

