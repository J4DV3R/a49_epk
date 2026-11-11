# A-49 · Web de la banda

Web estática de A-49 (HTML, CSS y JavaScript, sin dependencias ni compilación).

## Estructura

```
index.html            Página completa (estilos y scripts incluidos)
img/                  Logo, fotos de la sesión y del directo
favicon.png           Icono de la pestaña
apple-touch-icon.png  Icono al guardar la web en el móvil
og-image.jpg          Imagen al compartir el enlace (WhatsApp, redes…)
.nojekyll             Indica a GitHub Pages que sirva los archivos tal cual
```

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `a49-web`) y márcalo como **Public**.
2. En el repositorio, pulsa **Add file → Upload files** y arrastra **todo el contenido de esta carpeta** (no la carpeta en sí: `index.html` tiene que quedar en la raíz del repositorio). Pulsa **Commit changes**.
   - El archivo `.nojekyll` está oculto en algunos sistemas. Si no se sube, no pasa nada: la web funciona igual.
3. Ve a **Settings → Pages**.
4. En **Build and deployment → Source** elige **Deploy from a branch**.
5. En **Branch** elige `main` y la carpeta `/ (root)`. Pulsa **Save**.
6. En uno o dos minutos la web estará en `https://TU-USUARIO.github.io/a49-web/`. El enlace aparece arriba en esa misma página de Settings → Pages.

Para actualizar la web, vuelve a subir los archivos cambiados con **Upload files**; GitHub Pages la republica sola.

## Desde la terminal (opcional)

```bash
git init
git add .
git commit -m "Web de A-49"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/a49-web.git
git push -u origin main
```

Después, activa Pages como en los pasos 3 a 5.

## Dominio propio (opcional)

En **Settings → Pages → Custom domain** escribe tu dominio (por ejemplo `a49banda.com`) y configura en tu proveedor de dominio un registro CNAME que apunte a `TU-USUARIO.github.io`.
