# constructora-demo (genérica, marca OBRAS)
- Repo: Space Teskel (https://git.spacefast.com/teskel.git), path `obras/` (URL: https://teskel.online/obras/; desde 2026-11-14. `/constructora/*` y `/demo/constructora/*` redirigen con 301 vía `_redirects` del Space).
- App genérica, no de ningún cliente: sin logos, nombres ni normas de terceros.
- Es el laboratorio: lo que funciona se porta a otras apps, sin copiar estética ni marca.
- Look: marca OBRAS (ver DESIGN.md): crema sobre noche, amarillo de acento, portada de venta en `#portada`; la app en `#app`.
- Drive: carpeta `constructora`. Client ID propio (B).
- Publicación: GitHub (monticoagustin/constructora-demo) es la única copia. Desde 2026-11-12, cada push a `main` publica en vivo: la Action `.github/workflows/publicar-en-teskel.yml` copia index.html, manifest, íconos y `fonts/` a `obras/` del Space Teskel (secreto `SPACEFAST_TOKEN`). No editar `obras/` a mano en el Space.
- Git: commits y ramas libres; push o merge a `main` SOLO cuando el usuario lo pida (publica en vivo).
