# LG Therma V – Home Assistant Modbus Integration

![LG Therma V Integration Screenshot](https://github.com/USER/REPO/assets/your-image-id-here.png)

A fully integrated **Home Assistant Modbus configuration** for the  
**LG Therma V R32 Monoblock heat pump**.  
This setup allows you to **read, visualize, and control** all major parameters via Modbus TCP.  
The YAML package is modular, optimized for Home Assistant 2025+, and has been extensively tested in real-world use.

---

## ✨ Features

✅ **Complete Modbus coverage**
- Includes all key registers (Input, Holding, Coil, Discrete Input)  
- Access to temperatures, pressures, flow rates, and system states  

✅ **Bidirectional control**
- Automatic synchronization between Home Assistant UI and Modbus registers  
- Real-time updates of target temperatures and operation modes  

✅ **User-friendly interface**
- Sliders (`input_number`) and dropdowns (`input_select`) for all key settings  
- Template-based sensors for readable operation states (normal mode, energy saving, etc.)  

✅ **Stable & future-proof**
- Compatible with Home Assistant 2024.10 – 2025.11  
- Clear modular design separating sensors, automations, and inputs  

---

## ⚙️ Requirements

| Component | Description |
|------------|-------------|
| **Hardware** | LG Therma V R32 Monoblock with Modbus TCP enabled |
| **Home Assistant** | Version ≥ 2024.10 (tested with 2025.10) |
| **Integration** | [Modbus Integration](https://www.home-assistant.io/integrations/modbus/) |
| **Network** | Heat pump accessible via IP and port (default: 502) |

---

## 🧩 Structure Overview

| Section | Purpose |
|----------|----------|
| `modbus:` | Connection and register definitions |
| `input_number:` | Adjustable setpoints (heating circuits, DHW target temps) |
| `input_select:` | Operation and control mode selectors |
| `template:` | Readable status sensors (energy modes, operation states) |
| `automation:` | Sync logic between Modbus and the Home Assistant UI |

---

## 🖥️ Example Dashboard

> Example Home Assistant dashboard (ApexCharts + Mushroom cards)

![Dashboard Example](https://github.com/USER/REPO/assets/your-dashboard-image-id.png)

---

## 🛠️ Installation

1. Copy the file `lg_heatpump.yaml` into your Home Assistant `packages` directory  
   *(e.g., `/config/packages/lg_heatpump.yaml`)*  
2. Enable the packages folder in your `configuration.yaml`:
   ```yaml
   homeassistant:
     packages: !include_dir_named packages




## Description
This package is for connecting and controlling an LG Therma V heat pump with Homeassistant via Modbus RTU.  

You will find all information [here](https://github.com/basti242/homeassistant_lg_therma_v_modbus/wiki).
 



