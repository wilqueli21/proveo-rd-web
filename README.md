# Sitio web de Proveo RD

Página pública de **Proveo RD** (licitaciones: vender al Estado dominicano) y **Proveo Finanzas** (facturación para pymes),
pensada para enlazarla desde el perfil de Instagram y las demás redes.

- Dos páginas sin compilación: `index.html` (Proveo RD, con un resumen de Proveo Finanzas) y `finanzas.html` (todo lo
  que hace Proveo Finanzas), con los estilos compartidos en `estilos.css`. Se publica con GitHub Pages desde `main`.
- Lo que dice `finanzas.html` sale del README y el código de `nexo-rd` y de las respuestas del bot del hub de redes. La
  factura electrónica (e-CF) se presenta «en preparación» porque el módulo fiscal sigue bloqueado para producción.
- Marca: «proveo» en Plus Jakarta Sans con el punto dorado y «RD» (propuesta E, «Punto final», escogida el 26/10/2026).
  Colores: marino `#0F1E35`, oro `#C9A55C`, oro para texto sobre blanco `#A07C34`.
- Los textos salen de lo que los sistemas hacen hoy (README de licita-rd y del hub de redes): nada de precios, clientes ni
  garantías inventados. Los enlaces de privacidad y de borrado de datos apuntan al centro de mensajes en Cloudflare.
- `perfil.png` es la misma foto de perfil de Instagram; sirve de imagen para compartir el enlace y de ícono en el celular.

`entrar.html` es la página «Iniciar sesión», con una tarjeta por sistema. Los destinos de los botones están en los enlaces
con id `entrar-proveo` y `entrar-finanzas`; hoy apuntan a las direcciones locales de los sistemas instalados en la PC
(Proveo RD en `http://localhost:5173/`, la `FRONTEND_BASE_URL` de su API; Proveo Finanzas en `http://127.0.0.1:8787/`).
Cuando existan las direcciones en la nube (Proveo Finanzas: `docs/despliegue-cloudflare.md` de nexo-rd), se cambian ahí.

Para cambiar algo: edita `index.html`, haz commit y push a `main`; GitHub Pages lo publica en uno o dos minutos.
