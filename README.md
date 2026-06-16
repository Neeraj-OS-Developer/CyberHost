# 🌐 CyberHost – Your Private Offline Host

Welcome to **CyberHost**, your ultimate personal assistant-driven, 100% offline peer-to-peer (P2P) file-sharing network. CyberHost allows you to host a local web server and share files securely via Wi-Fi Direct without needing an internet connection.

---

## 🚀 Key Features & UI Guide

### 1. ⬅️ Back Button (Top Left)
* Takes you directly to the **Privacy & Info** page, where you can read our full offline compliance policy.

### 2. 🔑 Credential Panel
* **SSID Field:** Your Wi‑Fi Direct network name (automatically prefixed with `DIRECT‑NS‑`).
* **Password Field:** Set a strong password (8–20 characters) to protect your P2P group.
* *Note: The key icon next to the password is a decorative element matching the app's cyber theme.*

### 3. 📶 Band Toggle (2.4 GHz / 5 GHz)
* **2.4 GHz:** Longer range, better penetration through walls, standard speed.
* **5 GHz:** Ultra-fast data transfer, ideal for high-speed close‑range sharing.
* *Tapping a band instantly restarts the P2P group with the new frequency.*

### 4. 🛡️ Security Log
* Opens a scrollable popup listing all allowed and blocked devices.
* Easily **REMOVE** a previously allowed device or **UNBLOCK** a blocked one.
* IP addresses are highlighted in bright green for high visibility.

### 5. ⚙️ Network Config (Server Port)
* Change the default web server port (Default: `3000`).
* **Valid Range:** `1024` – `65535`.
* Modifying the port automatically updates the QR codes and safely restarts the system.

### 6. 📝 Grant Permissions
* Requests essential permissions: Storage, Wi‑Fi, and Notifications.
* **100% Offline Guarantee:** Permissions are strictly used for local file sharing and P2P networking. No internet access is required or used.

### 7. ▶️ Server Start
* Initializes the Wi‑Fi Direct group and launches the internal web server.
* Once online, the status turns green, displaying the SSID and the number of connected devices.
* The local portal is accessible at: `http://192.168.49.1:<port>`

### 8. 🔄 Apply & Restart Button
* Instantly saves your SSID, password, band, and port settings.
* Restarts the foreground service and the P2P group seamlessly.

### 9. 🔳 QR Code Section
* **WiFi SCAN QR:** Other devices can scan this to join your P2P network automatically.
* **OPEN PORTAL QR:** Scan to open the local web portal directly in any browser for instant file uploads/downloads.

### 10. 🎙️ The Assistant Girl (Interactive AI Guide)
* **Drag & Drop:** Move her anywhere on the screen.
* **Tap:** Opens the interactive help bubble.
* **Long-Press:** Cycles through sizes (Small / Medium / Large).
* **Voice Assistant:** Features a microphone mute/unmute button. When unmuted, she reads the entire guide aloud sentence-by-sentence in **Hindi** for a natural experience.

### 11. 🤫 Secret Volume Combo
* Press **Volume Up + Volume Down** simultaneously to open a hidden feedback/complaint form to email the developers directly.

---

## 🔒 Security & Privacy (Zero-Trust Offline Architecture)

CyberHost is engineered with a strict **Privacy-First** approach:

* **Physical Isolation:** Works 100% OFFLINE. No internet, no cloud storage, and zero tracking.
* **Encryption:** * Local device-to-device communication is secured via industry-standard **WPA2/WPA3** (depending on hardware support).
  * Web portal traffic utilizes **HTTPS** with a self-signed certificate for local connections.
  * Data at rest is secured by Android's native file encryption.
* **Data Ownership:** Your SSID and passwords are saved locally inside sandboxed **SharedPreferences**. They cannot be recovered if lost—this is by design for maximum security.
* **Clean Codebase:** Zero analytics, zero ads, no backdoors, and no third-party tracking libraries.

> 💡 **TIP:** If you ever forget your password, simply set a new one from the main screen. Due to our cryptographic design, the old password cannot be recovered.

---

## 🛠️ Tech Stack & Requirements

* **Platform:** Android
* **Minimum Network Requirement:** Wi-Fi Direct (P2P) compatible hardware
* **Local IP Address:** `192.168.49.1`
