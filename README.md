<p align="center">
  <img src="https://github.com/SyedMuhammadSajawalHussain/SoftBits-Assistant/blob/main/Icon.png" alt="SoftBits Assistant Logo" width="200" height="200">
</p>

# SoftBits Assistant

**Tagline:** "Don't Lose What's Special Online"  
**Version:** 2.1.0  
**Developer:** Syed Muhammad Sajawal Hussain

SoftBits Assistant is a high-security, completely offline Android application designed for managing site credentials and bookmarks. Built with a zero-trust architecture, it ensures that your sensitive data never leaves your device and is protected against both digital and physical threats.

---

## 🛡️ Security Features

Security is the core pillar of SoftBits Assistant. The following industry-standard measures are implemented:

*   **AES-256 Encryption:** All site passwords and the master signup password are encrypted using Advanced Encryption Standard (AES-256) in CBC mode with PKCS5Padding and SHA-256 key derivation.
*   **Root Detection:** The app features a multi-level root detection system (checking for `su` binaries and `test-keys`). If a rooted device is detected, the app terminates immediately to prevent memory dumping or unauthorized database access.
*   **Anti-Screen Capture:** Global implementation of `FLAG_SECURE` prevents screenshots, screen recording, and hides app content in the "Recent Apps" task switcher.
*   **Background Protection:** For security, the app automatically locks and requires re-authentication whenever it is moved to the background and resumed.
*   **Data Isolation:** Uses Android's internal "Sandbox" storage. No data is stored in publicly accessible folders, and the app requires zero internet permissions.
*   **Privacy-Focused Inputs:** Autofill and predictive text suggestions are disabled for all credential fields to prevent the OS or keyboard from "learning" your sensitive information.
*   **Action Verification:** Sensitive actions—including unhiding a password, editing an entry, or deleting an entry—require re-verification of the master signup password.

---

## ✨ Key Functionalities

*   **One-Time Profile Creation:** Simple, secure signup with strictly alphabetic usernames and alphanumeric passwords (8-12 characters).
*   **Credential Management (CRUD):** 
    *   Save site titles, passwords (optional), and links (mandatory).
    *   Links are hidden by default and only viewable during a verified edit session.
    *   Passwords are masked with "••••••••" and can be temporarily unhidden for 5 seconds.
*   **Seamless Navigation:** Use the "Continue" button to open site URLs directly in your system's default browser via Implicit Intents.
*   **App Reset:** A "Forgot Credentials" feature in the startup menu allows for a full factory reset, wiping all local data if needed.
*   **Adaptive UI:** Fully standard implementation of Light and Night modes that follow your system settings for optimal readability.
*   **Device Compatibility:** Optimized for all resolutions with responsive scrolling and intelligent keyboard handling to prevent UI overlap.

---

## 🛠️ Technology Stack

*   **Language:** Java
*   **UI Framework:** XML (Android Material Components)
*   **Local Storage:** SQLite
*   **Security Libraries:** `javax.crypto`, `java.security`
*   **Minimum SDK:** Android 7.0 (API 24)
*   **Target SDK:** Android 15 (API 36)

---

## 🚀 How to Run

1.  **Clone the Project:** Import the source code into **Android Studio**.
2.  **Build:** Let Gradle sync and build the project.
3.  **Run:** Deploy to an emulator or physical device.
4.  **Note:** Due to root detection, the app will not run on devices with a compromised root status.

---

## 👨‍💻 Developer Information

*   **Name:** Syed Muhammad Sajawal Hussain
*   **Email:** [syedmuhammadsajawalhussain@gmail.com](mailto:syedmuhammadsajawalhussain@gmail.com)
*   **Contact:** 0328-0841432
*   **LinkedIn:** [linkedin.com/in/syedmuhammadsajawalhussain1432](https://www.linkedin.com/in/syedmuhammadsajawalhussain1432)

---

*Disclaimer: This app is strictly offline. The developer does not have access to any data saved within the application. User data is solely stored on the user's physical device.*
