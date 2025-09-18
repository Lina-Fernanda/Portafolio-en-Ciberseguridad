# 📂 01 – Fundamentos de Ciberseguridad  

En esta carpeta encontrarás mis primeros laboratorios y prácticas básicas de ciberseguridad.  
El objetivo es reforzar conceptos fundamentales y documentar ejercicios prácticos que sirven de base para niveles más avanzados.  

---
Resultados esperados:

Detectar servicios activos (ejemplo: SSH, HTTP, MySQL).

Documentar posibles vulnerabilidades relacionadas con versiones obsoletas.

📄 Archivo: nmap-practica.md

🌐 Análisis de Tráfico con Wireshark

Objetivo: Capturar tráfico de red y filtrar protocolos específicos.

Herramienta: Wireshark

Ejemplo de filtros usados:

http → tráfico web

tcp.port == 22 → conexiones SSH

Resultados esperados:

Identificación de sesiones activas.

Posible detección de patrones anómalos.

📄 Archivo: wireshark-practica.md

🖥️ Scripts Básicos

Objetivo: Automatizar pequeñas tareas de seguridad.

Ejemplo de script en Bash:

#!/bin/bash
echo "Escaneo rápido de puertos abiertos"
nmap -F $1


Resultado: Escaneo rápido de puertos al ejecutar:

./puertos.sh 192.168.1.10


📄 Archivo: script-puertos.sh

✅ Próximos pasos

Completar prácticas adicionales con tcpdump.

Documentar hallazgos en informes más detallados.

Subir capturas de pantalla de los laboratorios (cuando sea posible).

✨ Esta carpeta refleja mis primeros pasos prácticos en seguridad informática.
## 🔍 Escaneo de Redes con Nmap  

- **Objetivo:** Identificar puertos abiertos y servicios en ejecución en un entorno controlado.  
- **Herramienta:** Nmap  
- **Comando usado:**  
  ```bash
  nmap -sV -T4 192.168.1.10

