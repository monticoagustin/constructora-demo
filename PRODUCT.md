# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Todos los roles de una obra usan la misma app, cada uno desde su situación:

- **Arquitecto / estudio:** coordina rubros y contratistas para un comitente y le rinde cuentas del avance.
- **Jefe / director de obra:** sigue tareas, plazos y contratistas de varias obras a la vez.
- **Dueño / gerente de constructora:** mira el avance general y el dashboard mensual.
- **Capataz en obra:** tilda tareas y saca fotos en el lugar.

## Product Purpose

App genérica de gestión de obras (checklist de tareas por obra) que se usa como demo de venta. Es además el laboratorio: lo que funciona acá se porta a la app de 3dF (`3df-checklist`) con la identidad de 3dF. El éxito es que un estudio de arquitectura, al verla, entienda que puede seguir sus obras de forma prolija y entregarle al comitente un PDF claro del avance.

## Positioning

Comprador objetivo: **estudios de arquitectura**. Mensaje central: seguimiento de obra prolijo y un PDF presentable para el comitente. Los datos se sincronizan con el Google Drive propio del usuario.

## Operating Context

- Varias obras en paralelo, cada una con tareas por rubro, ambiente y contratista.
- Pestañas de checklist por obra, filtros por estado y rubro, búsqueda, plazos próximos ("vencen mañana").
- Dashboard mensual con % ejecutado.
- Fotos de obra, exportación a PDF, sync con Google Drive (carpeta `constructora`).

## Capabilities and Constraints

- PWA single-file (`index.html`), sin build. Idioma español (es-AR).
- Storage local con keys `3df-teskel-demo-*`.
- Google Drive con Client ID propio (cliente B); nunca el de 3dF. Origen autorizado: `https://teskel.online`.
- Publicada en https://teskel.online/constructora/ (Space Teskel, path `constructora/`). Push a GitHub y publicar en vivo son pasos separados.
- **Pendiente:** el `index.html` en vivo difiere del del repo; decidir cuál queda antes de trabajar.
- **Sin decidir:** requisitos de uso en obra (offline, sol, tamaño de toque), alcance de idiomas, política de datos de ejemplo.

## Brand Commitments

- App genérica, no de ningún cliente.
- Sin logo 3dF ni normas ISO de 3dF.
- La identidad visual de esta demo y la de 3dF no se copian entre proyectos; solo se porta funcionalidad.

## Evidence on Hand

- La app misma (`index.html`) con datos de ejemplo.
- No hay testimonios, clientes, casos ni métricas reales: no inventarlos.

## Product Principles

1. Genérica primero: nada que ate la demo a un cliente concreto.
2. Laboratorio: cada feature se diseña para poder portarse a 3dF sin arrastrar estética ni marca.
3. Lo que ve el comitente (PDF, dashboard) tiene que verse presentable sin retoques.
4. Un mismo producto sirve a cuatro roles; ninguno debería necesitar una app distinta.
