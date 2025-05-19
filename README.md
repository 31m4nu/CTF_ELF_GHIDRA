# CTF_ELF_GHIDRA

Repositorio con un binario ELF estático diseñado para practicar análisis estático y reversing con Ghidra. Contiene 4 retos progresivos que simulan técnicas utilizadas por binarios maliciosos reales, como ofuscación de datos, exfiltración encubierta, transformación bitwise y ocultamiento en memoria.

Este proyecto está dirigido a quienes desean aprender a utilizar Ghidra para análisis de malware, desarrollar criterio de análisis, y entrenarse con ejemplos funcionales y realistas sin riesgo de ejecutar código malicioso real.

---

## 🧠 Objetivo

El objetivo es desarrollar habilidades de análisis estático usando Ghidra, comprender estructuras ELF, manipulación de secciones como `.rodata`, y seguir el flujo de ejecución para descubrir información oculta. Cada reto dentro del binario representa una técnica distinta comúnmente observada en reversing, CTFs y malware real.

---

## 📦 Contenido del repositorio

- `CTF_GHIDRA_v1`: Binario ELF estático con 4 retos.
- `banderas.txt`: Archivo vacío para registrar cada bandera encontrada, una por línea, en orden.
- `README_CTF_GHIDRA_v1.txt`: Instructivo completo para ejecutar el reto.
- `estego.png`: Imagen utilizada en uno de los retos como parte de la simulación de datos ocultos.

---

## 🛠 Requisitos

- Linux x86_64 (para ejecutar el binario ELF)
- [Ghidra](https://ghidra-sre.org/) (v10 o superior recomendada)
- Herramientas básicas:
  - `strings`
  - `base64`
  - `echo`
  - Un visor de imágenes (`xdg-open`, `feh`, `eog`, etc.)

---

## 🚀 Cómo comenzar

1. Clona el repositorio:
   ```bash
   git clone https://github.com/31m4nu/CTF_ELF_GHIDRA.git
   cd CTF_ELF_GHIDRA
   ```

2. Dale permisos de ejecución al binario:
   ```bash
   chmod +x CTF_GHIDRA_v1
   ./CTF_GHIDRA_v1
   ```

3. Lee las instrucciones simuladas. Analiza el binario en Ghidra para encontrar los datos ofuscados.

4. Coloca las banderas descubiertas, una por línea, en el archivo `banderas.txt`.

5. Comparte el conocimiento!!!

---

## ❗ Advertencia

Este binario no ejecuta acciones maliciosas reales. Todas las instrucciones que simulan comandos como `curl`, `base64`, o `fopen()` son solo `printf()` o estructuras pasivas. Está diseñado para fines educativos.

Aunque este binario ha sido creado con fines educativos y no contiene comportamientos maliciosos reales, se trata de un archivo ELF ejecutable que simula técnicas de ocultamiento, por lo que su ejecución debe realizarse únicamente en entornos controlados, como máquinas virtuales o laboratorios aislados.
No se recomienda ejecutar archivos ELF desconocidos directamente sobre sistemas de uso diario o producción.
Antes de cualquier análisis dinámico, se recomienda verificar que el hash del archivo binario coincida con el proporcionado, asegurando así su integridad y origen legítimo.
Hash oficial del binario:
Nombre del archivo: CTF_GHIDRA_v1
SHA256: 65d231c0da1ed6108b4a6f27a5aeb8e9fd0f550df408c2885029e8788977ad37

---

## 🧑‍💻 Autor

Creado por Manuel Eduardo Flores Cruz  
📧 31m4numx@gmail.com  
🔗 [linkedin.com/in/31m4nu](https://www.linkedin.com/in/31m4nu)

---

¡Explora, rompe y aprende!
