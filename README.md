Here’s a polished and professional `README.md` file for your **WebsiteBlocker** Chrome extension:

---

````markdown
# 🚫 WebsiteBlocker

A lightweight Chrome extension to block distracting or unwanted websites. Ideal for productivity, parental control, or simply reclaiming your focus online.

## 🚀 Features

- 🔒 **Block access to specific domains**  
  Easily block websites like Facebook, YouTube, Instagram, and more.

- ⚡ **Fast and Secure**  
  Powered by Chrome's `declarativeNetRequest` API — no background scripts needed.

- 📦 **Minimal and Efficient**  
  Lightweight with zero bloat; built for speed and privacy.

- 🛠️ **Customizable Blocklist**  
  Configure blocked websites directly through a `rules.json` file.

---

## 🧱 Installation

1. **Clone or download** this repository to your local machine.

2. Open `chrome://extensions/` in your Chrome browser.

3. **Enable Developer Mode** (toggle in the top right corner).

4. Click **"Load unpacked"**.

5. Select the extension folder that contains both `manifest.json` and `rules.json`.

---

## 🔧 Customizing Blocked Websites

To block additional websites:

1. Open the `rules.json` file.
2. Add a new rule using this format:

```json
{
  "id": 4,
  "priority": 1,
  "action": { "type": "block" },
  "condition": {
    "urlFilter": "*://*.reddit.com/*",
    "resourceTypes": ["main_frame"]
  }
}
````

📌 **Note:** Each rule must have a unique `"id"` to avoid conflicts.

---

## 📁 File Structure

```
📂 site-blocker-extension
├── manifest.json
└── rules.json
```

---

## 💡 Future Enhancements

* ⏱️ Time-based site blocking (e.g., block during work hours)
* 🧩 User interface for managing the blocklist dynamically
* 🔄 Sync rules across multiple devices using Chrome Sync

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

```

---

Let me know if you’d like me to generate the actual `manifest.json` and `rules.json` templates too.
```
