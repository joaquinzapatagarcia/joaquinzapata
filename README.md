# joaquinzapata.com — Letrero digital

Primera versión del SITE personal de Joaquín Zapata.

## Concepto

Un despacho editorial vivo que conecta:

1. **Criterio** — una mini columna o parte de situación.
2. **Sistema** — tres indicadores editoriales JISR.
3. **Aplicación** — una pauta práctica para el día.
4. **Oferta** — tres sesiones: Situación, Posición y Oferta.
5. **Conversión** — entrada directa por WhatsApp.

## Publicación con GitHub Pages

El SITE no necesita compilación ni dependencias. Está contenido en `index.html`.

En GitHub:

1. Abre **Settings**.
2. Entra en **Pages**.
3. En **Build and deployment**, selecciona **Deploy from a branch**.
4. Elige la rama `main` y la carpeta `/ (root)`.
5. Guarda los cambios.

Después puede conectarse el dominio `joaquinzapata.com` desde la misma sección de Pages.

## Configuración pendiente de WhatsApp

En la parte final de `index.html` aparece:

```js
const whatsappNumber = '';
```

Debe sustituirse por el número completo con prefijo internacional, sin `+`, espacios ni guiones.

Ejemplo para España:

```js
const whatsappNumber = '34600111222';
```

Mientras el número esté vacío, el botón abre WhatsApp con el mensaje preparado, pero no fija destinatario.

## Actualización editorial

La primera edición está escrita directamente dentro de `index.html`. Para actualizarla, deben modificarse:

- la fecha del teletipo;
- el título y cuerpo del Parte de situación;
- los tres valores JISR;
- las frases breves de interpretación;
- el bloque **Para hoy**.

Una evolución posterior puede separar el contenido en un archivo JSON o Markdown y automatizar la publicación diaria sin alterar el diseño.

## Diseño

- HTML, CSS y JavaScript nativos.
- Sin framework ni proceso de compilación.
- Responsive para escritorio y móvil.
- Tipografías: Newsreader, Manrope y DM Mono.
- Estética editorial, minimalista y de teletipo.
