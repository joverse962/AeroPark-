# 🚁 AeroPark Sentinel

## Command Center for Autonomous Drone Parking Monitoring

**AeroPark Sentinel** is a professional, real-time drone monitoring system designed for automated parking lot enforcement and data collection. Built with modern web technologies, it provides a cyber-industrial command center aesthetic for managing autonomous drone operations.

---

## Demo
https://github.com/user-attachments/assets/ff2409dc-da0a-422f-873f-e9c9ac40cf75

## 🛠 Technical Stack

### Frontend Framework
- **AstroJS** - File-based routing with server-side rendering for optimal performance
- **React** - Interactive UI components via `@astrojs/react` integration
- **TypeScript** - Type-safe development

### Styling & Design
- **Tailwind CSS v4** - Utility-first CSS framework with custom cyber-industrial theme
- **Custom Theme**: Deep Slate (`#020617`) background with Electric Blue (`#3b82f6`) and Alert Red (`#ef4444`) accents
- **Glassmorphism Effects** - Modern frosted-glass UI elements
- **Custom Animations** - Pulse effects, glows, and transitions for active states

### UI Components
- **Lucide React** - Modern, technical line-based iconography for hardware and data visualization

---

## 🚀 The Core Concept

### Hardware-Software Loop

1. **Stationary Mode**: Drone remains docked, monitoring entrance via long-range sensor
2. **Detection & Launch**: Autonomous launch triggered upon vehicle entry detection
3. **The Scan**: Drone maneuvers above vehicle to scan QR/Bar code on roof or dashboard
4. **Data Sync**: Scanned code cross-referenced with database to create "Vehicle Profile"
5. **Enforcement**: Automatic flagging of violations (overstays, after-hours entries)

---

## ⚙️ System Architecture

This section illustrates the core components of the AeroPark Sentinel system.

### 1. Autonomous Drone
The eye in the sky. The drone is equipped with an ESP32-S3 camera module and is responsible for autonomously navigating the parking area to scan vehicles.

<img width="700" height="500" alt="Drone pic" src="https://github.com/user-attachments/assets/ca3e96a5-1390-4ea7-ba25-4807e7fa0a43" />


### 2. ESP32-S3 CAM
The brain of the drone's vision system. This powerful microcontroller captures images of vehicle QR codes/barcodes and transmits them to the command center for processing.

<img width="500" height="400" alt="esp32s3 sense cam" src="https://github.com/user-attachments/assets/4dcf93e5-6d6d-41f8-ac3a-0b273d079357" />


### 3. AeroPark Sentinel Web Page
The command center. This web application provides a real-time overview of the parking facility, drone status, and violation management.

<img width="1000" height="600" alt="AeroPage" src="https://github.com/user-attachments/assets/cf853ee0-0d62-4492-8170-debd8875aa51" />


---

## 📊 Feature Pages

### 1. Live Operations Dashboard (`/`)
**Real-time drone control and monitoring**

Features:
- **FPV Live Feed** - High-definition video stream with AR overlay
- **Telemetry HUD** - Real-time battery, altitude, GPS, temperature, and signal strength
- **Manual Override Controls** - "Return to Base" and "Hover Mode" emergency commands
- **Recent Scans** - Live feed of vehicle detections and validations
- **Weather Conditions** - Current environmental data for flight safety
- **System Alerts** - Real-time notifications and status updates

### 2. Intelligence & Enforcement (`/intelligence`)
**Automated violation tracking and vehicle profiling**

Features:
- **Active Violations** - Real-time overstay and after-hours alerts
- **Overstay Detection** - Automatic flagging when vehicles exceed paid duration
- **After-Hours Security** - Red-alert status for entries outside operating hours
- **Profile History** - Searchable log of every vehicle entry
- **Violation Analytics** - Breakdown of compliance rates and violation types
- **Quick Actions** - Search profiles, generate citations, send notifications
- **Most Frequent Vehicles** - Tracking of regular visitors

### 3. Predictive Maintenance (`/maintenance`)
**Hardware health monitoring and preventive scheduling**

Features:
- **Component Health Status** - Real-time monitoring of propellers, battery, motors, cameras
- **Flight Minutes Tracking** - Alerts for component replacement timing
- **Weather Grounding** - Weather API integration preventing unsafe flight conditions
- **Maintenance Schedule** - Upcoming service reminders and firmware updates
- **Parts Inventory** - Track spare parts and order supplies
- **Maintenance History** - Complete log of all service activities
- **Auto-Grounding Thresholds** - Configurable safety limits (wind, rain, visibility)

### 4. Analytics (`/analytics`)
**Data visualization and reporting** (existing page)

---

## 🎨 Visual Design System

### Theme: Cyber-Industrial

**Color Palette:**
- **Base**: `#020617` (Deep Slate 950) - Primary background
- **Accent Blue**: `#3b82f6` - Active states, primary actions
- **Alert Red**: `#ef4444` - Violations, critical warnings
- **Success Green**: `#22c563` - Valid operations, healthy status
- **Warning Yellow**: `#eab308` - Cautions, scheduled maintenance

### Typography:
- **Font**: Inter (Google Fonts) - Modern, highly legible
- **Monospace**: Used for vehicle IDs, telemetry data, technical readouts

### UI Patterns:
- **Glassmorphism**: Frosted glass cards with backdrop blur
- **Card Hover Effects**: Subtle lift and glow on interaction
- **Pulse Animations**: Active status indicators with breathing effect
- **Glow Effects**: Color-coded glows (blue/red/green) for status emphasis

## 📂 Project Structure

The project is organized with a clear and modular file structure:

```
/
├── public/                  # Static assets (images, fonts)
├── src/
│   ├── assets/              # Project-specific assets
│   ├── components/          # Reusable React components (.tsx) and Astro components (.astro)
│   ├── hooks/               # Custom React hooks
│   ├── layouts/             # Main site layout
│   ├── pages/               # Astro pages for routing
│   └── styles/              # Global stylesheets
├── astro.config.mjs         # Astro configuration
├── package.json             # Project dependencies and scripts
└── tailwind.config.mjs      # Tailwind CSS configuration
```

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
