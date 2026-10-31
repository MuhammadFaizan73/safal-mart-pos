<div align="center">

<img src="assets/banner.svg" alt="Safal Tech Mart POS" width="100%"/>

<br/>

<img src="https://img.shields.io/badge/Electron-47848F?style=for-the-badge&logo=electron&logoColor=white" alt="Electron"/> <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=white" alt="React"/> <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express"/> <img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="SQLite"/> <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"/>

<br/>

<img src="https://img.shields.io/badge/Status-Active%20development-success?style=flat-square" alt="status"/>
<img src="https://img.shields.io/badge/Source-Private%20(commercial)-lightgrey?style=flat-square" alt="source"/>

**[Request a live demo](https://rootocloud.com) · [Hire me](mailto:faizan.developer9200@gmail.com) · [More projects](https://github.com/MuhammadFaizan73)**

</div>

---

## 📌 Overview

A retail and grocery point-of-sale built as a desktop app that also runs in the browser for development. All totals are computed on the server at checkout, with a promotions engine supporting buy-x-get-y, quantity discounts, combos and cart-value rules.

## ✨ Key Features

### Billing
- Barcode scan and search, categories, multi-bill tabs
- Hold and recall that survives a restart
- Split payments, returns and refunds, printed receipts

### Customers
- Loyalty points with tiers and redemption
- Khata (customer credit) balances updated automatically

### Inventory & Promotions
- Stock adjustments with audit trail and reorder levels
- Promotions engine: buy-x-get-y, quantity %, combo, cart-value
- Sales history with gross, returns, net and average basket stats

### HR
- Employees and payroll module

## 🏗️ Architecture

```mermaid
flowchart LR
  UI[React UI<br/>Vite] -->|/api| EX[Express server<br/>promo engine]
  EX --- DB[(SQLite)]
  subgraph Electron Desktop App
    UI
    EX
    DB
  end
  EX --> PR[Receipt Printer]
```

## 🧰 Tech Stack

| Layer | Technology |
|---|---|
| **Desktop** | Electron · electron-updater |
| **Frontend** | React · Vite · React Router · Zustand |
| **Backend** | Express (embedded) |
| **Database** | SQLite (better-sqlite3) |
| **Builds** | Windows .exe · macOS .dmg · Linux AppImage |

<!-- SCREENSHOTS -->
## 📸 Screenshots

<p align="center">
  <img src="docs/screenshots/01-employees.png" width="49%"/>
  <img src="docs/screenshots/02-employees.png" width="49%"/>
  <img src="docs/screenshots/03-employees.png" width="49%"/>
  <img src="docs/screenshots/04-employees.png" width="49%"/>
</p>

<!-- /SCREENSHOTS -->

## 🔒 About the Source Code

This is a **commercial / client project**, so the source code is kept in a private repository.
This page documents what the system does and how it is built.

- 🎥 **Live walkthrough** — available on request
- 💼 **Want something similar for your business?** I build custom versions of this for clients.

## 👨‍💻 Author

**Muhammad Faizan** — Founder, [Rootocloud](https://rootocloud.com)
AI agents & automation · Web & mobile apps · Custom software

[![Website](https://img.shields.io/badge/rootocloud.com-0B1220?style=for-the-badge&logo=googlechrome&logoColor=white)](https://rootocloud.com)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:faizan.developer9200@gmail.com)

<div align="center"><sub>© Muhammad Faizan. All rights reserved.</sub></div>
