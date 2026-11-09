# constructora-demo

App GENÉRICA de gestión de obras, estilo neumórfico. Es el laboratorio: acá se prueba todo. La versión 3dF con Drive vive aparte, en `checklists-drive` (carpeta local `3df-checklist-agustin`, publicada en `/3df/`).

- Demo: https://teskel.online/constructora/ (desde 2026-11-09; `/demo/constructora/` redirige con 301)
- Alojada en el Space Teskel, path `constructora/` (se separa al migrar).
- PWA single-file: Inter, superficie slate, sombras suaves.
- Drive: CARPETA = `constructora`
- Storage keys: `3df-teskel-demo-*`
- OAuth Client ID: cliente "B", ya cargado en `index.html` (`GOOGLE_CLIENT_ID`). Origen autorizado necesario: `https://teskel.online` (el origen es solo el dominio, no cuenta la ruta).

## Features
Multi-obra, filtros, plazos, dashboard, fotos, PDF, sync con Drive.

## Flujo hacia 3df-checklist
Lo que funcione acá se porta a `3df-checklist` con la misma funcionalidad, pero con identidad 3dF (Archivo, negro/blanco, logo 3dF) y respetando la ISO. El neumorfismo y el branding no se copian entre proyectos.

## Sin
Logo 3dF, normas ISO de 3dF.
