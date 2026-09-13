# Este sitio se mudo

El sitio de Ateliê R.Y. vive ahora en **https://atelie-ry-mooca.pages.dev**

Este repositorio ya no contiene el sitio: solo la redireccion que manda
cualquier ruta de `atelie-ry.vercel.app` a la URL nueva.

## Por que una redireccion y no borrar el proyecto

`atelie-ry.vercel.app` estuvo publicado desde febrero de 2026 y Google
lo indexo. La URL nueva, en cambio, no lo estaba todavia.

Dos sitios distintos con el mismo negocio, el mismo telefono y la misma
direccion compiten entre si: Google reparte las senales de busqueda
local en lugar de sumarlas, y elige el que quiere mostrar. La 301 le
dice explicitamente que uno sustituye al otro, asi que la senal
acumulada pasa al sitio nuevo en vez de perderse.

Borrar el proyecto habria conseguido lo contrario: la URL vieja muere,
Google la retira del indice en unas semanas y los meses de indexacion
no le sirven a nadie. Ademas, cualquier enlace ya compartido —mensajes
de WhatsApp, la biografia de una red— se habria roto.

## Que contenia

Una tarjeta de enlaces de una pagina: nombre, telefono, direccion y
botones a WhatsApp, Instagram, Facebook, TikTok y Google Maps. Todo
ese contenido existe en el sitio nuevo; se comprobo dato por dato
antes de redirigir. El enlace de Maps vive en `src/data/site.json`.

`index.html` y `img/` se conservan en el historial de git. No se
sirven: la redireccion captura todas las rutas.

## No borrar este proyecto de Vercel

La redireccion solo funciona mientras el proyecto siga desplegado. Si
se elimina, los enlaces viejos pasan a dar error y se pierde el
traspaso de senal hacia el sitio nuevo.
