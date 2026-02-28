<div align="center">

# 🎯 eJPTv2 — Playbook Maestro

[![eJPTv2](https://img.shields.io/badge/Certificación-eJPTv2-red?style=for-the-badge&logo=target&logoColor=white)](https://ine.com/learning/certifications/internal/elearnsecurity-junior-penetration-tester-cert)
[![Idioma](https://img.shields.io/badge/Idioma-Español-blue?style=for-the-badge&logo=googletranslate&logoColor=white)](#)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-green?style=for-the-badge)](#-licencia)
[![PRs Welcome](https://img.shields.io/badge/PRs-Bienvenidos-brightgreen?style=for-the-badge&logo=github)](#-cómo-contribuir)
[![Stars](https://img.shields.io/github/stars/TU_USUARIO/eJPTv2-Playbook?style=for-the-badge&color=yellow&logo=github)](../../stargazers)
[![Forks](https://img.shields.io/github/forks/TU_USUARIO/eJPTv2-Playbook?style=for-the-badge&color=orange&logo=github)](../../forks)

<br/>

**El playbook interactivo más completo en español para aprobar el eJPTv2.**  
Metodología estructurada + comandos listos para copiar y pegar + sabiduría colectiva de la comunidad.

<br/>

[🚀 Ver Playbook Online](https://TU_USUARIO.github.io/eJPTv2-Playbook) · [🐛 Reportar Error](../../issues/new?template=bug_report.md) · [💡 Sugerir Mejora](../../issues/new?template=feature_request.md) · [🤝 Contribuir](CONTRIBUTING.md)

<br/>

> ⭐ **Si este recurso te ayudó a aprobar el eJPTv2, dale una estrella — ayuda a que más personas lo encuentren.**

</div>

---

## 📋 Tabla de contenidos

- [¿Qué es esto?](#-qué-es-esto)
- [Vista previa](#-vista-previa)
- [Contenido del Playbook](#-contenido-del-playbook)
- [Cómo usar](#-cómo-usar)
- [Herramientas cubiertas](#️-herramientas-cubiertas)
- [La Metodología](#-la-metodología)
- [Consejos de aprobados](#-consejos-de-aprobados)
- [Cómo contribuir](#-cómo-contribuir)
- [Roadmap](#-roadmap)
- [Créditos](#-créditos)
- [Disclaimer](#️-disclaimer)
- [Licencia](#-licencia)

---

## 🌟 ¿Qué es esto?

Este repositorio contiene un **playbook HTML interactivo y standalone** para preparar el examen **eJPTv2 (eLearnSecurity Junior Penetration Tester v2)** de INE Security.

**¿Para quién es?**

| Perfil | Cómo te ayuda |
|--------|---------------|
| 🎓 Estudiantes del PTSv2 (INE) | Complementa el curso con comandos listos |
| 🧪 Practicantes de CTFs | Metodología estructurada para no perderte |
| 🔰 Personas que empiezan en pentesting | Referencia rápida de herramientas y técnicas |
| 🏆 Los que van a rendir el examen | Cheatsheet open-book para tener a mano |

---

## 👀 Vista previa

```
┌─────────────────────────────────────────────────────────────────┐
│  🎯 eJPTv2 — Playbook Maestro              [v2.0 Community Ed.] │
├──────────────────────────────────────────────────────────────────│
│  🧠 Metodología │ 🔍 Recon │ 🔭 Scan │ 🗂 Enum │ ⚔️ Exploits... │
├──────────────────────────────────────────────────────────────────│
│                                                                   │
│   R · S · E · G · P                                              │
│   RECON → SCAN → ENUM → GAINING → POST-EXPL                     │
│                                                                   │
│   [Copy] nmap -p- -T4 <TARGET_IP> -oN all_ports.txt             │
│   [Copy] gobuster dir -u http://<IP> -w wordlist.txt             │
│   [Copy] hydra -L users.txt -P rockyou.txt ssh://<IP>            │
│                                                                   │
└──────────────────────────────────────────────────────────────────┘
```

> 📸 Puedes ver el playbook en vivo en: `https://TU_USUARIO.github.io/eJPTv2-Playbook`

---

## 📖 Contenido del Playbook

<details>
<summary><b>🧠 Metodología R·S·E·G·P</b> — El framework mental central</summary>

- Mnemónico visual para recordar el orden
- Árbol de decisión por puerto abierto
- Reglas de oro de quienes aprobaron
</details>

<details>
<summary><b>🔍 FASE 1 — Reconnaissance</b></summary>

- Orientación en la red (`ip a`, `ip route`, `/etc/hosts`)
- Descubrimiento de hosts: `nmap`, `fping`, `netdiscover`, ping sweep bash
</details>

<details>
<summary><b>🔭 FASE 2 — Scanning</b></summary>

- Flujo de 3 pasos: rápido → completo → detallado
- Scans especializados: vuln, OS, UDP, EternalBlue, HeartBleed
- Tabla de puertos: qué esperar de cada uno
</details>

<details>
<summary><b>🗂️ FASE 3 — Enumeration</b></summary>

- **SMB**: enum4linux, smbclient, smbmap, crackmapexec, MSF modules
- **FTP**: anonymous login, comandos internos, banner grabbing
- **HTTP/HTTPS**: whatweb, nikto, gobuster, dirb, ffuf, HTTP verbs, WPScan
- **SSH / SMTP / MySQL / WinRM / RDP**: comandos y scripts específicos
</details>

<details>
<summary><b>⚔️ FASE 4 — Gaining Access</b></summary>

- CVEs más comunes: EternalBlue, vsftpd 2.3.4, Shellshock, BlueKeep, Log4Shell
- IIS WebDAV: davtest, cadaver, payload ASP, MSF automatizado
- Apache Tomcat: payload WAR, panel manager, MSF
- psexec, Pass-the-Hash con crackmapexec
</details>

<details>
<summary><b>💣 msfvenom — Generación de Payloads</b></summary>

- Staged (`/`) vs Non-Staged (`_`) explicado
- Windows: .exe x86/x64, ASP, ASPX, WAR
- Linux: ELF x86/x64, PHP, JSP
- Encoding para evasión básica
- Cómo transferir payloads al target
</details>

<details>
<summary><b>🐉 Metasploit Framework</b></summary>

- Comandos esenciales: search, use, sessions, workspaces
- Meterpreter: info, navegación, shell, migration, hashdump
- Kiwi/Mimikatz: dump de credenciales
- Shell to Meterpreter upgrade
</details>

<details>
<summary><b>🏴 FASE 5 — Post-Exploitation</b></summary>

- **Linux**: estabilizar shell, enumeración, buscar flags, LinPEAS
- **Windows**: systeminfo, buscar archivos, listar drives, WinPEAS
</details>

<details>
<summary><b>⬆️ Privilege Escalation</b></summary>

- **Linux**: sudo -l, SUID binaries, cron jobs, contraseñas en configs, kernel exploits, SSH keys
- **Windows**: UAC bypass (UACME), Token Impersonation (Incognito), kernel exploits
- MSF: `local_exploit_suggester` automático
</details>

<details>
<summary><b>🔀 Pivoting — Llegar a redes ocultas</b></summary>

- Autoroute + Socks Proxy + proxychains
- Port forwarding con `portfwd`
- Rutas manuales con `ip route add`
- ARP Spoofing (MitM)
</details>

<details>
<summary><b>🌐 Web Application Attacks</b></summary>

- SQLi manual + SQLMap completo (GET, POST, request file, os-shell)
- File Upload bypass: extensiones, Content-Type, double ext, null byte, HTTP PUT
- XSS payloads y recursos
- Reverse shells: bash, python, php, netcat, PowerShell
</details>

<details>
<summary><b>🔑 Brute Force & Password Cracking</b></summary>

- Hydra: SSH, FTP, HTTP POST/GET, SMB, MySQL
- John the Ripper: unshadow, formatos, reglas
- Hashcat: tipos de hash, modos
- Referencia de wordlists en Kali
</details>

---

## 🚀 Cómo usar

### Opción 1 — GitHub Pages (recomendada, siempre actualizado)
```
https://TU_USUARIO.github.io/eJPTv2-Playbook
```

### Opción 2 — Clonar y abrir local (funciona offline)
```bash
git clone https://github.com/TU_USUARIO/eJPTv2-Playbook.git
cd eJPTv2-Playbook
# Abre index.html en tu navegador
```

### Opción 3 — Descarga directa
Descarga [`index.html`](index.html) — funciona sin internet, sin dependencias, en cualquier navegador.

---

## 🛠️ Herramientas cubiertas

<div align="center">

| Categoría | Herramientas |
|-----------|-------------|
| **Scanning** | `nmap`, `fping`, `netdiscover` |
| **Web Enum** | `gobuster`, `dirb`, `ffuf`, `nikto`, `whatweb`, `wpscan` |
| **SMB** | `smbclient`, `smbmap`, `enum4linux`, `crackmapexec` |
| **Exploitation** | `metasploit`, `msfvenom`, `searchsploit` |
| **Web Attacks** | `sqlmap`, `burpsuite`, `netcat` |
| **Brute Force** | `hydra`, `john`, `hashcat` |
| **Post-Exploit** | `linpeas`, `winpeas`, `evil-winrm`, `meterpreter` |
| **Pivoting** | `autoroute`, `proxychains`, `portfwd`, `arpspoof` |
| **Misc** | `davtest`, `cadaver`, `xfreerdp`, `openssl` |

</div>

---

## 🧠 La Metodología

```
┌─────┐    ┌─────────┐    ┌─────────┐    ┌────────┐    ┌──────────────┐
│  R  │───▶│    S    │───▶│    E    │───▶│   G    │───▶│      P       │
│RECON│    │SCANNING │    │  ENUM   │    │GAINING │    │POST-EXPLOIT  │
│     │    │         │    │         │    │ACCESS  │    │              │
│¿Qué │    │¿Cómo    │    │¿Qué     │    │¿Cómo   │    │¿Qué hago     │
│hay? │    │está?    │    │tiene?   │    │entro?  │    │aquí dentro?  │
└─────┘    └─────────┘    └─────────┘    └────────┘    └──────────────┘
                                ▲
                                │ Si te atascas en G, vuelve aquí
```

> **Regla de oro:** Si te bloqueas buscando acceso (G), vuelve siempre a enumerar más (E). Hay información que aún no extrajiste.

---

## 🏆 Consejos de aprobados

> *"Haz TODOS los labs del PTSv2 de INE. El examen es prácticamente igual. Repítelos hasta hacerlos sin notas."*

> *"El examen es open-book. Ten tu cheatsheet lista antes de entrar. No pierdas tiempo buscando comandos."*

> *"Siempre escanea con `-p-` (todos los puertos). Los 1000 por defecto de nmap son insuficientes."*

> *"Cuando entres a una máquina, lo primero: `ip route` e `ifconfig`. Casi siempre hay una red oculta."*

> *"Tienes 48 horas. No es una carrera. Si te bloqueas, descansa 30 minutos y vuelve con ojos frescos."*

---

## 🤝 Cómo contribuir

¡Este proyecto vive gracias a la comunidad! Hay muchas formas de ayudar:

| Tipo | Cómo |
|------|------|
| 🐛 **Encontraste un error** | [Abre un Issue](../../issues/new?template=bug_report.md) |
| ➕ **Quieres agregar comandos** | [Abre un Pull Request](CONTRIBUTING.md) |
| 📝 **Tienes notas de tu examen** | Compártelas vía PR — la comunidad lo agradece |
| ⭐ **Quieres apoyar** | Dale una estrella al repo |
| 📢 **Quieres difundir** | Compártelo en LinkedIn, Reddit, Discord |

Lee [CONTRIBUTING.md](CONTRIBUTING.md) para los detalles del proceso.

---

## 🗺️ Roadmap

- [x] Playbook inicial con metodología R·S·E·G·P
- [x] Enumeration completa (SMB, FTP, HTTP, SSH, SMTP, MySQL, WinRM)
- [x] msfvenom payload reference completo
- [x] Pivoting con autoroute + proxychains
- [x] PrivEsc Linux y Windows
- [ ] Añadir Chisel para pivoting avanzado
- [ ] Sección de Active Directory básico
- [ ] Sección de CTFs resueltos paso a paso
- [ ] Versión PDF descargable
- [ ] Traducción al inglés
- [ ] Dark/Light mode toggle en el HTML

¿Quieres trabajar en alguno de estos? ¡[Abre un PR](CONTRIBUTING.md)!

---

## 📚 Créditos

Este playbook sintetiza el trabajo de la comunidad. Gracias a:

| Autor | Contribución |
|-------|-------------|
| **[syselement](https://blog.syselement.com/ine/courses/ejpt/ejpt-cheatsheet)** | Cheatsheet completo + PDF descargable |
| **[dev-angelist](https://github.com/dev-angelist/eJPTv2-Notes)** | Notas detalladas del curso PTSv2 |
| **[nmmorette](https://nmmorette.github.io/posts/2023/12/ejptv2-cheat-sheet/)** | Review post-examen + cheatsheet |
| **[iabdullah215](https://github.com/iabdullah215/eJPT-CheatSheet)** | eJPT CheatSheet community edition |
| **[th3cyb3rc0p / xalgord](https://methodological-notes.gitbook.io/ejptv2-preparation)** | ejPTv2 Preparation GitBook |
| **[HackTricks](https://book.hacktricks.xyz)** | Referencia técnica de técnicas |
| **[INE Security](https://ine.com)** | Curso PTSv2 original |

---

## ⚠️ Disclaimer

Este material es **exclusivamente para fines educativos** y preparación para certificaciones de ciberseguridad legítimas.

- ✅ Úsalo en laboratorios, CTFs, y entornos autorizados
- ✅ Úsalo para preparar el eJPTv2 u otras certificaciones
- ❌ **NO** uses estas técnicas en sistemas sin autorización explícita
- ❌ El uso no autorizado de estas técnicas es **ilegal** y va contra los términos de uso

Los autores no se responsabilizan por el uso indebido de este material.

---

## 📄 Licencia

Distribuido bajo la licencia **MIT**. Ve [LICENSE](LICENSE) para más detalles.

Puedes usarlo, modificarlo y distribuirlo libremente. Solo mantén los créditos originales. 🙏

---

<div align="center">

**Hecho con ❤️ para la comunidad de ciberseguridad hispanohablante**

Si este recurso te ayudó, considera darle una ⭐ — significa mucho y ayuda a que otros lo encuentren.

[⬆ Volver arriba](#-eJPTv2--playbook-maestro)

</div>
