---
name: Constructora Demo
description: Checklist genérico de obras, neumórfico, para mostrar a estudios de arquitectura.
colors:
  pizarra: "#cfd8e6"
  pizarra-honda: "#b8c4d4"
  cabecera-tabla: "#b7c3d4"
  tinta: "#121c2a"
  tinta-suave: "#2a3a50"
  azul-acero: "#3a567f"
  azul-acero-claro: "#4a6690"
  azul-acero-hondo: "#344d72"
  borde: "#8e9fb5"
  borde-suave: "#a3b2c5"
  borde-control: "#7f91a8"
  sombra-oscura: "#8494ab"
  sombra-clara: "#f8fafc"
  terracota-suave: "#e5cec5"
  terracota-card: "#e9d8d0"
  terracota-borde: "#bd927f"
  terracota-tinta: "#784331"
  ocre-importante: "#a8792c"
  verde-ok: "#3f6b52"
  verde-ok-suave: "#c5d6cb"
  verde-ok-borde: "#7f9f8a"
  verde-ok-tinta: "#2f4f3d"
  rojo-peligro: "#a23e48"
  rojo-peligro-suave: "#e5cbd0"
  rojo-peligro-borde: "#b7828b"
  naranja-hora: "#F26B4E"
typography:
  display:
    fontFamily: "Inter, system-ui, -apple-system, 'Segoe UI', Roboto, Arial, sans-serif"
    fontSize: "clamp(24px, 3.2vw, 34px)"
    fontWeight: 800
    lineHeight: 1.15
    letterSpacing: "-0.035em"
  stat:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "38px"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "-0.05em"
    fontFeature: "tnum"
  headline:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "25px"
    fontWeight: 700
    letterSpacing: "-0.03em"
  title:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "16px"
    fontWeight: 800
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "13px"
    fontWeight: 500
    lineHeight: 1.35
  label:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "12px"
    fontWeight: 700
  label-estado:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "12px"
    fontWeight: 800
    letterSpacing: "0.04em"
  caption:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "11px"
    fontWeight: 700
rounded:
  input-celda: "8px"
  input: "10px"
  segmento: "11px"
  control: "14px"
  card: "16px"
  fila-movil: "22px"
  panel: "24px"
  header: "28px"
  pill: "999px"
spacing:
  xxs: "4px"
  xs: "6px"
  sm: "8px"
  md: "12px"
  lg: "16px"
  xl: "18px"
  xxl: "24px"
  panel: "28px"
components:
  button:
    backgroundColor: "{colors.pizarra}"
    textColor: "{colors.tinta}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.control}"
    padding: "12px 16px"
    height: "48px"
  button-hover:
    textColor: "{colors.azul-acero}"
  button-primary:
    backgroundColor: "{colors.azul-acero-hondo}"
    textColor: "#ffffff"
    rounded: "{rounded.control}"
    padding: "12px 16px"
    height: "48px"
  button-danger:
    backgroundColor: "{colors.rojo-peligro-suave}"
    textColor: "{colors.rojo-peligro}"
    rounded: "{rounded.control}"
  tab:
    backgroundColor: "{colors.pizarra}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.control}"
    height: "48px"
  tab-active:
    backgroundColor: "{colors.pizarra}"
    textColor: "{colors.azul-acero}"
  input-search:
    backgroundColor: "{colors.pizarra}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.control}"
    padding: "12px 14px"
    height: "48px"
  segmented:
    backgroundColor: "{colors.pizarra}"
    textColor: "{colors.tinta-suave}"
    rounded: "{rounded.card}"
    padding: "5px"
  estado-toggle:
    backgroundColor: "{colors.pizarra}"
    textColor: "{colors.tinta}"
    typography: "{typography.label-estado}"
    rounded: "{rounded.segmento}"
    height: "44px"
  estado-toggle-si:
    backgroundColor: "{colors.verde-ok-suave}"
    textColor: "{colors.verde-ok-tinta}"
  obra-card:
    backgroundColor: "{colors.terracota-card}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.card}"
    padding: "14px 16px"
  obra-card-actual:
    backgroundColor: "{colors.terracota-suave}"
  panel:
    backgroundColor: "{colors.pizarra}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.panel}"
    padding: "26px 28px"
