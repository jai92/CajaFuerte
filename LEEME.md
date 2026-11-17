# Mi Caja Fuerte v1.0

Garantías, vencimientos, suscripciones y vacunas y citas de la familia (personas y mascotas).
Funciona sin internet, sin cuentas y sin suscripciones. Todos los datos se guardan en el móvil.

## Cómo sacar la APK

1. Crea un repositorio nuevo en GitHub (por ejemplo `mi-caja-fuerte`).
2. Sube TODO el contenido de esta carpeta, incluida la carpeta oculta `.github`.
   (Si lo subes desde la web de GitHub, arrastra las carpetas; la de `.github/workflows` tiene que quedar tal cual.)
3. Ve a la pestaña **Actions**: se pone a compilar sola (tarda unos 5-8 minutos).
   Si no arranca, entra en "Compilar APK" y pulsa **Run workflow**.
4. Al terminar, abajo del todo aparece **MiCajaFuerte-APK**: descárgalo, descomprime e instala la APK.

## Estructura

- `www/index.html` → toda la app (aquí se hacen los cambios).
- `capacitor.config.json` → nombre y paquete de la app (`es.micajafuerte.app`).
- `assets/` → icono y pantalla de inicio.
- `.github/workflows/build.yml` → compilación automática.

## Primera prueba en el móvil

Ajustes (⚙️) → **Probar un aviso**: acepta el permiso de notificaciones y en 5 segundos te llega un aviso.

## Para publicarla en Google Play (más adelante)

La APK de Actions es de pruebas (debug). Para Play hace falta un AAB firmado con tu clave.
Cuando llegue el momento, se añade al workflow.
