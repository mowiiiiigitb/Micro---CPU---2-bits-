# 📌 PINOUT_FINAL — Calculadora de 1 Dígito con Ciclo de Instrucción (RP2040 Zero)

Este documento describe todos los pines GPIO utilizados en el proyecto según el código final en MicroPython.

---

# 🟢 1. Pines de Entrada — Botones (con Pull-Up Interno)

| Función | GPIO |
|--------|------|
| Botón Dígito 0 | **GPIO0** |
| Botón Dígito 1 | **GPIO1** |
| Botón Dígito 2 | **GPIO2** |
| Botón Dígito 3 | **GPIO3** |
| Botón “+” | **GPIO4** |
| Botón “–” | **GPIO5** |
| Botón “=” | **GPIO6** |

Todos configurados como entradas con:

```python
machine.Pin.IN, machine.Pin.PULL_UP
```

---

# 🔵 2. LEDs del Ciclo de Instrucción (Salidas)

| LED / Fase CPU | GPIO |
|----------------|------|
| LED Fetch | **GPIO7** |
| LED Decode | **GPIO8** |
| LED Execute | **GPIO9** |
| LED Write-Back | **GPIO10** |

---

# 🔴 3. Banderas (FLAGS)

| Bandera | GPIO | Descripción |
|---------|------|-------------|
| Zero | **GPIO11** | Se enciende si resultado = 0 |
| Negative | **GPIO12** | Se enciende si resultado < 0 |
| Overflow | **GPIO16 (NeoPixel)** | Se ilumina en rojo si hay overflow |

---

# 🌈 4. NeoPixel Integrado

| Componente | GPIO | Función |
|------------|------|---------|
| LED RGB integrado | **GPIO16** | Indica overflow (rojo) |

Inicialización:

```python
neopixel.NeoPixel(machine.Pin(16), 1)
```

---

# 🟣 5. Display de 7 Segmentos (Cátodo Común)

| Segmento | GPIO |
|----------|------|
| a | **13** |
| b | **14** |
| c | **15** |
| d | **26** |
| e | **27** |
| f | **28** |
| g | **29** |

---

# ✔ Resumen Final

- **7 botones** → GPIO0–GPIO6  
- **4 LEDs CPU** → GPIO7–GPIO10  
- **2 LEDs FLAGS** → GPIO11–GPIO12  
- **Overflow LED (RGB)** → GPIO16  
- **Display 7 segmentos** → GPIO13–15 + GPIO26–29  
- Botones con **pull-up interno**
