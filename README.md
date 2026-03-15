# Shiftly – Gestor de Trabajadores

PWA para gestionar turnos, horarios y nóminas de tu equipo. Funciona offline y se instala como app en el móvil.

## Deploy en GitHub Pages

```bash
# 1. Crea un repo en GitHub (ej: shiftly)

# 2. Sube los archivos
git init
git add .
git commit -m "Shiftly PWA"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/shiftly.git
git push -u origin main

# 3. Activa GitHub Pages
#    Settings → Pages → Source: "Deploy from a branch" → Branch: main → / (root) → Save
#    Tu app estará en: https://TU_USUARIO.github.io/shiftly/
```

## Estructura

```
shiftly/
├── index.html      ← App completa (React + Babel standalone)
├── manifest.json   ← Manifest PWA
├── sw.js           ← Service Worker (cache offline)
├── icons/
│   ├── icon-192.png
│   └── icon-512.png
└── README.md
```

## Funcionalidades

- **Calendario interactivo** con vista mensual y detalle diario
- **Gestión de equipo** con nombre, puesto, precio/hora y color
- **Rangos horarios** normales y **partidos** (2 bloques con descanso)
- **Asignación de turnos** rápida desde el calendario
- **Perfil del trabajador** con resumen mensual
- **Desglose de nómina** (bruto, SS, IRPF, neto estimado)
- **Gráfico de actividad** diaria por trabajador
- **Persistencia** en localStorage (los datos se guardan en el navegador)
- **Funciona offline** gracias al Service Worker
- **Instalable** como PWA en Android/iOS

## Instalar en el móvil

1. Abre la URL en Chrome (Android) o Safari (iOS)
2. Android: menú ⋮ → "Instalar app" / "Añadir a pantalla de inicio"
3. iOS: botón compartir → "Añadir a pantalla de inicio"
