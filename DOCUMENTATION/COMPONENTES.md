# 📦 COMPONENTES — Calculadora con Ciclo de Instrucción (RP2040 Zero)

Este documento detalla los elementos de hardware utilizados en el proyecto.

---

## 🖥 1. Unidad de Control
- **1x RP2040 Zero**  
  - Compatible con MicroPython  
  - Incluye un NeoPixel RGB integrado

---

## 🔘 2. Entradas (Botones)
- **4x Botones** para los dígitos 0–3
- **1x Botón** para suma “+”
- **1x Botón** para resta “–”
- **1x Botón** para igual “=”

Total: **7 botones**

Todos usan **pull-up interno**, sin resistencias externas.

---

## 💡 3. Indicadores Visuales
- **4 LEDs** del ciclo CPU:  
  - Fetch  
  - Decode  
  - Execute  
  - Write-Back
- **2 LEDs** de banderas:  
  - Zero  
  - Negative
- **1 NeoPixel (LED RGB integrado)** usado para Overflow

Total: **7 LEDs + 1 NeoPixel**

---

## 🔌 4. Resistencias
- **7 resistencias de 220Ω–330Ω** (para cada LED excepto el NeoPixel)

---

## 🟣 5. Display
- **1 Display de 7 segmentos (Cátodo Común)**  
  Controlado por los GPIO **13,14,15,26,27,28,29**.

---

## 🧵 6. Cableado y Prototipado
- **1 Protoboard grande**
- **Cables jumper hembra–macho**
- **Cables jumper macho–macho**
- **Cables UTP / puenteado**

---

## 🔌 7. Alimentación
- **1 Cable USB-C**
- Voltaje operativo del sistema: **3.3V**

---

## 🛠 8. Entorno de Desarrollo
- Lenguaje: **MicroPython**  
- IDE recomendado: **Thonny**  

