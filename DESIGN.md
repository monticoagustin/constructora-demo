---
name: OBRAS (Constructora Demo)
description: Checklist de obra genérico, crema sobre noche con amarillo de acento, con portada de venta.
colors:
  noche: "#121212"
  noche-2: "#1C1C1C"
  crema: "#F6F3EC"
  crema-2: "#EEE9DD"
  tinta: "#17171A"
  tinta-suave: "#5B574E"
  amarillo: "#F5B700"
  amarillo-suave: "#FFF0C2"
  ok: "#1D7044"
  ok-fondo: "#E3F0E6"
  peligro: "#B3262E"
typography:
  display:
    fontFamily: "Anybody"
    fontWeight: 800-900
    fontStretch: "110-150%"
  cuerpo:
    fontFamily: "Instrument Sans"
    fontSize: "15px"
rounded:
  pieza: "8px"
  control: "12px"
  tarjeta: "18px"
  pildora: "999px"
---

# Design System: OBRAS

## Overview

Marca genérica **OBRAS** (casita amarilla + palabra en Anybody extendida). Fondo noche, tarjetas crema redondeadas, un solo acento amarillo. Reemplaza al estilo Señalética (2026-11-14), a partir de una referencia que eligió el usuario.

- Todo el estilo vive en `<style id="skin-obras">` de `index.html`; fuentes Anybody e Instrument Sans (OFL) en `fonts/`; íconos Tabler (MIT) embebidos.
- **Portada de venta** (`#portada`): siempre se ve al entrar a teskel.online/constructora. "Abrir la app" pasa a `#app` (recargar ahí sigue en la app); `#app` abre la app directo y la PWA instalada arranca ahí; "Ver portada" vuelve.
- Portada: "OBRAS" gigante, losa amarilla con grúas dibujadas en SVG (sin fotos de stock), ventana de la app con datos de muestra, funciones, roles y cierre. Si se consiguen fotos reales, reemplazan la losa.

## Colors

Noche para la página y el encabezado; crema para tarjetas; amarillo para la acción principal, la pestaña y el filtro activos, la obra seleccionada, el aviso "Vencen mañana" y la barra de avance. Verde solo para ejecutado, siempre con la palabra SÍ.

## Typography

Títulos y cifras en Anybody 800-900 extendida; texto en Instrument Sans. Cifras del resumen grandes (52px).

## Shapes & Depth

Tarjetas de 18px, controles de 12px, botones y pestañas en píldora. Sombra suave solo para separar tarjetas del fondo noche.

## Motion

- Portada: las letras de OBRAS suben una vez, la losa se despliega, la ventana entra y sus números cuentan; el gancho de la grúa se mueve lento.
- App: sello al tildar, contadores que ruedan, cinta de avance que corre, borrar con Deshacer (5 s), botones que se achican al presionar.
- Todo se apaga con "reducir movimiento".

## Don'ts

- Nada de logos, nombres ni datos de clientes reales; no inventar precios ni testimonios en la portada.
- No volver al neumorfismo ni a bordes de color a un costado.
- No usar Archivo (es de la identidad de otro proyecto), Inter ni Roboto.
