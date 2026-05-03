# ACNET Steampunk Lab

> *Homelab modular impreso en 3D que combina red, virtualización y control integrado en un diseño inspirado en el steampunk.*

---

🇪🇸 Español | 🇬🇧 English

---

# 🇪🇸 Español

## 🧠 Descripción

ACNET Steampunk Lab es un homelab compacto y completamente funcional, construido dentro de un rack diseñado e impreso en 3D, combinando infraestructura real con una estética steampunk.

Este proyecto integra red, virtualización y control local en una única unidad autónoma.

---

## 🔥 Características

* 🧱 Estructura **100% diseñada e impresa en 3D** (PETG + PLA)
* 🌐 Red segmentada con **VLANs y SSIDs**
* 🖥️ **Servidor Proxmox** con múltiples servicios
* 🧰 Nodo de **control integrado (Windows 11 + LCD)**
* 🎨 Diseño steampunk con **cobre, negro mate y colores neón**
* 🚫 Bloqueo de publicidad con **Pi-hole**

---

## 📸 Vista general

![Frontal](images/rack_front.jpg)
![Interior](images/rack_inside.jpg)
![Pantalla](images/lcd.jpg)

---

## 🏗️ Diseño e Impresión

* Diseñado en **Onshape**
* Desarrollo apoyado por la comunidad **[SHARE HORIZONS](https://sharehorizons.com/)**
* Impreso con:

  * **Bambu Lab X1C**
  * **Bambu Lab P2S**

### Materiales

* **PETG negro** → base estructural (resistencia térmica)
* **PLA colores** → frontales y estética

Colores:

* Negro mate
* Cobre
* Amarillo neón
* Azul cian

---

## 🧰 Hardware

De abajo a arriba:

* **Ubiquiti UniFi Express**
  Firewall + punto de acceso WiFi 6

* **Ubiquiti USW Ultra 210W**
  Switch gestionable de 8 puertos

* **Intel NUC12WSK (i5-1240P)**

  * 32GB RAM
  * 1TB NVMe
  * Host de virtualización (Proxmox)

* **Cudy LT300 4G Router**

  * Conectividad LTE
  * WiFi deshabilitado (uso exclusivo como backup WAN)

* **Pantalla LCD 7”**
  👉 https://es.aliexpress.com/item/1005002570180532.html

  * Conectada mediante adaptador USB → HDMI
  * Usada como interfaz local del sistema


## 🌐 Red

* **VLAN 1 – Principal**

  * SSID: `ACNET_HOMELAB`

* **VLAN 20 – IT**

  * Solo cable (sin WiFi)

* **VLAN 120 – Invitados**

  * SSID: `ACNET_GUEST`

Funciones:

* Segmentación por VLAN
* Separación de redes WiFi
* Enrutamiento centralizado
* Bloqueo de publicidad con Pi-hole

---

## 🖥️ Servidor (Proxmox)

En el NUC:

* 🧱 **Pi-hole** (contenedor)
* 📊 **Grafana** (contenedor – en preparación)
* 🍏 **macOS VM**
* 🪟 **Windows 11 LTSC**

  * Salida directa a la pantalla LCD
  * Nodo de control del sistema

---

## 🧪 Nodo de control integrado

El propio rack permite su gestión directa:

* Windows 11 conectado a:

  * Pantalla LCD
  * Teclado y ratón
* Control completo sin necesidad de otro equipo

---

## 🎓 Aprendizaje y comunidad

Proyecto desarrollado como parte de aprendizaje en:

* Diseño 3D (Onshape)
* Redes y segmentación
* Virtualización (Proxmox)

Con apoyo de:

👉 **[SHARE HORIZONS](https://sharehorizons.com/)**

---

## 🚀 Mejoras futuras

* Dashboards en Grafana
* Automatización
* Mejora de cableado
* Nueva versión del diseño

---

## 📍 Contexto

Proyecto presentado en la **3D Printer Party**.

---

# 🇬🇧 English

## 🧠 Overview

ACNET Steampunk Lab is a compact and fully functional homelab built inside a custom 3D-printed rack, combining real infrastructure with a steampunk-inspired design.

This project integrates networking, virtualization and local control into a single standalone unit.

---

## 🔥 Highlights

* 🧱 Fully custom **3D-printed structure** (PETG + PLA)
* 🌐 Segmented network with **VLANs and SSIDs**
* 🖥️ **Proxmox server** running multiple services
* 🧰 Integrated **control node (Windows 11 + LCD)**
* 🎨 Steampunk design with **copper, matte black and neon accents**
* 🚫 Network-wide ad blocking with **Pi-hole**

---

## 📸 Preview

![Front](images/rack_front.jpg)
![Interior](images/rack_inside.jpg)
![LCD](images/lcd.jpg)

---

## 🏗️ Design & Manufacturing

* Designed in **Onshape**
* Developed with support from the **[SHARE HORIZONS](https://sharehorizons.com/)** community
* Printed using:

  * **Bambu Lab X1C**
  * **Bambu Lab P2S**

### Materials

* **Black PETG** → structural base (heat resistant)
* **Colored PLA** → front panels and aesthetic parts

Color palette:

* Matte black
* Copper
* Neon yellow
* Cyan blue

---

## 🧰 Hardware

From bottom to top:

* **Ubiquiti UniFi Express**
  Firewall + WiFi 6 access point

* **Ubiquiti USW Ultra 210W**
  Managed 8-port switch

* **Intel NUC12WSK (i5-1240P)**

  * 32GB RAM
  * 1TB NVMe
  * Virtualization host (Proxmox)

* **Cudy LT300 4G Router**

  * LTE connectivity
  * WiFi disabled (used as backup WAN)

* **7” LCD Display**
  👉 https://es.aliexpress.com/item/1005002570180532.html

  * Connected via USB → HDMI adapter
  * Used as local control interface


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
* Centralized routing
* Ad blocking with Pi-hole

---

## 🖥️ Server (Proxmox)

Running on the Intel NUC:

* 🧱 **Pi-hole** (container)
* 📊 **Grafana** (container – planned)
* 🍏 **macOS VM**
* 🪟 **Windows 11 LTSC**

  * Direct output to the LCD
  * Used as local control node

---

## 🧪 Integrated Control Node

The lab includes a built-in control system:

* Windows 11 connected to:

  * LCD display
  * External keyboard & mouse
* Enables full **local management directly from the rack**

---

## 🎓 Learning & Community

This project was developed as part of a learning journey in:

* 3D design (Onshape)
* Networking & segmentation
* Virtualization (Proxmox)

With support from:

👉 **[SHARE HORIZONS](https://sharehorizons.com/)**

---

## 🚀 Future Improvements

* Grafana dashboards
* Automation
* Improved cable management
* Version 2 of the rack

---

## 📍 Context

Showcased at the **3D Printer Party**.

---

## ⭐ If you like it

Feel free to star the repo!
