CAJA DE INSUMOS - proyecto Android

OPCION A (recomendada): sacar el APK con GitHub, sin instalar nada
1. Crea un repositorio en GitHub (puede ser privado).
2. Sube TODO el contenido de esta carpeta a la raiz del repositorio:
   las carpetas "app" y ".github", y los archivos build.gradle, settings.gradle,
   gradle.properties y .gitignore.
   - Si la carpeta oculta ".github" no se sube al arrastrar, usa
     "Add file > Create new file", escribe como nombre:  .github/workflows/apk.yml
     y pega alli el contenido del archivo apk.yml.
3. Entra a la pestana "Actions", elige "Generar APK" y toca "Run workflow".
   (Tambien corre solo cada vez que subes un cambio.)
4. En unos 5 a 10 minutos termina con una marca verde. Abre esa ejecucion y,
   en "Artifacts", descarga "Caja-de-insumos-apk". Dentro esta app-debug.apk.
5. Pasa el APK al celular, abrelo y permite instalar apps de origen desconocido.

OPCION B: compilar en tu computadora con Android Studio
1. Instala Android Studio (https://developer.android.com/studio) y abre esta carpeta.
2. Espera "Gradle sync" y acepta las descargas.
3. Build > Build Bundle(s) / APK(s) > Build APK(s). El archivo queda en
   app/build/outputs/apk/debug/app-debug.apk

Notas:
- Los datos se guardan SOLO en el celular. Si desinstalas la app o borras sus datos, se pierden.
- La app no necesita internet.
- Boton "Guardar reporte en PDF": abre la ventana de impresion de Android. Elige
  "Guardar como PDF" y toca guardar; luego puedes compartir el PDF por WhatsApp.
- Para cambiar la pagina, edita app/src/main/assets/index.html y vuelve a generar el APK.
