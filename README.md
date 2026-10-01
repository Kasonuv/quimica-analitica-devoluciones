# Devoluciones del Primer Parcial — Química Analítica

Sitio estático preparado para GitHub Pages.

## Qué hace
- El estudiante ingresa su número de legajo.
- Se carga únicamente el archivo cifrado asociado a ese legajo.
- Muestra una devolución personalizada, organizada problema por problema.
- El botón **Imprimir / Guardar como PDF** genera una versión A4 limpia de la devolución.
- El botón **Ver resolución completa** muestra la resolución de los cinco problemas con ecuaciones y unidades mediante MathJax.
- La resolución se excluye automáticamente de la impresión/PDF y no se publica como archivo PDF descargable.

## Estructura
- `index.html`
- `robots.txt`
- `data/` — devoluciones cifradas individualmente.

## Publicar manualmente en GitHub Pages
1. Crear un repositorio nuevo en GitHub.
2. Subir **todo el contenido** de esta carpeta conservando la carpeta `data`.
3. Abrir `Settings` → `Pages`.
4. En `Build and deployment`, elegir `Deploy from a branch`.
5. Seleccionar la rama `main` y la carpeta `/ (root)`.
6. Guardar.
7. GitHub mostrará la URL pública del sitio.

## Privacidad: alcance real
Este diseño cifra cada devolución y utiliza el legajo para derivar la clave de descifrado. Esto evita que las devoluciones aparezcan legibles al inspeccionar los archivos del sitio.

Sin embargo, **el legajo no es una contraseña fuerte**. Al ser un identificador de baja entropía, una persona técnicamente capacitada podría intentar adivinar legajos de terceros. Si se requiere confidencialidad fuerte, hace falta autenticación real (por ejemplo, un backend o un segundo factor).

## Resoluciones "no descargables"
No existe una forma técnica de impedir por completo que alguien conserve contenido que puede ver en su navegador: puede copiarlo, inspeccionar el código o hacer capturas de pantalla.

Este sitio:
- no ofrece un archivo de resolución para descargar;
- deshabilita el menú contextual dentro de la resolución;
- dificulta la selección directa del texto;
- excluye toda la resolución al imprimir o guardar la devolución como PDF.

## Prueba recomendada
Antes de publicar al curso:
1. subir el sitio;
2. probar 2 o 3 legajos;
3. revisar la impresión PDF;
4. revisar la visualización de ecuaciones desde celular.
