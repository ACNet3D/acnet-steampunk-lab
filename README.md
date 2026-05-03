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

---

## ⚡ Consumo estimado

El consumo total del ACNET Steampunk Lab depende principalmente de la carga del NUC, el uso de la pantalla LCD y la actividad de red.

### 🔌 Consumo por dispositivo (estimado)

| Equipo                  | Consumo aprox. | Nota                            |
| ----------------------- | -------------: | ------------------------------- |
| UniFi Express           | hasta **10 W** | dato fabricante                 |
| USW Ultra 210W          |        **8 W** | sin dispositivos PoE conectados |
| Intel NUC12WSK i5-1240P |    **15–45 W** | según carga de CPU y VMs        |
| Cudy LT300 4G           |      **3–8 W** | 3 W idle / hasta 8 W            |
| Pantalla LCD 7”         |      **4–8 W** | estimación típica               |
| Adaptador USB-HDMI      |      **1–3 W** | estimación                      |

---

### 📊 Consumo total

| Escenario           | Consumo estimado |
| ------------------- | ---------------: |
| Reposo / uso ligero |      **35–45 W** |
| Uso normal          |      **45–65 W** |
| Pico de carga       |      **75–90 W** |

> Valores estimados. Pendiente de validación con medidor real.

---

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

## ⚡ Estimated Power Consumption

The total power consumption of the ACNET Steampunk Lab mainly depends on NUC load, LCD usage and network activity.

### 🔌 Per-device estimation

| Device                  | Approx. Consumption | Notes                  |
| ----------------------- | ------------------: | ---------------------- |
| UniFi Express           |      up to **10 W** | manufacturer data      |
| USW Ultra 210W          |             **8 W** | without PoE devices    |
| Intel NUC12WSK i5-1240P |         **15–45 W** | depends on CPU/VM load |
| Cudy LT300 4G           |           **3–8 W** | 3 W idle / up to 8 W   |
| 7” LCD Display          |           **4–8 W** | typical estimate       |
| USB-HDMI Adapter        |           **1–3 W** | estimated              |

---

### 📊 Total consumption

| Scenario           | Estimated Consumption |
| ------------------ | --------------------: |
| Idle / light usage |           **35–45 W** |
| Normal usage       |           **45–65 W** |
| Peak load          |           **75–90 W** |

> Estimated values. Pending validation with a real power meter.

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
