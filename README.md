# Arco Nova

Tienda virtual de Arco Nova (Costa Rica): tenis, joyería, relojes, lentes, bolsos, termos, ropa, belleza, accesorios y más. Los pedidos se envían por WhatsApp; la página no cobra.

**Sitio:** https://cbgrowth.github.io/arco-nova/

## Qué incluye

- Intro animada con el logo y carrusel de productos en el inicio.
- Catálogo por categorías y subcategorías, con buscador, orden por precio y fichas de producto con galería.
- Bolsa de compras: la clienta agrega todo lo que quiera, completa sus datos y el pedido completo se abre en WhatsApp con número de pedido.
- Cupón de bienvenida del 3% (seguir en Instagram) y ruleta de descuentos del 1% al 5%; ambos se guardan en la bolsa y viajan con el pedido para que la vendedora los verifique.
- Favoritos, historias, lookbook, joyero "arma tu set", preguntas frecuentes, guía de tallas y modo oscuro.
- Diseño adaptado a celular con barra de navegación inferior.

## Estructura

```
index.html   Página completa (HTML, CSS y JavaScript en un solo archivo)
img/         Logo, fotos de productos y videos
.nojekyll    Hace que GitHub Pages sirva los archivos tal cual
```

## Cómo editar

Todo se edita dentro de `index.html`:

| Qué | Busca |
|---|---|
| Productos, precios, fotos y opciones | `DEFAULT_PRODUCTS` |
| Categorías y subcategorías | `const GROUPS` |
| Número de WhatsApp | `50664729998` |
| Premios y probabilidades de la ruleta | `const SEG` y `const ODDS` |
| Cupón de bienvenida (3%, 14 días) | `pct:3` y `14*864e5` |
| Reseñas | `Espacio para una reseña real` |
| Pago con tarjeta (hoy "próximamente") | `Tarjeta (próximamente)` |

Para agregar un producto: sube su foto a `img/` en formato `.webp` y agrega una línea en `DEFAULT_PRODUCTS` con `cat` (categoría) y, si aplica, `sub` (subcategoría).

## Pendientes antes del lanzamiento

- Confirmar los precios marcados como estimados.
- Reemplazar las reseñas de ejemplo por reseñas reales.
- Reemplazar las fotos de referencia de tenis (Unsplash) por fotos del inventario.
