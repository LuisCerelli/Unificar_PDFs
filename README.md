# Fusión de archivos PDF con Streamlit

Este proyecto consiste en una aplicación web sencilla desarrollada con **Streamlit** que permite fusionar múltiples archivos PDF en uno solo de forma rápida y eficiente. Utiliza la librería **PyPDF2** para gestionar la combinación de los documentos PDF.

## ¿Cómo funciona?

La aplicación presenta una interfaz gráfica donde los usuarios pueden adjuntar varios archivos PDF y fusionarlos en uno solo con solo hacer clic en un botón. El resultado se puede descargar directamente desde la aplicación una vez que los documentos han sido fusionados.

### Funcionalidad detallada:

1. **Interfaz gráfica**: Se muestra una imagen en la parte superior de la página con un encabezado y un subtítulo que guía al usuario a adjuntar archivos PDF.
2. **Carga de archivos**: Los usuarios pueden cargar varios archivos PDF simultáneamente mediante un cuadro de carga de archivos.
3. **Fusión de PDFs**: Una vez cargados, al hacer clic en el botón “Fusionar archivos PDF”, el código fusiona todos los archivos PDF adjuntados.
4. **Advertencias**: Si se carga menos de un PDF, la aplicación mostrará una advertencia indicando que se necesita más de un archivo para fusionar.
5. **Descarga del PDF fusionado**: Al finalizar, el PDF combinado está disponible para ser descargado directamente desde la página.

### Ejemplo de uso:

1. Iniciar la aplicación.
2. Adjuntar dos o más archivos PDF mediante el botón de carga.
3. Hacer clic en el botón "Fusionar archivos PDF".
4. Descargar el archivo fusionado cuando esté listo.

### Instrucciones para ejecutar:

1. Instala las dependencias necesarias:
   ```bash
   pip install streamlit PyPDF2
   ```
2. Ejecuta la aplicación en tu terminal:
   ```bash
   streamlit run <nombre_del_archivo>.py
   ```
3. Abre el navegador en la dirección que te proporciona la terminal, y la aplicación estará lista para ser utilizada.

## Utilidad en ingeniería de datos

**Este código es una herramienta útil en el contexto de la ingeniería de datos**, ya que permite la automatización del manejo y combinación de múltiples archivos PDF, algo común en entornos corporativos y de análisis de datos. Al adaptarlo, se podrían combinar diferentes tipos de documentos (como **JPG, DOCX, etc.**) para crear informes unificados o simplificar la gestión documental. Esto puede resultar particularmente útil para los equipos de trabajo que gestionan grandes volúmenes de información, permitiéndoles fusionar documentos técnicos, reportes o cualquier archivo relevante en un solo documento final eficientemente.

### Consideraciones adicionales:

- **Formatos de archivo**: Aunque este código está diseñado para PDF, puede ampliarse para soportar otros formatos de archivo con algunas modificaciones en la lógica de manejo de archivos.
- **Tamaño de archivos**: Ten en cuenta que, al manejar archivos grandes o un alto número de documentos, la memoria disponible del servidor puede ser un factor limitante.
- **Seguridad**: Al tratarse de archivos subidos por los usuarios, se deben tomar en cuenta buenas prácticas de seguridad, como validar los archivos y limitar los tipos de contenido admitido.
