# Fichas técnicas CALEFACCIÓN

Generador de fichas técnicas de producto en PDF (BigMat) a partir de un Excel. Todo se procesa en el navegador: no se sube ningún dato.

## Uso

1. Abre `index.html` (en el navegador o desde GitHub Pages). Al abrirla no se muestra ninguna ficha: aparece «Carga un Excel para ver la vista previa.»
2. Importa la BBDD en Excel y la carpeta de imágenes y logos.
3. Elige el tamaño de ficha (A4 o A5) y descarga:
   - **Descargar PDF de esta ficha**: la ficha que ves en la vista previa.
   - **Descargar un PDF por ficha**: descarga todas las fichas una a una, en archivos PDF separados (sin ZIP), cada uno con el código de producto (CODIGO_LN, 8 dígitos) como nombre. Si el navegador lo pide, permite las descargas múltiples.

El PDF sale en hoja A4 con la ficha centrada y líneas de corte hasta los bordes del papel. Una ficha por hoja.

## Formato del Excel

Una fila por producto. Columnas principales: `CODIGO_LN`, tipología, modelo, características, «Incluye» («Apto para») y «Añade y mejora tu compra», más los nombres de las imágenes. Los códigos se completan a 8 dígitos.

## Colores de la ficha

| Elemento | Color |
|---|---|
| Fondo de la ficha | `#ffffff` |
| Texto general | `#1a1a1a` |
| Banda de cabecera, líneas de la tabla, marcos y etiquetas Incluye/Añade, barras de pie | `#0f498b` |
| Texto de cabecera y de etiquetas | `#ffffff` |
| Filas grises de características (1.ª, 3.ª, 5.ª) | `#dbdbdb` |
| Nombre de la característica | `#1f2c44` |
| Texto «Ref.» | `#4b5563` |
| Recuadro discontinuo de la Ref. y líneas de corte | `#cfd4dc` |
| Borde de Asesoramiento profesional | `#e1e2f1` |
| Texto del hueco vacío de imagen | `#b6bccb` |

## Archivos

- `index.html`: la aplicación completa (HTML, CSS y JS en un solo fichero).
- `README.md`: este documento.

## Publicar en GitHub Pages

1. Sube `index.html` y `README.md` a la raíz del repositorio.
2. En *Settings → Pages*, elige la rama `main` y la carpeta `/ (root)`.
3. La app quedará disponible en `https://<usuario>.github.io/<repositorio>/`.

## Librerías (CDN, versión fijada)

XLSX 0.18.5, jsPDF 2.5.1, html2canvas 1.4.1 y fuente Montserrat.
