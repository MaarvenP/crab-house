# crab-house
# 🦀 Vertical Mudcrab Farm (Tower System)

A Raspberry Pi based monitoring and control system for a vertical mudcrab grow out farm.  
Built to track water quality across stacked trays, log data, and alert you before conditions drift.

---

## What this project does

- Monitors water quality in each vertical tier
- Logs sensor data to a local database
- Shows live readings on a simple dashboard
- Flags risky conditions (example: pH crash, high turbidity)
- Designed around a drawer / tray tower that drains down into a sump

---

## Why vertical farming for mudcrab

Vertical trays let you:
- Use space efficiently
- Keep crabs separated to reduce cannibalism
- Run one shared water loop with staged filtration

This repo focuses on the **electronics + software layer** that sits on top of that farm.

---

## Hardware used

**Controller**
- Raspberry Pi 5

**Sensors (from our build)**
1. **pH sensor**: DFRobot SEN0169  
   Used to track acidity / alkalinity in the recirculating loop.
2. **Temperature sensor**: DS18B20 (waterproof)  
   Used to track tray and sump temperatures.
3. **Turbidity sensor**: “PPM Turbidity Gravity Analog Sensor for Arduino”  
   Used as a low cost indicator of suspended solids, waste buildup, or biofouling.

**Hydraulics**
- Sump tank (53 L)
- Pump feeding top tray
- Gravity overflow between trays down to sump
- Single valve on pump output for flow tuning

---
