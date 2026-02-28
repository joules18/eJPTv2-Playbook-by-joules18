# 🤝 Guía para Contribuir

¡Gracias por querer contribuir al **eJPTv2 Playbook Maestro**! Este proyecto vive gracias a la comunidad y cada aporte, por pequeño que sea, hace una diferencia real para quienes estudian para el eJPTv2.

---

## 📋 ¿Qué tipo de contribuciones aceptamos?

| Tipo | Ejemplos |
|------|---------|
| 🐛 **Bug fixes** | Comando incorrecto, typo, enlace roto |
| ➕ **Nuevos comandos** | Técnicas que no están cubiertas |
| 📝 **Notas del examen** | Técnicas que viste en el eJPTv2 real |
| 🌍 **Traducciones** | Traducir secciones a otros idiomas |
| 📚 **Recursos** | Links a recursos útiles de calidad |
| 🎨 **Mejoras de UI** | Mejoras al diseño del HTML |
| ✅ **CTF writeups** | Resolución de labs relacionados |

---

## 🚀 Proceso para hacer un Pull Request

### 1. Fork del repositorio
Haz clic en el botón **Fork** en la esquina superior derecha del repo.

### 2. Clona tu fork
```bash
git clone https://github.com/TU_USUARIO/eJPTv2-Playbook.git
cd eJPTv2-Playbook
```

### 3. Crea una rama descriptiva
```bash
# Formato: tipo/descripción-corta
git checkout -b feat/añadir-chisel-pivoting
git checkout -b fix/comando-hydra-incorrecto
git checkout -b docs/mejorar-seccion-smb
```

### 4. Haz tus cambios
- Edita `index.html` para cambios en el playbook
- Edita `README.md` para cambios en la documentación
- Prueba que el HTML se ve bien en tu navegador antes de hacer PR

### 5. Commit con mensaje claro
Usamos [Conventional Commits](https://www.conventionalcommits.org/):

```bash
git add .
git commit -m "feat: añadir pivoting con chisel en sección de redes"
git commit -m "fix: corregir comando hydra para HTTP POST"
git commit -m "docs: añadir recurso de GTFOBins en sección privesc"
```

**Prefijos válidos:**
- `feat:` — nueva funcionalidad o contenido
- `fix:` — corrección de error
- `docs:` — cambios en documentación
- `style:` — cambios de formato/diseño
- `refactor:` — reorganización de contenido

### 6. Push y abre el PR
```bash
git push origin feat/añadir-chisel-pivoting
```

Luego ve a GitHub y abre el Pull Request contra la rama `main`.

---

## ✅ Checklist antes de hacer PR

- [ ] El HTML abre correctamente en el navegador
- [ ] Los comandos están probados y funcionan
- [ ] No hay errores ortográficos obvios
- [ ] Si añades una nueva sección, está en el TOC de navegación
- [ ] Los botones "Copy" del HTML funcionan en la nueva sección

---

## 🐛 Reportar un bug

Abre un [Issue](../../issues/new) con:

1. **Descripción** del problema
2. **Sección afectada** (ej: "Sección SMB, comando smbmap")
3. **Comportamiento esperado** vs **comportamiento actual**
4. Si es un comando incorrecto, el comando correcto con fuente

---

## 💡 Sugerir una mejora

Abre un [Issue](../../issues/new) con:

1. **¿Qué técnica/herramienta falta?**
2. **¿Por qué sería útil para el eJPTv2?**
3. **Ejemplo de los comandos** (si los tienes)

---

## 🏆 Hall of Fame de contribuidores

Todos los que hagan un PR aceptado serán añadidos a la sección de **Créditos** del README con su usuario de GitHub. ¡Es nuestra forma de decir gracias! 🙌

---

## ❓ ¿Tienes dudas?

Abre un [Issue](../../issues/new) con el tag `question` o pregunta en las [Discussions](../../discussions).

---

*Recuerda: no hay contribución demasiado pequeña. Un typo corregido ya ayuda a la siguiente persona que lea el playbook.* ✨
