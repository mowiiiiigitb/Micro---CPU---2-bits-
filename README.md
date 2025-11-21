------Micro-CPU de 2 Bits – Calculadora en Protoboard------

Este proyecto implementa una calculadora funcional de 2 bits basada en una placa RP2040 Zero, montada en un protoboard y programada en MicroPython.
El objetivo es simular el comportamiento básico de una Unidad Central de Procesamiento (CPU) mediante hardware real.

---Características Principales---

Simulación del ciclo de instrucción:
- Fetch
- Decode
- Execute
- Write-Back

Banderas de estado:
- Zero
- Negative

Operaciones aritméticas con operandos de 0 a 3 (+, − y =).
Resultado mostrado en un display de 7 segmentos.
Indicadores LED para etapas de la CPU y estados.

---Hardware Utilizado---
- RP2040 Zero (MicroPython)
- Protoboard
- 7 botones (4 dígitos + 3 operaciones)
- 6 LEDs (ciclo CPU + banderas)
- 7 resistencias (220–330 Ω)
- Display de 7 segmentos (cátodo común)
- Jumpers hembra-macho
- Cable UTP / protoboard
- Cable USB-C

---Entorno de Desarrollo---

- Lenguaje: MicroPython
- IDE: Thonny
- Botones: Configuración Pull-Up interna

---Funcionamiento---

- El usuario ingresa el primer operando (0–3).
- Selecciona la operación (+ o −).
- Ingresa el segundo operando.
- Presiona el botón "=" para ejecutar.
- La placa recorre las fases de la CPU (indicadas con LEDs).
- Se activan las banderas (Zero o Negative si corresponde).
- El resultado se muestra en el display de 7 segmentos.

---Objetivo Educativo---

Comprender cómo una CPU procesa instrucciones utilizando un modelo físico y simplificado, visualizando cada fase mediante LEDs y ejecutando 
operaciones reales con hardware digital.
