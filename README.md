# WebsiteBlocker

📛 Simple Site Blocker Chrome Extension
Block distracting or unwanted websites effortlessly with this lightweight Chrome extension. Customize the blocklist to suit your productivity or parental control needs.

🚀 Features
Blocks access to specific domains (e.g., Facebook, YouTube, Instagram)

Uses Chrome's declarativeNetRequest API for fast performance

Lightweight, no background scripts

Easy to customize list of blocked websites

🧱 Installation
Clone or download this repository

Open chrome://extensions/ in your browser

Enable Developer Mode (toggle in the top right)

Click Load unpacked

Select the extension folder containing manifest.json and rules.json

🔒 Customizing Blocked Websites
Edit rules.json to add or remove domains. Each domain has its own rule object:

json
{
  "id": 4,
  "priority": 1,
  "action": { "type": "block" },
  "condition": {
    "urlFilter": "*://*.reddit.com/*",
    "resourceTypes": ["main_frame"]
  }
}
Make sure each rule has a unique id.

📁 File Structure
plaintext
📂 site-blocker-extension
├── manifest.json
└── rules.json
💡 Future Ideas
Time-based blocking

User interface to manage blocklist

Sync settings across devices

📄 License
This project is licensed under the MIT License.
