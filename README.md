---

# **ComRent: PC Rental Management Dashboard**

ComRent is a self-contained, front-end administrative dashboard designed for real-time supervision of computer rental sessions in an internet café environment. It provides operators with a clear, dynamic view of PC status, remaining session time, and essential transaction details.

![](images/Screenshot(1).png)
![](images/Screenshot(2).png)
![](images/Screenshot(3).png)

---

## ✨ **Features**

### **Session Management**

* **Real-Time Countdown:** Each active session shows a live, second-by-second timer under the *Time Left (HH:MM)* column.
* **Quick Session Start:** A modal enables administrators to register a user, choose an available PC, set duration, price, and payment method.
* **Automatic Status Changes:**

  * **Green:** Active
  * **Orange:** Less than 5 minutes remaining
  * **Red:** Expired/Offline
* **Manual Status Control:** Clicking the status indicator cycles through Active → Warning → Offline, clearing session data when set to Offline.

### **Data Management**

* **Inline Editing:** The *PC* and *Name* fields can be edited directly on the dashboard for immediate adjustments.

---

## 🛠️ **Technologies Used**

This prototype is implemented as a single, portable file for quick deployment:

* **HTML5:** Structure and layout
* **Vanilla JavaScript:** Timers, data management, and interactive logic
* **Tailwind CSS (CDN):** Clean and responsive interface with no external CSS files

---

## 🚀 **Getting Started**

No installation or build process is required.

### **Installation & Execution**

1. Save the provided source code as **index.html**.
2. Open **index.html** in any modern browser (Chrome, Firefox, Edge, Safari).

The dashboard loads instantly with placeholder data, and all timers begin running automatically.

---

## 💻 **Usage Guide**

| Action                   | Description                                                                                     |
| ------------------------ | ----------------------------------------------------------------------------------------------- |
| **Start New Session**    | Click **+ Start New Session**, select an available PC (Red), fill in user details, and confirm. |
| **Monitor Status**       | Track indicators: Green (Active), Orange (Warning), Red (Offline).                              |
| **Edit PC/Name**         | Click directly on the PC or Name fields to modify them.                                         |
| **End Session Manually** | Click the status square until it returns to Red to clear the session.                           |

---

## 📂 **Project Structure**

Current Architecture: **Single-file application**

```
/ (Root)
├── index.html   # Complete HTML, CSS, and JavaScript
└── README.md    # Documentation
```

### **Code Organization (inside index.html)**

* **HTML Head:** Viewport settings and Tailwind CDN
* **Custom <style>:** Minor visual adjustments (status indicator, highlights)
* **HTML Body:** Header, PC dashboard table (`#pcDashboard`), session modal (`#sessionModal`)
* **<script>:** Data model, rendering logic, timer engine, and interaction handlers

---

## 📦 **Packaging for Distribution (Planned)**

A future release aims to transition from browser-based to a full desktop application capable of enforcing PC lock screens.

* **Target OS:** Windows / Linux
* **Possible Frameworks:** Electron.js, JavaFX, PyQt
* **System Interaction:** Required for PC lock/unlock functionality
* **Synchronization:** Real-time data sharing via a backend (e.g., Firebase Firestore)

---

## 💡 **Future Enhancements**

* **Database Persistence:** Firebase Firestore integration
* **Session Extension Modal:** Add time, update price, log new payments
* **Email Invoice System:** Capture user email and send digital receipts
* **Admin Login & Rates Management:** Secure access and pricing configuration

---

## 📜 **Changelog**

### **v0.1.0 — Initial Prototype (November 2025)**

* Dashboard layout established
* Base data model introduced
* Live countdown timer implemented
* Automatic status transitions
* Session Start modal added
* Clickable status indicator
* Inline editing for PC/Name fields

---

## ⚙️ **System Requirements**

* **OS:** Any system running a modern browser
* **Browser:** Chrome, Firefox, Edge, Safari (ES6+ supported)
* **Internet:** Needed only for Tailwind CDN

---

## ⚠️ **Troubleshooting**

| Issue                 | Cause                          | Solution                                 |
| --------------------- | ------------------------------ | ---------------------------------------- |
| Timers stop running   | JavaScript error or throttling | Open Developer Console (F12) and refresh |
| Start button disabled | No PCs are in Red state        | Manually cycle a PC to Red               |
| Layout broken         | Tailwind failed to load        | Check internet connection                |

---

## 🙏 **Acknowledgements**

Developed by the project creator as part of the ComRent system.

---

## ⚖️ **License**

This project is licensed under the **MIT License**. A dedicated LICENSE file is recommended for distribution.

---

