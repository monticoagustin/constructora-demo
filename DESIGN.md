---
name: Constructora Demo
description: Seguimiento de obra genérico, mate y cálido, para mostrar a estudios de arquitectura.
colors:
  cal: "#EEEBE5"
  losa: "#F7F5F1"
  losa-honda: "#E3DFD7"
  hormigon: "#CFC9BE"
  borde-control: "#837C70"
  hierro: "#26231F"
  hierro-suave: "#5A544A"
  ladrillo: "#9D3E25"
  on-ladrillo: "#FFF8F4"
  ladrillo-suave: "#EFD9CF"
  patina: "#2F6B50"
  on-patina: "#F4FAF6"
  patina-suave: "#D4E4DA"
  senal: "#E0A21B"
  on-senal: "#26231F"
  senal-suave: "#F5E2B0"
  peligro: "#A2243A"
  on-peligro: "#FFF6F7"
  peligro-suave: "#F2D3D6"
  encofrado: "#7C5428"
  encofrado-suave: "#EBDCC6"
colors-dark:
  cal: "#1B1916"
  losa: "#25221E"
  losa-honda: "#141210"
  hormigon: "#3A362F"
  borde-control: "#948D82"
  hierro: "#F1EEE8"
  hierro-suave: "#B9B3A8"
  ladrillo: "#E08A66"
  on-ladrillo: "#1B1916"
  ladrillo-suave: "#3B2A22"
  patina: "#78BE9B"
  on-patina: "#10241A"
  patina-suave: "#1F3329"
  senal: "#E8B53A"
  on-senal: "#1B1916"
  senal-suave: "#3A2F14"
  peligro: "#F08A99"
  on-peligro: "#2A0E14"
  peligro-suave: "#3D1F25"
  encofrado: "#CDA070"
  encofrado-suave: "#33281B"
typography:
  display:
    fontFamily: "Bricolage Grotesque"
    fontSize: "44px"
    lineHeight: "48px"
    fontWeight: 700
  titulo:
    fontFamily: "Bricolage Grotesque"
    fontSize: "28px"
    lineHeight: "32px"
    fontWeight: 700
  subtitulo:
    fontFamily: "Bricolage Grotesque"
    fontSize: "20px"
    lineHeight: "26px"
    fontWeight: 600
  seccion:
    fontFamily: "Bricolage Grotesque"
    fontSize: "16px"
    lineHeight: "22px"
    fontWeight: 600
  cuerpo:
    fontFamily: "Instrument Sans"
    fontSize: "15px"
    lineHeight: "22px"
    fontWeight: 400
  cuerpo-fuerte:
    fontFamily: "Instrument Sans"
    fontSize: "15px"
    lineHeight: "22px"
    fontWeight: 600
  celda:
    fontFamily: "Instrument Sans"
    fontSize: "14px"
    lineHeight: "20px"
    fontWeight: 400
  etiqueta:
    fontFamily: "Instrument Sans"
    fontSize: "12px"
    lineHeight: "16px"
    fontWeight: 600
    letterSpacing: "0.04em"
  nota:
    fontFamily: "Instrument Sans"
    fontSize: "12px"
    lineHeight: "16px"
    fontWeight: 400
  cota-grande:
    fontFamily: "IBM Plex Mono"
    fontSize: "32px"
    lineHeight: "36px"
    fontWeight: 600
  cota:
    fontFamily: "IBM Plex Mono"
    fontSize: "14px"
    lineHeight: "20px"
    fontWeight: 500
  codigo:
    fontFamily: "IBM Plex Mono"
    fontSize: "12px"
    lineHeight: "16px"
    fontWeight: 400
rounded:
  r-arista: "2px"
  r-pieza: "4px"
  r-losa: "8px"
  r-panel: "12px"
  r-pildora: "999px"
spacing:
  esp-1: "4px"
  esp-2: "8px"
  esp-3: "12px"
  esp-4: "16px"
  esp-5: "24px"
  esp-6: "32px"
  esp-7: "48px"
  esp-8: "64px"
  toque-min: "44px"
  toque: "48px"
---

# Design System: Constructora Demo ("Losa")

## Overview

**Norte creativo: "Instrumento de bolsillo", ahora en material.** La app se siente como una herramienta de obra bien hecha: mate, cálida y táctil, hecha de hormigón, hierro y ladrillo. Reemplaza al look neumórfico anterior: no hay sombras hundidas ni relieves suaves. La profundidad sale del tono escalonado y de líneas finas.

