# Finanzas

App personal para registrar cuentas, gastos, ingresos, pagos pendientes e inversiones. Se instala en el celular como app (PWA) y se sincroniza con la compu.

- **Datos:** Supabase (proyecto `finanzas-valen`). Cada usuario solo puede leer y escribir sus propios datos (Row Level Security).
- **Publicación:** GitHub Pages, desde la rama `main`.

## Instalar en iPhone

1. Abrí la dirección de la app en **Safari**.
2. Tocá **Compartir** → **Agregar a pantalla de inicio**.
3. Abrila desde el ícono e iniciá sesión.

## Archivos

| Archivo | Para qué |
|---|---|
| `index.html` | La app completa |
| `manifest.webmanifest` | Nombre, ícono y modo pantalla completa |
| `sw.js` | Guarda la app en el celu para que abra rápido |
| `icon-*.png`, `apple-touch-icon.png` | Íconos |

La clave que aparece en `index.html` es la clave pública de Supabase: está pensada para ir en el código del navegador. Los datos los protegen las reglas de la base de datos, no la clave.
