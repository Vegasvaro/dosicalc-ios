Este directorio debe contener la build web final para publicar en GitHub Pages.

Generacion local (cuando tengas Flutter en PATH):

  cd flutter_ios
  flutter pub get
  flutter build web --release --base-href "/<NOMBRE_REPO>/"

Luego sube todo el contenido de build/web al repositorio.

Tambien puedes usar el workflow `.github/workflows/build_web.yml` para que GitHub genere automaticamente esta carpeta en cada push a `main`.
