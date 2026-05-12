# SW-NET Forensic v.2.0.0

## 🎨 General Changes
* **Complete Visual Overhaul:** Modern dark UI optimized for long-term forensic analysis.

## 🚀 New Features
* **Visual GeoIP Map:** Interactive world map of network traffic (the perfect "executive toy" for dashboards).
* **"Kill process with parent":** Hardcore termination of the entire process tree (Kill the root).
* **Network Anomaly Score Card:** New module in the "Network Information" menu for rapid risk assessment.
* **Suspicious Connections Filter:** One-click toggle to display only risky communications in the table.
* **Hide Microsoft Processes:** Filter out legitimate system processes to focus on real threats.
* **Command Line Inspector:** Intelligent highlighting of suspicious command-line arguments.
* **Privilege Level Analysis:** Detailed info on process origin and execution rights.
* **Process & Child Lineage:** Visual representation of parent/child relationships with live/dead status indicators.
* **AlienVault API Threat Intelligence:** Real-time automated threat analysis integration.
* **Report Export:** Generate forensic reports in PDF and HTML formats.
* **Advanced Search (Power-User engine):** Column-header searching with advanced support:
    * Port ranges (e.g., `1000-2000`, `>1024`, `<443`).
    * IP ranges via CIDR notation (e.g., `192.168.0.0/24`).
    * Logical operators and negation (`-`, `!`).
* **Process Tree Context Menu:** Added management tools directly in the tree view.
* **Persistent Connections Alert:** Dashboard alert for suspicious long-term connections.
* **Windows Native Notifications:** System tray alerts for new suspicious activities.
* **Minimize to Tray:** Ability to run the app silently in the system tray.

## ⚙️ Settings
* **Enhanced Startup Options:** Run on Windows startup (via startup folder) with "Start Minimized" and confirmation notifications.
* **AlienVault API Integration:** dedicated field for custom API keys.
* **Visual Polish:** Refined settings UI for better usability.

## 🔧 Bug Fixes & Improvements
* **Persistence Fix:** Resolved issues where settings, logs, and API keys were lost during updates.
* **Advanced Logging:** Comprehensive logging of all process and network events.
* **UI Fixes:** Fixed clickable labels for Hashes and icon alignment in API settings.
* **Code Refactoring:** Minor bug fixes and performance optimization of legacy functions.
