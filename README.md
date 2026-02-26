# 🌐 MyConnect - System Status & Maintenance

This repository serves as the **Remote Configuration** and **Maintenance Hub** for the **MyConnect** AI Chat application. 

### 🤖 About MyConnect
MyConnect is a next-generation AI platform focused on immersive **Character Roleplay** and interactive storytelling. 

---

### 🛠 Maintenance Configuration
The client-side application (iOS/Android/Web) fetches the `maintenance.json` file from this repository to check for system-wide updates or scheduled downtime.

* **File:** `maintenance.json`
* **Purpose:** Kill-switch and service announcements.

### 📡 Current Status Structure
The app expects the following JSON format:

| Key | Type | Description |
| :--- | :--- | :--- |
| `is_maintenance` | Boolean | `true` blocks app access; `false` allows normal use. |
| `message` | String | The text displayed to users during downtime. |
| `min_version` | String | Forces users on older versions to update. |

### 🚀 Contact & Support
If you are a developer or a user experiencing issues not reflected in the status file, please reach out via the main MyConnect portal.