# 📋 Changelog

Todos los cambios notables en este proyecto serán documentados aquí.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es/1.0.0/).

---

## [2.0.0] — 2024-12-01 — Community Edition 🎉

### Añadido
- Playbook HTML interactivo con dark mode y botones de copia
- Barra de navegación sticky con acceso rápido a todas las secciones
- Tabla de referencia de puertos con qué hacer al ver cada uno
- Árbol de decisión visual por puerto abierto
- Sección completa de **msfvenom**: staged vs non-staged, todos los formatos
- Sección completa de **Pivoting**: autoroute, portfwd, socks proxy, proxychains, rutas manuales
- **Windows PrivEsc**: UAC bypass con UACME, Token Impersonation con Incognito
- **Mimikatz/Kiwi** desde Meterpreter: creds_all, lsa_dump_sam
- **Pass-the-Hash** con psexec y crackmapexec
- IIS WebDAV completo: davtest, cadaver, payload ASP, brute-force
- Apache Tomcat: payload WAR, MSF automatizado
- Fping y ping sweep bash script
- Referencia completa de wordlists con rutas exactas en Kali
- Recursos curados de la comunidad (syselement, dev-angelist, nmmorette, iabdullah215)
- Consejos reales de personas que aprobaron el eJPTv2
- CONTRIBUTING.md para guiar contribuciones de la comunidad
- GitHub Pages ready

### Mejorado
- Flujo de scanning: rápido → completo → detallado (3 pasos)
- Sección SMB: añadido crackmapexec y MSF modules
- Sección HTTP: añadido ffuf, HTTP verbs check, nmap http-enum
- Hydra: añadidos MySQL, más ejemplos reales con flags explicados
- John the Ripper: añadido unshadow, formatos, reglas

---

## [1.0.0] — 2024-11-01 — Initial Release

### Añadido
- Metodología R·S·E·G·P (Recon, Scanning, Enumeration, Gaining, Post-expl)
- Fase 1 Recon: orientación en red, nmap ping sweep, netdiscover
- Fase 2 Scanning: nmap básico y con scripts
- Fase 3 Enumeration: SMB, FTP, HTTP, SSH, SMTP, MySQL
- Fase 4 Gaining Access: exploits comunes, brute force con Hydra
- Fase 5 Post-Exploitation: enumeración básica Linux y Windows
- Escalada de privilegios básica: sudo -l, SUID, cron jobs
- Web attacks: SQLi manual, SQLMap, file upload bypass, XSS
- Reverse shells: bash, python, php, netcat, PowerShell
