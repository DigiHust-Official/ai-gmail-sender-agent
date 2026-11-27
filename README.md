#  DigiHust Gmail Sender Agent

**An Intelligent Chrome Extension for Automated, Anti-Spam Bulk Email Outreach**

Developed by **Muhammad Haseeb Ashraf** | **DigiHust**

---

## 📌 Overview

**DigiHust Gmail Sender Agent** is a specialized browser automation extension designed for high-deliverability B2B outreach, candidate recruitment, and client acquisition. 

Traditional bulk emailing methods (such as adding hundreds of recipients in **CC** or **BCC**) instantly trigger spam filters and put your email domain at risk. This extension solves that problem by sending **individual, personalized emails** to up to **500+ recipients** sequentially using smart **configurable time delays**. You can configure your campaign, hit start, and let the agent run autonomously in the background—even while you sleep.

---

## ✨ Key Features

- **🛡️ Anti-Spam Sequential Sending:** Sends separate, 1-on-1 emails instead of mass CC/BCC blasts, keeping sender reputation high and inbox placement optimal.
- **⏱️ Smart Time-Delay Engine:** Configurable delays between each email to mimic natural human sending behavior and bypass rate limits.
- **🤖 Autonomous Background Execution:** Runs seamlessly via background service workers (`background.js`) so you can leave your system running overnight without manual intervention.
- **📝 Built-in Proposal & Template Editor:** Dedicated template management (`templates.js` & `proposal-editor.js`) to customize outreach formats for different campaigns.
- **📊 Interactive Control Dashboard:** Clean, dedicated web dashboard (`dashboard.html`) to manage recipient lists, monitor live sending progress, and configure campaign settings.
- **💾 Persistent Local Storage:** Safely saves templates, logs, and queue states locally (`storage.js`) so progress isn't lost if interrupted.

---

## 📂 Project Architecture

```text
professor-Gmail-Sender-Agent/
├── assets/               # Icons, logos, and static UI resources
├── background.js         # Background service worker handling queue & time delays
├── dashboard.css         # Styling for the extension control dashboard
├── dashboard.html        # Main UI interface for managing outreach campaigns
├── dashboard.js          # Dashboard logic, campaign controls, and live status updates
├── gmail-content.js      # Content script that interacts directly with Gmail's DOM
├── manifest.json         # Chrome Extension Manifest (V3) configuration & permissions
├── proposal-editor.js    # Rich editor logic for crafting custom email proposals
├── storage.js            # Local storage wrapper for saving templates and campaign states
├── templates.js          # Pre-built outreach templates and dynamic formatting handlers
└── utils.js              # Helper functions (validators, timers, formatters)
