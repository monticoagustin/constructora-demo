# constructora-demo (genérica, estilo Señalética)
- Repo: Space Teskel (https://git.spacefast.com/teskel.git), path `constructora/` (URL: https://teskel.online/constructora/; el prefijo `/demo` se eliminó el 2026-11-09 y `/demo/constructora/*` redirige con 301).
- App genérica, no de ningún cliente: sin logos, nombres ni normas de terceros.
- Es el laboratorio: lo que funciona se porta a otras apps, sin copiar estética ni marca.
- Look: Señalética de obra (ver DESIGN.md): negro, blanco y amarillo de seguridad, sin neumorfismo.
- Drive: carpeta `constructora`. Client ID propio (B).
- Publicación: GitHub (monticoagustin/constructora-demo) es la única copia. Desde 2026-11-12, cada push a `main` publica en vivo: la Action `.github/workflows/publicar-en-teskel.yml` copia index.html, manifest, íconos y `fonts/` a `constructora/` del Space Teskel (secreto `SPACEFAST_TOKEN`). No editar `constructora/` a mano en el Space.
- Git: commits y ramas libres; push o merge a `main` SOLO cuando el usuario lo pida (publica en vivo).
