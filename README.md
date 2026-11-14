# constructora-demo

App GENÉRICA de gestión de obras, marca OBRAS (ver `DESIGN.md`). Es el laboratorio: acá se prueba todo.

- Demo: https://teskel.online/constructora/ (desde 2026-11-09; `/demo/constructora/` redirige con 301)
- Alojada en el Space Teskel, path `constructora/` (se separa al migrar).
- PWA single-file: Anybody e Instrument Sans (en `fonts/`), íconos Tabler embebidos.
- Drive: CARPETA = `constructora`
- Storage keys: `constructora-demo-*`
- OAuth Client ID: cliente "B", ya cargado en `index.html` (`GOOGLE_CLIENT_ID`). Origen autorizado necesario: `https://teskel.online` (el origen es solo el dominio, no cuenta la ruta).

## Features
Multi-obra, filtros, plazos, dashboard, fotos, PDF, sync con Drive.

## Flujo hacia otras apps
Lo que funcione acá se porta con la misma funcionalidad, pero con la identidad de cada proyecto. El look y el branding no se copian entre proyectos.

## Sin
Logos, nombres ni normas de ningún cliente.
