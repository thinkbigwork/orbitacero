# Órbita Cero — Wizor Space

Maqueta de landing page y research de mercado del programa de acceso a microgravedad de **Wizor Space** para empresas, investigadores y universidades de América Latina.

## Contenido

| Archivo | Qué es |
|---|---|
| `index.html` | Maqueta de la landing, v3. Autocontenida: un solo archivo con HTML, CSS y JS inline. |
| `docs/investigacion-mercado.md` | Investigación de mercado: proveedores, usuarios, experimentos, oportunidad Latam, productos, modelo de negocio y pricing. Con fuentes citadas. |

Para verla, abrir `index.html` en cualquier navegador. No requiere build ni dependencias.

## Arquitectura de marca

Marca endosada: **Wizor Space** es la casa, **Órbita Cero** es el programa. El lockup del encabezado y el pie es el logo de Wizor Space, un separador y la palabra ÓRBITA CERO. En el habla queda «Órbita Cero, de Wizor Space»; el título de la página es «Órbita Cero — Wizor Space». No se usa «Wizor Space Órbita Cero» como cadena única.

## Sistema visual heredado de space.wizor.io

Los tokens salieron de los estilos reales del sitio padre, no de una aproximación:

| Token | Valor | Origen |
|---|---|---|
| `--bg` | `#000000` | Wizor `--bg-color` |
| `--panel` | `#050505` | Wizor `--glass-bg` |
| `--line` | `#222222` | Wizor `--glass-border` |
| `--text` | `#ffffff` | Wizor `--text-main` |
| `--muted` | `#b8b8b8` | Wizor `--text-muted` |
| `--body` | `#d1d5db` | Wizor, color de párrafo |
| `--wz` | `#4ade80` | Wizor `--wizor-green` — foco y hover, mismo rol funcional que en el padre |
| `--oc` | `#ff5a1f` | acento propio de Órbita Cero |

- **Tipografía:** Space Grotesk 400/700 para todo lo display, en mayúsculas; Inter 300/400/600 para texto corrido. Son las dos familias del sitio padre.
- **Botones:** sin radio, borde de 1 px, mayúsculas, Space Grotesk 600, `letter-spacing: 2px`, `padding: 16px 32px`. Calcados del padre; el relleno sólido va en naranja en lugar de blanco, que es donde Órbita Cero se distingue.
- **Etiquetas de sección:** Space Grotesk en mayúsculas con `letter-spacing: 3px`, el mismo patrón que el `.rm-meta` del roadmap de Wizor.

**Para volver la página monocroma como el padre**, cambiar `--oc` por `#4ade80` y `--oc-soft` por `#bbf7d0` en `:root`. Es un solo lugar.

## ⚠️ Antes de publicar: hay imágenes sin licenciar

La maqueta usa **fotografías y un video de terceros**, tomados de los sitios públicos de Novespace / Air Zero G y de Zero Gravity Corporation, **sólo como referencia visual para el equipo de diseño**. La mayoría de las fotos de Zero-G son de Steve Boxall.

Estas imágenes no están licenciadas, están referenciadas por hotlink a los servidores de origen y deben reemplazarse por material propio o licenciado antes de cualquier publicación. **No activar GitHub Pages ni ningún otro hosting sobre este repositorio mientras siga la franja amarilla de advertencia en el encabezado.**

El logo y la imagen de astronauta de Wizor Space sí son propios y pueden quedarse.

**La vía más barata para resolverlo es el contrato con Air Zero G que está en curso:** conviene negociar los derechos de uso de material gráfico dentro de ese acuerdo (fotos, video, logos y guía de marca). Con eso cubierto, las imágenes de Zero-G se reemplazan por las de Air Zero G, que va a ser el operador ancla. A mediano plazo, lo mejor sigue siendo material propio: fotos con investigadores latinoamericanos a bordo valen bastante más que las de cualquier operador.

### Sobre el descargo de afiliación

El pie tenía la línea «Wizor Space no está afiliada a ninguno de esos operadores». Se quitó a propósito: deja de ser cierta al firmar con Air Zero G. Una vez firmado conviene reemplazarla por lo contrario —«Órbita Cero opera con Air Zero G / Novespace»—, que es un argumento de venta y no un descargo: es el único dato de la página que un investigador no puede verificar por su cuenta. Mientras tanto la maqueta no debe circular fuera del equipo, porque lleva fotos de ambos operadores sin licencia ni aclaración.

## Pendientes de contenido

- **Los tres nombres de la tripulación**, con foto real y la credencial del astronauta. Hoy la sección dice `[Nombre]` y es el bloque más importante de la página.
- **Validar la sección de telemetría.** Afirma que podemos instrumentar a los investigadores que vuelan con la stack de Wizor. Es una propuesta: hay que confirmar que el hardware puede volar y pasar el expediente de seguridad del operador antes de ofrecerlo en firme.
- **Precios.** Son una propuesta calculada sobre un margen del 20–25% por encima de los precios públicos de los operadores. Validar contra costos reales una vez negociada la capacidad.
- **Ancla de comparación con la ISS** en la sección de inversión: falta un número público y defendible del costo de poner un experimento en la estación espacial.
- **Wizor Education.** El concurso «Tu tesis en gravedad cero» y la cátedra deberían integrarse al programa educativo que ya existe, no correr aparte.

## Dato de contexto que define la estrategia

Al momento de la investigación (septiembre de 2026) el avión de Zero-G está fuera de servicio y no se espera que vuelva antes de mediados de 2027, y los vuelos públicos de Air Zero G están agotados hasta octubre de 2027. El cuello de botella del negocio es el **acceso**, no el precio. El detalle completo está en `docs/investigacion-mercado.md`.
