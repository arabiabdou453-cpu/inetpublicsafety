# iNet Public Safety - Next Generation CAD & NG911 Call Handling Platform

[![GitHub Pages](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-brightgreen?style=for-the-badge&logo=github)](https://arabiabdou453-cpu.github.io/inetpublicsafety/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Node.js](https://img.shields.io/badge/Node.js-18%2B-green?style=for-the-badge&logo=node.js)](https://nodejs.org/)
[![Standards](https://img.shields.io/badge/Standards-NENA%20%7C%20NG911%20%7C%20NIEM-orange?style=for-the-badge)](https://www.nena.org/)

An enterprise-grade, map-centric Computer-Aided Dispatch (CAD), Next-Generation 911 (NG911) Call Handling System (CHS), and in-field mobile dispatch platform engineered for mission-critical emergency response operations across Police, Fire, and Emergency Medical Services (EMS).

---

## 🌟 Live Demo

- **Public Live Application:** [https://arabiabdou453-cpu.github.io/inetpublicsafety/](https://arabiabdou453-cpu.github.io/inetpublicsafety/)
- **Source Repository:** [https://github.com/arabiabdou453-cpu/inetpublicsafety](https://github.com/arabiabdou453-cpu/inetpublicsafety)

---

## 🏛️ Platform Architecture Overview

iNet Public Safety delivers a unified, high-reliability command-and-control ecosystem designed to meet the rigorous demands of primary and secondary Public Safety Answering Points (PSAPs), regional emergency dispatch centers, and hospital EMS networks.

```
+-----------------------------------------------------------------------------------+
|                        iNet Public Safety Unified Ecosystem                       |
+-----------------------------------------------------------------------------------+
         │                                       │                          │
         ▼                                       ▼                          ▼
+───────────────────────────+   +───────────────────────────+   +───────────────────────────+
|         iNetCAD           |   |       iNet911 CHS         |   |        iNetMobile         |
| • Map-Centric Dispatch    |   | • NG911 / E911 Core       |   | • In-Vehicle Touch MDT    |
| • Automatic Vehicle Loc.  |   | • iNetPhone Softphone     |   | • Turn-by-Turn Routing    |
| • Multi-Agency Routing    |   | • NENA i3 Standard Compl. |   | • Tactical Status Sync    |
| • Active/Active Redundancy|   | • CAD Cross-Integration   |   | • Offline Resilient Sync  |
+───────────────────────────+   +───────────────────────────+   +───────────────────────────+
         │                                       │                          │
         └───────────────────────────────┬───────┴──────────────────────────┘
                                         ▼
+-----------------------------------------------------------------------------------+
|                      Interoperability & External Interfaces                       |
|   • ESRI GIS Mapping   • Priority Dispatch ProQA   • CPIC Interfacing   • RMS     |
+-----------------------------------------------------------------------------------+
```

---

## 🚀 Key Modules & Capabilities

### 1. iNetCAD (Computer-Aided Dispatch)
- **Map-Centric Interface:** Dispatch directly from real-time spatial GIS layers with dynamic unit tracking and automatic recommended unit recommendations.
- **Enterprise Scalability:** Validated at scale from single-seat regional centers to nationwide multi-agency operations with **220+ simultaneous CAD consoles**.
- **Active/Active High Availability:** Real-time bi-directional synchronization between geographically separated data centers ensures zero downtime and instant failover.
- **Cross-Agency Dispatching:** Orchestrates unified responses across Police, Fire, and EMS with agency-specific SOPs and run-cards.

### 2. iNet911 CHS (Next-Generation 911 Call Handling System)
- **iNetPhone Softphone Console:** Streamlined softphone console built for rapid call triage, conference transfers, and ANI/ALI location presentation.
- **NENA i3 & NG911 Standards:** Built to support NG911 ESInet ingress, emergency incident data documents (EIDD), and legacy E911 trunk migration.
- **CAD/Call-Handling Fusion:** Out-of-the-box shared geospatial mapping and one-click call launching directly inside CAD.

### 3. iNetMobile & Field Responder Suite
- **In-Cab Mobile Data Terminals (MDT):** High-contrast day/night user interface designed for in-vehicle and ruggedized tablet hardware.
- **Situational Awareness:** Real-time call updates, hazard warnings, hydrants, pre-plans, and mutual aid unit telemetry.
- **Flexible Connectivity:** Native multi-bearer support over commercial 4G/5G cellular, FirstNet, satellite, private Wi-Fi, and VPN tunnels.

### 4. Seamless Interfacing
- **Emergency Medical Priority Dispatch (ProQA):** Embedded medical protocol interrogation.
- **ESRI ArcGIS Enterprise:** Native integration with authoritative municipal and regional GIS layers.
- **Law Enforcement Queries:** Certified CPIC / NCIC criminal record checks and state registry lookups.

---

## 🌍 Proven Global Deployments

| Client / Agency | Jurisdiction | Scope & Implementation |
|:---|:---|:---|
| **National 911** | Dominican Republic | Countrywide unified Police, Fire, and Ambulance dispatch for **11.5M citizens**. Operates **220+ CAD positions** across two active/active PSAPs handling sustained volumes of **15,000 to 30,000 calls per day** for over a decade. |
| **PEI Provincial 911** | Prince Edward Island, Canada | Province-wide Fire and Ambulance dispatching using integrated iNet911 CHS, iNetPhone, iNetCAD, and in-field iNetMobile units. |
| **Mercy Hospital Network** | USA | EMS Dispatch Center with 10 dispatch consoles, 80+ ambulance units, integrated ProQA medical protocols, and dedicated Mobile Command Center vehicles. |
| **Taber Regional 911** | Alberta, Canada | Multi-agency 911 center providing regional Fire and Police dispatching with direct interfaces to CPIC and ProQA. |

---

## 💻 Tech Stack & Deployment Options

- **Frontend:** Semantic HTML5, CSS3 responsive grid/flexbox, vanilla ES6+ automated carousel slider.
- **Runtime / Server:** Zero-dependency Node.js HTTP static server with automated MIME resolution.
- **Hosting Models:** Available for on-premise high-availability server clusters or cloud-hosted SaaS deployment.

---

## 🛠️ Quick Start Guide

### Prerequisites
- Node.js (v16.0 or higher recommended)
- Git

### Installation & Local Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/arabiabdou453-cpu/inetpublicsafety.git
   cd inetpublicsafety
   ```

2. **Start the local server:**
   ```bash
   npm start
   ```

3. **Open the browser:**
   ```
   http://localhost:3000
   ```

*(Alternatively, because this project contains zero runtime dependencies, you can also launch it with any static web server such as `npx serve .` or Python's `python -m http.server 3000`.)*

---

## 📁 Repository Structure

```
inetpublicsafety/
├── images/                        # Platform graphics, customer logos & UI assets
│   ├── about_team.png
│   ├── arowreadmore.png
│   ├── esri trans small.png
│   ├── image003.png
│   ├── images.jpg
│   ├── inback.png
│   ├── inetps_resized.png
│   ├── islandems.PNG
│   ├── mercy.jpg
│   └── sail1.jpg
├── includes/                      # Slideshow visual assets & styling
│   └── jQuerySlideshow/
│       ├── jQuerySlideshow2.css
│       └── images/jQuerySlideshow2/
├── stylesheets/                   # Modular layout and typography styles
│   ├── index.css
│   └── reset.css
├── index.html                     # Main application entry point
├── package.json                   # Project metadata & npm scripts
├── server.js                      # Zero-dependency local Node.js server
├── LICENSE                        # MIT License
└── README.md                      # Project documentation & overview
```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
