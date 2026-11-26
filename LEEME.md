# Política Nuclear — proyecto de APK (Android 5.0 o superior; tu J7 con Android 8.1 funciona)

La app es un envoltorio mínimo (WebView a pantalla completa, horizontal, pantalla siempre encendida) que carga el juego
desde `app/src/main/assets/index.html`. Los logros y ajustes se guardan en el teléfono.

## Opción A (la más simple, sin instalar nada): abrir el HTML en el teléfono
1. Pasa `politica-nuclear.html` al teléfono (WhatsApp, Drive, cable USB).
2. Ábrelo con Chrome. Pon el teléfono en horizontal y activa "Modo ahorro" en el menú.

## Opción B: compilar el APK con Android Studio (gratis, en una PC)
1. Instala Android Studio.
2. `File > Open` y elige esta carpeta. Espera a que termine la sincronización (descarga sola lo necesario).
3. `Build > Build Bundle(s) / APK(s) > Build APK(s)`.
4. El archivo queda en `app/build/outputs/apk/debug/app-debug.apk`. Cópialo al teléfono e instálalo
   (permite "instalar apps de orígenes desconocidos" cuando te lo pida).

## Opción C: que GitHub lo compile por ti (sin instalar nada en la PC)
1. Crea un repositorio privado en github.com y sube el contenido de esta carpeta (incluida `.github`).
2. En la pestaña **Actions** ejecuta "Construir APK" (Run workflow).
3. Al terminar, descarga el APK desde "Artifacts".

## Para actualizar el juego
Reemplaza `app/src/main/assets/index.html` por la versión nueva de `politica-nuclear.html` y vuelve a compilar.
