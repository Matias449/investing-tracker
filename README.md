<div align="center">

# 📈 Inversión Tracker

**Tracker semanal de portafolio de inversiones · CLP**

![PWA](https://img.shields.io/badge/PWA-ready-6366f1?style=flat-square&logo=googlechrome&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-deployed-22c55e?style=flat-square&logo=github&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-fb923c?style=flat-square)
![Vanilla JS](https://img.shields.io/badge/vanilla-JS-f7df1e?style=flat-square&logo=javascript&logoColor=black)

[**→ Abrir App**](https://Matias449.github.io/investing-tracker/)

</div>

---

## ¿Qué es esto?

Una PWA (Progressive Web App) minimalista para hacer seguimiento semanal de tu portafolio de inversiones. Sin registro, sin servidores, sin complicaciones — solo tú y tus números.

```
Cada lunes → ingresas el valor actual de tu portafolio → listo.
El tracker calcula todo lo demás.
```

## Funcionalidades

- **Registro semanal** — ingresa el valor de tu portafolio cada lunes
- **Desglose capital vs ganancia** — barra visual que separa lo que pusiste de lo que ganaste
- **Comparación semanal** — cuánto subió o bajó respecto a la semana anterior
- **Gráfico de evolución** — línea de progreso con referencia del capital aportado
- **Múltiples aportes** — agrega capital mes a mes y el tracker recalcula todo
- **Funciona offline** — service worker cachea la app completa
- **Instalable en Android** — se instala como app nativa desde Chrome

## Instalar en tu móvil

1. Abre la URL de la app en **Chrome para Android**
2. Toca el banner **"Instalar"** que aparece automáticamente
3. O bien: menú `⋮` → **Añadir a pantalla de inicio**

La app se abrirá a pantalla completa, sin barra del navegador, como cualquier app nativa.

## Stack

| Archivo | Rol |
|---|---|
| `index.html` | App completa — HTML + CSS + JS en un solo archivo |
| `manifest.json` | Configuración PWA (nombre, icono, colores) |
| `sw.js` | Service Worker — cache offline |
| `icon-192.png` / `icon-512.png` | Íconos de la app |

Sin frameworks. Sin dependencias. Sin `node_modules`. Solo archivos.

## Deploy en GitHub Pages

```bash
# 1. Clona o forkea este repositorio
git clone https://github.com/TU-USUARIO/inversion-tracker.git

# 2. Activa GitHub Pages
# Settings → Pages → Branch: main → Save

# 3. Tu app estará en:
# https://TU-USUARIO.github.io/inversion-tracker/
```

## Datos y privacidad

Los datos se guardan **únicamente en tu dispositivo** via `localStorage`. No se envía nada a ningún servidor. No hay analytics, no hay tracking, no hay cookies.

> ⚠️ Por esto mismo, los datos no se sincronizan entre dispositivos (PC ↔ móvil). Cada navegador tiene su propia copia local.

## Roadmap

- [ ] Sincronización entre dispositivos (Firebase / Supabase)
- [ ] Exportar / importar datos en JSON
- [ ] Notificación recordatorio los lunes
- [ ] Modo múltiples portafolios

## Licencia

MIT — úsalo, modifícalo, compártelo.

---

<div align="center">
  <sub>Hecho con Claude · <a href="https://claude.ai">claude.ai</a></sub>
</div>
