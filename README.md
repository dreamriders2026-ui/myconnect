# 🌐 MyConnect - System Status & Maintenance

This repository serves as the **Remote Configuration** and **Maintenance Hub** for the **MyConnect** AI Chat application. 

### 🤖 About MyConnect
MyConnect is a next-generation AI platform focused on immersive **Character Roleplay** and interactive storytelling. 

---

### 🛠 Maintenance Configuration
The client-side application (iOS/Android/Web) fetches the `maintenance.json` file from this repository to check for system-wide updates or scheduled downtime.

* **File:** `maintenance.json`
* **Purpose:** Kill-switch and service announcements.
* **File:** `welcome.json`
* **Purpose:** Marketing announcements, onboarding messages, and MOTD (Message of the Day).
* **File:** `policy.json`
* **Purpose:** Legal and compliance notices, such as Privacy Policy or Terms of Service updates.

### 📡 Current Status Structure
The client application fetches configuration from three separate files, each serving a distinct purpose:

1.  **`maintenance.json`**: Handles critical operational states.
    *   **Forced Updates**: Requires users to update to a minimum client version.
    *   **Maintenance Mode**: Informs users about scheduled downtime or ongoing service interruptions, with the ability to block app access.

2.  **`welcome.json`**: Manages user engagement and marketing messages.
    *   **Welcome Messages**: Displays non-critical announcements, feature highlights, or "Message of the Day" (MOTD) pop-ups.
    *   **Targeted Content**: Can deliver different messages to different user segments (e.g., `default` vs. `premium_users`).

3.  **`policy.json`**: Governs legal and compliance notifications.
    *   **Policy Updates**: Notifies users of changes to the Terms of Service or Privacy Policy.
    *   **Blocking Consent**: Can require users to review and accept policy changes before continuing to use the app.

This separation ensures clarity, reduces risk, and allows for independent management of technical, marketing, and legal configurations.

### 🚀 Contact & Support
If you are a developer or a user experiencing issues not reflected in the status file, please reach out via the main MyConnect portal.