- Superficie en tres tonos: `cal` (página), `losa` (tarjetas y filas) y `losa-honda` (lo hundido: pistas, campos, filtros).
- Un solo acento, `ladrillo`, para la acción principal y el avance. Detalle puntual, no relleno.
- Verde (`patina`), ámbar (`senal`) y rojo (`peligro`) son solo estado y siempre llevan palabra o tilde.
- Genérica: sin logo ni identidad de ningún cliente. Los íconos de la app instalada son los de Teskel, provisorios.

La fuente de verdad ejecutable es el artifact "Sistema Losa" (tokens, componentes y README). Este archivo es su resumen para el repo. Estado: el sistema está definido; `index.html` todavía usa el look anterior y se migra en un paso aparte.

## Colors

Dos temas, claro y oscuro (valores oscuros en `colors-dark`). Cada par de texto y fondo cumple 4,5:1 y cada borde de control 3:1 en los dos temas.

- **Superficies:** `cal`, `losa`, `losa-honda`; línea fina `hormigon`; borde de control `borde-control`.
- **Texto:** `hierro` (principal) y `hierro-suave` (metadatos).
- **Acento:** `ladrillo` con `on-ladrillo` encima; `ladrillo-suave` para lo seleccionado.
- **Estado:** `patina` (hecho), `senal` (importante, vence mañana), `peligro` (vencida, error), cada uno con `on-…` y `-suave`.
- **Material:** `encofrado` para rubros.
- **Foco:** anillo de 2px con 2px de separación, color `hierro`.

### Named Rules
- **Regla del acento único:** `ladrillo` no ocupa más de una acción principal y la parte llena de la cota por pantalla.
- **Regla de la palabra:** ningún estado se comunica solo con color.
- **Regla del color fijo:** sobre un relleno de color se usa su `on-…`, nunca blanco o negro fijos.

## Typography

- **Títulos:** Bricolage Grotesque (`display`, `titulo`, `subtitulo`, `seccion`).
- **Texto:** Instrument Sans (`cuerpo`, `cuerpo-fuerte`, `celda`, `etiqueta`, `nota`). No tiene "²": usar "m2".
- **Datos:** IBM Plex Mono (`cota-grande`, `cota`, `codigo`) para cifras, porcentajes y fechas.
- Mínimo 12px. Las etiquetas van con mayúscula inicial, no en versalitas.

## Layout

Escala de 4 (`esp-1` a `esp-8`). Todo control tocable mide al menos `toque-min` (44px); lo de uso en obra, `toque` (48px). En celular las filas de tarea apilan los chips debajo del título y las pestañas se desplazan en horizontal.

## Elevation & Depth

Mate. La profundidad es tonal: `cal` < `losa`, y `losa-honda` hundido. Solo hay dos sombras: `sombra-apoyo` (casi plana, tarjetas) y `sombra-flotante` (modales, menús y avisos).

### Named Rules
- **Regla anti-neumorfismo:** ninguna sombra clara ni sombras internas dobles. El relieve no es decoración.

## Shapes

`r-arista` 2px (marcas), `r-pieza` 4px (chips, filas), `r-losa` 8px (botones, campos, tareas), `r-panel` 12px (tarjetas de obra, modales), `r-pildora` (filtros y toggles).

## Components

- **Button:** primario en `ladrillo` (uno por pantalla), secundario sobre `losa` con borde `borde-control`, de texto y de peligro. Alto mínimo 44px.
- **Tabs:** pestañas del checklist; la activa, texto `ladrillo` y subrayado de 3px.
- **Filtro:** control segmentado sobre `losa-honda`; la opción activa con `ladrillo-suave` y borde `ladrillo`.
- **Campo:** sobre `losa-honda` con borde `borde-control`, etiqueta siempre visible y error con mensaje.
- **Estado:** toggle Pendiente / Hecho con palabra y tilde.
- **Chip:** Importante (`senal`), Vence mañana, Vencida, Hecho y rubro (`encofrado`).
- **Cota:** el motivo propio: avance como línea de plano con marcas a 25, 50 y 75 %, con etiqueta mono. Lleno `ladrillo`; completo, `patina`.
- **ObraCard, Tarea, Resumen, Panel:** tarjeta de obra con cota y chips, fila de tarea, cifra del dashboard y modal de Drive.

## Do's and Don'ts

### Do:
- **Do** separar superficies con tono y una línea `hormigon` de 1px.
- **Do** marcar "Importante" con un chip `senal`.
- **Do** escribir en español rioplatense, con verbo y objeto en los botones.
- **Do** mostrar siempre el número junto a la cota.

### Don't:
- **Don't** usar neumorfismo, gradientes ni brillos.
- **Don't** usar un borde de color a un solo lado para marcar una tarjeta.
- **Don't** usar Inter ni Roboto.
- **Don't** usar logos, nombres o datos de ningún cliente real.
