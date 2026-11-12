---
name: Constructora Demo
description: Seguimiento de obra genérico con estética de señalética de obra, para mostrar a estudios de arquitectura.
colors:
  fondo: "#E9E7E1"
  tarjeta: "#FFFFFF"
  hundido: "#F2F0EA"
  tinta: "#16181A"
  tinta-suave: "#3F4348"
  amarillo-seguridad: "#FFC20E"
  ok: "#127A3E"
  ok-fondo: "#E3F2E8"
  aviso: "#C98A00"
  importante-fondo: "#FFF3CC"
  peligro: "#B8141F"
typography:
  titulo:
    fontFamily: "Barlow Condensed"
    fontWeight: 700
    textTransform: uppercase
  cifras:
    fontFamily: "Barlow Condensed"
    fontWeight: 700
  cuerpo:
    fontFamily: "Barlow"
    fontSize: "15px"
    fontWeight: 400
  rotulo:
    fontFamily: "Barlow Condensed"
    fontWeight: 600
    textTransform: uppercase
    letterSpacing: "0.04em"
rounded:
  todo: "0"
borders:
  control: "2px solid #16181A"
shadows:
  pieza: "3px 3px 0 #16181A"
  boton-encabezado: "3px 3px 0 #FFC20E"
---

# Design System: Constructora Demo ("Señalética")

## Overview

**Norte creativo: cartelería de obra.** La app se lee como la señalética de un obrador: negro, blanco y amarillo de seguridad, bordes gruesos, esquinas rectas y tipografía condensada. Alto contraste para usarla al sol y con guantes. Reemplaza al look neumórfico anterior (sin relieves suaves ni sombras difusas).

- El estilo vive en el bloque `<style id="skin-senaletica">` de `index.html`, encima del CSS anterior.
- Fuentes Barlow y Barlow Condensed (OFL) en `fonts/`, servidas junto a la app.
- Íconos: Tabler Icons (MIT), embebidos como máscaras SVG en el CSS.
- Genérica: sin logo ni identidad de ningún cliente. Los íconos de la PWA son los de Teskel, provisorios.

## Colors

- **Superficies:** `fondo` (página), `tarjeta` (bloques), `hundido` (pistas, filtros).
- **Tinta:** `tinta` para texto, bordes y botón primario; `tinta-suave` para metadatos.
- **Amarillo de seguridad:** acento único. Texto del botón primario sobre negro, pestaña y obra seleccionadas, filtro activo, aviso "Vencen mañana", franjas de peligro.
- **Estado:** `ok` (ejecutada, con la palabra SÍ), `aviso` (importante), `peligro` (borrar). Nunca solo color.

## Typography

Títulos, cifras y rótulos en Barlow Condensed (mayúscula en títulos y rótulos); texto en Barlow. Las cifras del resumen van grandes (hasta 52px).

## Elevation & Shapes

Todo con esquinas rectas. La profundidad es una sombra dura desplazada (`pieza`, 3px). El encabezado es negro y cierra con una franja de peligro. Las barras de avance son cintas rayadas amarillo y negro.

## Motion

Seco y mecánico, sin rebotes. Se apaga con "reducir movimiento".

- **Sello al tildar:** el botón SÍ se estampa (escala 1.22 a 1), la fila se pinta de verde de izquierda a derecha y el título se tacha.
- **Contadores:** Tareas, Pendientes, Ejecutadas y % entran rodando desde arriba cuando cambian.
- **Cinta de avance:** al cambiar el %, la barra se mueve en 0,6 s con las franjas corriendo. Al 100 % la cinta pasa a verde y aparece "Todo ejecutado".
- **Borrar con Deshacer:** la fila sale hacia la izquierda y un aviso negro ofrece Deshacer durante 5 s; las fotos se borran recién cuando vence.
- **Botones físicos:** al presionar, el botón baja 3px y su sombra desaparece.

## Do's and Don'ts

- **Do** usar el amarillo solo para lo seleccionado, lo urgente y el acento.
- **Do** mantener bordes de 2px y esquinas rectas en todo control.
- **Don't** volver a sombras difusas, gradientes suaves ni neumorfismo.
- **Don't** usar Inter, Roboto ni logos o datos de clientes reales.