---

# Design System: Constructora Demo

## Overview

**Creative North Star: "Instrumento de bolsillo"**

La app se comporta como una herramienta física que se lleva a la obra: una sola superficie de pizarra azul grisácea de la que salen en relieve los controles, y que se hunde cuando algo está activo o apretado. Cada botón, pestaña y toggle tiene peso y respuesta táctil; el estado se lee en la profundidad antes que en el color.

El tono es táctil y calmo. No hay gradientes decorativos, ni fondos de color, ni ruido: la jerarquía la hacen el relieve, el peso tipográfico (Inter en 700–800 para todo lo que se lee de un vistazo) y los números en cifras tabulares. El color se reserva para significado: azul acero para lo activo y lo primario, verde para lo hecho, rojo para borrar, ocre para lo importante, terracota para el contexto "obra".

Es densa donde hace falta (la tabla de tareas en escritorio) y generosa en el toque (controles de 44–48px). En móvil la tabla se desarma en tarjetas en relieve, una por tarea.

**Key Characteristics:**
- Una sola superficie (pizarra #cfd8e6); la profundidad es la jerarquía.
- Relieve = disponible, hundido = activo/seleccionado/apretado.
- Inter en peso alto, tracking negativo en títulos y cifras.
- Color solo semántico, nunca decorativo.
- Objetivos táctiles de 44–48px.

## Colors

Paleta fría y apagada sobre una única superficie, con una familia cálida terracota que marca el mundo de las obras y acentos semánticos de baja saturación.

### Primary
- **Azul acero** (azul-acero): lo activo. Texto de la pestaña actual, segmento seleccionado, porcentajes de obra, anillos de foco y summaries.
- **Azul acero hondo / claro** (azul-acero-hondo → azul-acero-claro): el gradiente a 145° del único botón primario y la barra de progreso. No se usa en ningún otro lado.

### Secondary
- **Terracota** (terracota-card, terracota-suave, terracota-borde, terracota-tinta): el panel de Obras y sus tarjetas. Es el color de "la obra" como entidad; la obra seleccionada usa la variante suave y hundida.

### Tertiary
- **Ocre importante** (ocre-importante): filete izquierdo de 4px en filas y pestañas marcadas como importantes.
- **Naranja hora** (naranja-hora): solo la aguja de segundos del reloj de Buenos Aires. Detalle puntual, nunca un acento de interfaz.

### Neutral
- **Pizarra** (pizarra): fondo de la página y de todas las superficies. Es a la vez fondo y material.
- **Pizarra honda / cabecera de tabla** (pizarra-honda, cabecera-tabla): el encabezado de la tabla y zonas levemente rebajadas.
- **Tinta / tinta suave** (tinta, tinta-suave): texto principal y secundario (meta, labels de celda, notas).
- **Bordes** (borde, borde-suave, borde-control): filete de 1px que define el borde de cada pieza; los controles usan el más oscuro.
- **Luz y sombra** (sombra-clara, sombra-oscura): los dos lados de todo relieve. No son colores de relleno.

### Semánticos
- **Verde ok** (verde-ok-*): tarea hecha ("SI"). Fondo suave, tinta oscura, hundido.
- **Rojo peligro** (rojo-peligro-*): borrar tarea, pestaña o foto; foco de esas acciones.

### Named Rules
**The Una Superficie Rule.** Fondo, header, paneles, controles e inputs comparten el mismo color de pizarra. Si una pieza necesita destacarse, se levanta o se hunde; no se pinta.

**The Color Significa Rule.** Todo color fuera de la pizarra y la tinta tiene un significado fijo (activo, hecho, borrar, importante, obra). Un color nuevo necesita un significado nuevo.

## Typography

**Display Font:** Inter (con system-ui, -apple-system, Segoe UI, Roboto, Arial)
**Body Font:** Inter (mismo stack)

**Character:** Una sola familia, trabajada por peso. Los títulos y cifras van en 800 con tracking negativo, compactos y firmes como un rótulo de herramienta; el cuerpo queda en 400–500 para que la tabla respire.

### Hierarchy
- **Display** (800, clamp(24px, 3.2vw, 34px), 1.15, −0.035em): el título de la app en el header.
- **Stat** (800, 38px, 1, −0.05em, cifras tabulares): los números grandes del resumen.
- **Headline** (700, 25px, −0.03em): títulos de paneles modales (Google Drive, dashboard).
- **Title** (800, 16px, −0.01em): títulos de sección (Obras) y nombre de pestaña activa.
- **Body** (400, 15px, 1.5): texto general.
- **Body small** (500, 13px, 1.35): contenido de celdas, tareas, botones.
- **Label** (700, 12px): labels de celda en móvil, meta, summaries.
- **Label estado** (800, 12px, +0.04em): el toggle de estado de cada tarea.
- **Caption** (700, 11px): textos auxiliares mínimos.

### Named Rules
**The Cifra Tabular Rule.** Todo porcentaje, conteo o número que se compara (resumen, obras, pisos) usa `font-variant-numeric: tabular-nums`.

**The 16px en Móvil Rule.** Bajo 820px, todo input editable sube a 16px para que iOS no haga zoom.

## Layout

App de una sola columna con margen lateral `max(16px, safe-area-inset)`. El header es una pieza flotante con margen propio (16px arriba, 12px abajo), no una barra pegada al borde. Debajo: resumen, panel de obras, controles de filtro y la tabla de tareas.

Ritmo de espaciado sobre 4/6/8/12/16/18/24/28px; el gap más usado es 12px entre piezas hermanas y 24–28px de padding en paneles grandes.

Breakpoints:
- **≤820px:** la tabla deja de ser tabla. El thead se oculta y cada fila se vuelve una tarjeta en relieve de dos columnas, con el label de cada celda arriba del valor (`data-l`). Tarea, acciones y fotos ocupan el ancho completo. Header y paneles achican padding y radio.
- **≤520px:** header y resumen se compactan más (20px de padding, radio 20px); el input de obra pasa a ancho completo.

En escritorio la tabla tiene un mínimo de 1200px y scrollea horizontal dentro de su contenedor.

Respeta `safe-area-inset` arriba, abajo y a los lados (PWA instalada).

## Elevation & Depth

Sistema neumórfico: toda la profundidad sale de un par de sombras opuestas sobre la misma superficie, una oscura abajo a la derecha y una clara arriba a la izquierda. No hay sombras de color ni elevación por z-index, salvo el panel modal, que flota con una sombra difusa real.

### Shadow Vocabulary
- **Relieve** (`box-shadow: 8px 8px 18px #8494ab, -8px -8px 18px #f8fafc`): header, resumen, panel de obras, filas-tarjeta en móvil.
- **Relieve chico** (`box-shadow: 5px 5px 11px #8494ab, -5px -5px 11px #f8fafc`): botones, pestañas, toggles de estado, segmento seleccionado.
- **Hundido** (`box-shadow: inset 5px 5px 10px #8e9db2, inset -5px -5px 10px #f8fafc`): inputs, búsqueda, selects, contenedor de segmentos, barra de progreso, pestaña activa, botón apretado, estado "SI".
- **Relieve terracota** (`5px 5px 12px #c4a090, -5px -5px 12px #f7ebe6`, e inset equivalente para la obra actual): solo tarjetas de obra.
- **Flotante** (`18px 18px 52px rgba(27,40,59,.32), inset 1px 1px 0 #fff`): panel modal de Drive/dashboard.

### Named Rules
**The Hundido Es Activo Rule.** Lo que está seleccionado, encendido o apretado se hunde; lo que está disponible sobresale. Nunca al revés.

**The Contraste Primero Rule.** En `prefers-contrast: more` los bordes se oscurecen (#44566d) y la tinta baja a #0c1420; en `forced-colors` desaparecen todas las sombras y el estado pasa a outline `Highlight`. La profundidad nunca es el único portador del estado.

## Shapes

Esquinas generosas y redondeadas, que crecen con el tamaño de la pieza: 8px en inputs de celda, 10–11px en inputs y segmentos, 14px en controles, 16px en tarjetas, 22–24px en paneles y 28px en el header. Píldora completa solo para barras de progreso. Todas las piezas llevan un filete de 1px que completa el borde que la sombra sola no define. Los botones de borrar foto son círculos.

## Components

### Buttons
Táctiles y silenciosos: sobresalen, y al apretarlos se hunden.
- **Shape:** esquinas redondeadas de 14px, 48px de alto mínimo.
- **Default:** pizarra en relieve chico, borde de control, texto tinta 13px/700.
- **Hover (solo `hover:hover`):** el texto pasa a azul acero; la sombra no cambia.
- **Active:** hundido.
- **Primario:** gradiente azul acero a 145°, texto blanco. Hover baja la opacidad a .85; active se hunde con sombras azules internas. Uno por contexto.
- **Peligro:** fondo rojo suave, texto y borde rojo.
- **Disabled:** opacidad .55, cursor wait.

### Tabs (pestañas de checklist)
- Píldoras de 14px en relieve chico, 48px de alto.
- **Activa:** hundida, texto azul acero 800 16px, y el nombre es un input editable en el lugar (subrayado azul al enfocar).
- **Importante:** filete ocre de 4px a la izquierda.
- Botón de borrar de 44×44 dentro de la pestaña, en rojo.

### Segmented control (filtros)
- Contenedor hundido de 16px de radio con padding de 5px.
- Opción seleccionada: sobresale con relieve chico, texto azul acero 800 (`aria-pressed="true"`).

### Inputs / Fields
- **Búsqueda y selects:** hundidos, 14px de radio, 48px de alto, borde de control.
- **Celdas de tabla:** transparentes y sin borde en reposo; al enfocar se hunden con borde azul acero. En móvil quedan siempre hundidos.
- **Foco:** outline 3px azul acero con 3px de separación (2px/1px dentro de celdas).

### Toggle de estado
Componente propio: un botón de ancho completo, 44px de alto (48px en móvil), 11px de radio, label 12px/800 en mayúsculas con +0.04em. En relieve cuando la tarea está pendiente; hundido sobre verde suave cuando está hecha ("SI").

### Tarjeta de obra
- Terracota sobre panel terracota, 16px de radio, padding 14×16.
- Nombre 15px a la izquierda, % ejecutado 24px/800 azul acero a la derecha.
- Desplegable de pisos con mini barras de progreso de 10px.
- **Obra actual:** se hunde sobre terracota suave.

### Barra de progreso
Canal hundido en píldora de 14px con 3px de padding; relleno con gradiente azul acero, animado en ancho (.35s ease).

### Panel modal
Pizarra, 26px de radio, 30px de padding, máximo 460px de ancho, con sombra flotante. Es la única pieza que flota de verdad.

## Do's and Don'ts

### Do:
- **Do** construir cada pieza nueva sobre la pizarra con el par de sombras: relieve si está disponible, hundida si está activa.
- **Do** mantener objetivos táctiles de 44px como mínimo (48px en controles principales).
- **Do** usar Inter 800 con tracking negativo para títulos y cifras, y cifras tabulares en todo número comparable.
- **Do** dar a cada pieza su filete de 1px además de la sombra.
- **Do** probar cada componente nuevo en `prefers-contrast: more`, `forced-colors` e impresión (fondo blanco, sin sombras).

### Don't:
- **Don't** pintar fondos de color para destacar algo; levantalo o hundilo.
- **Don't** usar el naranja de la hora fuera de la aguja del reloj.
- **Don't** usar el gradiente azul en más de un botón por contexto.
- **Don't** agregar el logo de 3dF, la tipografía Archivo ni el blanco y negro de 3dF: esa identidad vive en la otra app.
- **Don't** dejar el estado de una tarea solo en la sombra; siempre tiene texto y color.
