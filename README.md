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
* Desarrollo apoyado por la comunidad **SHARE HORIZONS**
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

* **Ubiquiti UniFi Express** (Firewall + WiFi 6)
* **Ubiquiti USW Ultra 210W** (switch)
* **Intel NUC i5-1240P**

  * 32GB RAM
  * 1TB NVMe
* **Router 4G Cudy LT300** (WiFi deshabilitado)
* **Pantalla LCD** (USB → HDMI)

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

👉 SHARE HORIZONS
(link YouTube próximamente)

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

It integrates networking, virtualization and local control into a single standalone unit.

---

## 🔥 Highlights

* 🧱 Fully custom **3D-printed structure**
* 🌐 Segmented network with **VLANs and SSIDs**
* 🖥️ **Proxmox host**
* 🧰 Integrated **control node (Windows + LCD)**
* 🎨 Steampunk aesthetic with neon accents
* 🚫 Network-wide ad blocking (Pi-hole)

---

## 🧰 Hardware

* Ubiquiti UniFi Express (Firewall + AP)
* Ubiquiti USW Ultra 210W
* Intel NUC i5-1240P (32GB / 1TB)
* Cudy LT300 4G Router (WiFi disabled)
* LCD display (USB-HDMI)

---

## 🌐 Network

* VLAN 1 – Main (`ACNET_HOMELAB`)
* VLAN 20 – IT (wired only)
* VLAN 120 – Guest (`ACNET_GUEST`)

---

## 🖥️ Server

* Pi-hole (container)
* Grafana (planned)
* macOS VM
* Windows 11 LTSC (local control)

---

## 📍 About

Showcased at the **3D Printer Party**.

---

## ⭐ If you like it

Feel free to star the repo!
