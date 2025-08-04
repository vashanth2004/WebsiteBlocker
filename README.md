🚫 WebsiteBlocker
A lightweight Chrome extension to block distracting or unwanted websites. Ideal for productivity, parental control, or simply reclaiming your focus online.

🚀 Features
🔒 Block access to specific domains (e.g., Facebook, YouTube, Instagram)

⚡ Powered by Chrome's declarativeNetRequest API for performance and security

📦 Minimal and efficient — no background scripts needed

🛠️ Fully customizable blocklist via rules.json

🧱 Installation
Clone or download this repository.

Open chrome://extensions/ in your Chrome browser.

Enable Developer Mode (toggle in the top right corner).

Click Load unpacked.

Select the extension folder containing manifest.json and rules.json.

🔧 Customizing Blocked Websites
To block additional websites:

Open the rules.json file.

Add a new rule for each domain using this format:

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
📌 Each rule must have a unique "id" to avoid conflicts.

📁 File Structure
plaintext
📂 site-blocker-extension
├── manifest.json
└── rules.json
💡 Future Enhancements
⏱️ Time-based site blocking (e.g., block during work hours)

🧩 User interface for managing the blocklist dynamically

🔄 Sync rules across multiple devices

📄 License
This project is licensed under the MIT License.
