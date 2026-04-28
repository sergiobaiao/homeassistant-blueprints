# 🔵 Home Assistant Bluetooth Blueprints

Repository dedicated to **advanced Bluetooth-based blueprints for Home Assistant**, focused on reliability, performance, and flexibility.

## 📦 Purpose

Provide reusable blueprints for Bluetooth devices, enabling:

- Fast configuration via Home Assistant UI
- Event-driven automations
- Reduced YAML duplication

---

## 🚀 How to Use

1. Go to:
   **Settings → Automations & Scenes → Blueprints**

2. Click:
   **Import Blueprint**

3. Paste the blueprint URL or upload the `.yaml` file

4. Create an automation using the blueprint

---

## 📁 Available Blueprints

### 🎛️ Lutron Pico (5 Buttons – Event-Based)

**File:** `pico.yaml`

Blueprint for Lutron Pico remotes using event entities:

- Supports up to 5 buttons
- Independent actions per button
- Compatible with Home Assistant `event.*` entities
- Safe execution (prevents loops and invalid triggers)

#### 🔧 Configuration

You will need to provide:

- Event entity for each button
- Action for each button

#### 💡 Typical Use Cases

- Lighting control
- Scene activation
- Multi-device automations

---

## 🧠 Best Practices

- ✅ Always filter by `entity_id`
- ✅ Use `mode: single` or `restart` appropriately
- ✅ Enable logging for debugging when needed

---

## 🐞 Troubleshooting

### 🔁 Automation Loop / High CPU Usage

If you notice:

- High CPU usage
- Repeated logs in short intervals
- Automations triggering continuously

👉 Check if the blueprint is listening to generic/global events.

---

## 📌 Roadmap

- [ ] Select a device and automatically populate it's entities below (If HA ever allows this)
- [ ] Optional advanced logging

---

## 🤝 Contributing

Pull requests are welcome!

Suggested contributions:

- Performance improvements
- Bug fixes

---

## 📄 License

MIT License

---

## 👨‍💻 Author

Sérgio Baião  
GitHub: https://github.com/sergiobaiao

---

## ⭐ Notes

These blueprints are designed with **stability and performance in mind**, avoiding common pitfalls such as automation loops that can crash or freeze Home Assistant.
