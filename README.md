# 🌱 Lexfund – ICP Hackathon Project

**Lexfund** is a decentralized farming and crop management platform built on the **Internet Computer Protocol (ICP)**. It enables farmers, stakeholders, and users to interact seamlessly with crop data, manage resources, and ensure transparency through blockchain-backed storage.


Built for the Legal Tech Hackathon 2025

The project consists of:

* **Backend**: Rust canister handling data storage, user interactions, and business logic.
* **Frontend**: React-based UI for interacting with the canister in a user-friendly way.

---

## 🚀 Features

### Backend (ٌRust Canister)

The backend implements all core functionalities for managing crops and users.

**Main Functions:**

* `addFarmer(name : Text, location : Text)` → Registers a new farmer in the system.
* `getFarmer(farmerId : Nat)` → Retrieves details about a specific farmer.
* `addCrop(farmerId : Nat, cropName : Text, quantity : Nat, harvestDate : Text)` → Adds a crop entry for a given farmer.
* `getCrops(farmerId : Nat)` → Fetches all crops linked to a farmer.
* `updateCrop(cropId : Nat, quantity : Nat, harvestDate : Text)` → Updates crop details.
* `removeCrop(cropId : Nat)` → Deletes a crop entry from the records.
* `listAllFarmers()` → Returns all registered farmers.
* `listAllCrops()` → Returns all crops in the system across all farmers.

🔒 **Security Considerations:**

* Access-controlled farmer and crop management.
* On-chain storage of farmer and crop records for transparency.

---

### Frontend (React dApp)

The frontend provides a smooth, responsive, and user-friendly interface to interact with the backend canister.

**Key Features:**

* 🌾 **Farmer Dashboard** – View and manage farmer details.
* 🌱 **Crop Management** – Add, update, and delete crop entries.
* 📊 **Crop Overview** – List all crops and filter by farmer.
* 🔍 **Search & Filter** – Easily find farmers or crops.
* 🖥️ **ICP Integration** – Connects directly to the deployed canister for live data sync.

---

## 🛠️ Tech Stack

* **Backend**: Motoko (ICP Canisters)
* **Frontend**: React, TailwindCSS
* **Blockchain**: Internet Computer Protocol (ICP)
* **Deployment**: DFX, Canister architecture

---

## ⚙️ Installation & Setup

### Prerequisites

* Install [DFINITY SDK (dfx)](https://internetcomputer.org/docs/current/developer-docs/setup/install)
* Install [Node.js](https://nodejs.org/)

### Clone the Repository

```bash
git clone https://github.com/danielchukwuu/Lexfund.git
cd Lexfund
```

### Backend Setup

```bash
dfx start --background
dfx deploy
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## 📸 Screenshots

(Add 2–3 screenshots of your frontend UI: farmer dashboard, crop list, etc.)

---

## 🤝 Contributing

Contributions are welcome! Please fork the repo and submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

