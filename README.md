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
Got it! We can definitely add a **Screenshots / UI Preview** section to your README for GitHub. This will let anyone visiting the repo immediately see the UI and output of Dravik without running the app. Here’s a polished version you can add **after your current content**, keeping placeholders that you can replace with actual images later:

---

# 📸 **13. App Screens (UI Preview)**

*(Replace the placeholders with your actual screenshots in `/screenshots/`)*

## 🔐 Login Screen

A clean wallet + password login flow with JWT authentication.

![Login Screen](screenshots/login.png)

---

## 📝 Signup Screen

Simple signup with wallet + password + optional email.

![Signup Screen](screenshots/signup.png)

---

## 🏠 Main Dashboard

Shows user assets, marketplace shortcuts, revenue summary, and Story Protocol sync status.

![Dashboard](screenshots/dashboard.png)

---

## 📤 Asset Registration Form

Creators upload any file → backend hashes it → uploads to Pinata → registers IP on Story Protocol.

Includes optional **PizzaDAO IP integration**:

> “Add to PizzaDAO Decentralized IP Registry (Optional)”
> ✔ If selected → pizzaDAO-logo.png rendered next to asset

![Registration Form](screenshots/registration_form.png)
![PizzaDAO Attach](screenshots/pizzadao_attach.png)

---

## 🛒 Marketplace Screen

Beautiful asset cards showing:

* Image preview
* Price & license terms summary
* Creator wallet address
* “Buy License” button
* IPFS & Story Explorer links

![Marketplace](screenshots/marketplace.png)

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

![License Card UI](screenshots/license_card_ui.png)

---

## 💰 IPFi Dashboard (Earnings + Claiming)

Includes:

* Claimable revenue
* Total earned
* Withdraw button (Story Protocol)
* Recent licensing activity

![IPFi Dashboard](screenshots/ipfi_dashboard.png)

---

## 🌐 Story Dashboard (On-Chain View)

Integrates with Story Explorer:

* Shows registered IPs
* Shows license tokens
* “View on Story Explorer” button
* Status: Registered / Syncing / Minting / WIP revenue calculating

![Story Dashboard](screenshots/story_dashboard.png)

---

✅ **Tips for GitHub:**

1. Create a `screenshots/` folder at the repo root.
2. Add your PNG/JPG screenshots there.
3. Use **relative paths** in the README like above: `screenshots/login.png`.
4. When ready, push to GitHub — they will render the images automatically in your README.

---


---

# 📸 **13. App Screens (UI Preview)**

| Login                           | Signup                            | Dashboard                               |
| ------------------------------- | --------------------------------- | --------------------------------------- |
| ![Login](screenshots/login.png) | ![Signup](screenshots/signup.png) | ![Dashboard](screenshots/dashboard.png) |

| Registration Form                                       | PizzaDAO Attach                                     | Marketplace                                 |
| ------------------------------------------------------- | --------------------------------------------------- | ------------------------------------------- |
| ![Registration Form](screenshots/registration_form.png) | ![PizzaDAO Attach](screenshots/pizzadao_attach.png) | ![Marketplace](screenshots/marketplace.png) |

| License Card UI                                     | IPFi Dashboard                                    | Story Dashboard                                     |
| --------------------------------------------------- | ------------------------------------------------- | --------------------------------------------------- |
| ![License Card UI](screenshots/license_card_ui.png) | ![IPFi Dashboard](screenshots/ipfi_dashboard.png) | ![Story Dashboard](screenshots/story_dashboard.png) |

---




# 📁 **8. Repository Structure**

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

# 📘 **9. Backend Documentation**

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

# 💻 **10. Frontend Documentation**

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

# 🔧 **10. Setup Instructions**

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


# 📜 **12. License**

MIT License — free for all usage.

