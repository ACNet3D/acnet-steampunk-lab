# ACNET Steampunk Lab

> *Homelab modular impreso en 3D que combina red, virtualización y control integrado en un diseño inspirado en el steampunk.*
>
> <p align="center">
  <img src="logo.png" width="400"/>
</p>

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

<p align="center">
  <img src="rack_front.jpg" width="400"/>
</p>


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
