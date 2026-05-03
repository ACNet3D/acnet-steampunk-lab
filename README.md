# ACNET Steampunk Lab

> *3D-printed modular homelab combining networking, virtualization and integrated control in a steampunk-inspired design.*

---

## 🧠 Overview

ACNET Steampunk Lab is a compact, fully functional homelab built inside a custom 3D-printed rack, combining real infrastructure with a strong steampunk aesthetic.

Designed and built from scratch, this project integrates networking, virtualization and local control into a single standalone unit.

---

## 🔥 Highlights

* 🧱 Fully custom **3D-printed structure** (PETG + PLA)
* 🌐 Segmented network with **VLANs and WiFi SSIDs**
* 🖥️ **Proxmox host** running multiple services
* 🧰 Integrated **control node (Windows 11 + LCD)**
* 🎨 Steampunk design with **copper, matte black and neon accents**
* 🚫 Network-wide ad blocking with **Pi-hole**

---

## 📸 Preview

![Rack Front](images/rack_front.jpg)
![Rack Interior](images/rack_inside.jpg)
![LCD Control](images/lcd.jpg)

---

## 🏗️ Design & Manufacturing

* Designed in **Onshape**
* Developed with support from the **SHARE HORIZONS community**
* Printed using:

  * **Bambu Lab X1C**
  * **Bambu Lab P2S**

### Materials

* **PETG (black)** → structural base (heat resistant)
* **PLA (colors)** → front panels and aesthetic parts

Color palette:

* Matte black
* Copper
* Neon yellow
* Cyan blue

---

## 🧰 Hardware

From bottom to top:

* **Ubiquiti UniFi Express** (Firewall + WiFi 6 AP)
* **Ubiquiti USW Ultra 210W** (8-port switch)
* **Intel NUC i5-1240P**

  * 32GB RAM
  * 1TB NVMe
* **Cudy LT300 4G Router** (WiFi disabled)
* **LCD Display** (connected via USB-HDMI)

---

## 🌐 Network

* **VLAN 1 – Main**

  * SSID: `ACNET_HOMELAB`

* **VLAN 20 – IT**

  * Wired only (no WiFi)

* **VLAN 120 – Guest**

  * SSID: `ACNET_GUEST`

Features:

* VLAN segmentation
* WiFi separation
* Centralized routing via UniFi Express
* Ad blocking with Pi-hole

---

## 🖥️ Server (Proxmox)

Running on the Intel NUC:

* 🧱 **Pi-hole** (container)
* 📊 **Grafana** (container – planned)
* 🍏 **macOS VM**
* 🪟 **Windows 11 LTSC VM**

  * Direct output to LCD
  * Used as local control interface

---

## 🧪 Integrated Control Node

The lab includes a built-in control system:

* Windows 11 VM connected to:

  * LCD screen
  * External keyboard & mouse
* Enables **direct management from the rack itself**

---

## 🎓 Learning & Community

This project was developed as part of a personal learning journey in:

* 3D design (Onshape)
* Networking & segmentation
* Virtualization (Proxmox)

With inspiration and support from:

👉 SHARE HORIZONS
(YouTube link coming soon)

---

## 🚀 Future Improvements

* Grafana dashboards for monitoring
* More automation
* Improved cable management
* Version 2 of the rack design

---

## 📍 About

Built as a personal homelab and showcased at the **3D Printer Party**.

---

## ⭐ If you like it...

Feel free to star the repo or reach out!
