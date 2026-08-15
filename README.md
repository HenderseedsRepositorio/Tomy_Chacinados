# El Salvador de Henderson — Chacinados

Sitio de venta y estudio de marca. Todo estático: dos archivos HTML autónomos, sin dependencias, sin build, sin servidor.

## Qué es cada archivo

| Archivo | Qué es | Quién lo usa |
|---|---|---|
| `index.html` | **La tienda.** Landing con catálogo y carrito que arma el pedido por WhatsApp. | Los clientes |
| `estudio.html` | **El tablero de control.** Pestaña 1 previsualiza la landing, pestaña 2 configura marca, paleta, tipografía, productos y precios. | Vos |
| `.nojekyll` | Le dice a GitHub Pages que publique los archivos tal cual. No lo borres. | — |

## Publicar

1. Subí estos archivos a la raíz del repo.
2. En GitHub: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**.
3. Al minuto queda en `https://TU-USUARIO.github.io/TU-REPO/`

El estudio queda en `https://TU-USUARIO.github.io/TU-REPO/estudio.html`

## Cómo cambiar la tienda

1. Abrí `estudio.html` (online o el archivo local, da igual).
2. Cambiá lo que quieras en la pestaña **Configurador**: nombre, logo, paleta, tipografía, productos, precios, teléfono.
3. Mirá cómo queda en la pestaña **Landing**.
4. Tocá **⤓ Descargar index.html**.
5. Subí ese archivo al repo reemplazando el anterior.

Desde la web de GitHub: entrás al repo → clic en `index.html` → ícono del lápiz → o más simple, **Add file → Upload files** y arrastrás el nuevo `index.html` (te pregunta si querés reemplazarlo).

> Lo que cambiás en el estudio **no se publica solo**. Hay que descargar y subir. Es a propósito: así podés probar veinte variantes sin romper la tienda que está online.

## No perder tus elecciones

El estudio no guarda nada en ningún lado. Para conservar tu configuración:

- **🔗 Copiar link con mi config** — te da un link que lleva todo adentro. Guardátelo o mandátelo por WhatsApp. Al abrirlo vuelve todo como lo dejaste, en cualquier dispositivo.
- **⤓ Respaldo .json** — descarga un archivo con la configuración, que después cargás con **↥ Cargar respaldo**.

## Antes de dar a conocer el sitio

- [ ] Cambiar el **teléfono de WhatsApp** (arranca en ceros)
- [ ] Cambiar los **precios** (los que están son inventados, sólo para maquetar)
- [ ] Revisar descripciones y presentaciones de cada producto
- [ ] Cargar el usuario de **Instagram** si lo tienen
- [ ] Sacar fotos propias de cada producto y pegarlas en el campo *Foto* del editor
- [ ] Completar **RNE / RNPA** en el pie cuando salgan los trámites

## Detalles técnicos

- Un solo archivo por página. Fuentes (woff2 subseteadas), fotos y logo van embebidos en base64.
- Funciona sin conexión una vez cargado. No usa CDN, ni analytics, ni cookies, ni almacenamiento del navegador.
- El símbolo de la marca es el hierro de marca ganadera **382297** (partido de Hipólito Yrigoyen, vigente hasta 24/05/2032), vectorizado desde el boleto original.
- `index.html` pesa ~530 KB, `estudio.html` ~920 KB. Muy por debajo del límite de GitHub Pages.

## Dominio propio (opcional)

Comprás el dominio, agregás un archivo `CNAME` en la raíz con el dominio adentro, y en **Settings → Pages → Custom domain** lo cargás. El HTTPS lo genera GitHub solo.
