# Motor de Búsqueda de Imágenes de Moda

## Descripción General
Este proyecto desarrolla un motor de búsqueda de imágenes de moda completamente implementado en un Jupyter Notebook, utilizando aprendizaje profundo para analizar y recuperar artículos de moda similares de un amplio conjunto de datos. Utiliza una red neuronal convolucional (CNN) basada en la arquitectura VGG16 para extraer características de las imágenes y realiza comparaciones de similitud utilizando la distancia coseno.

## Características
- **Extracción de Características de Imágenes:** Utiliza VGG16 para extraer características relevantes de imágenes de productos de moda.
- **Búsqueda de Similitudes:** Implementa la similitud del coseno para encontrar los artículos más similares basados en el contenido de la imagen.
- **Búsqueda Eficiente:** Las características y los modelos se precalculan y guardan dentro del Notebook para mejorar la eficiencia de la búsqueda y el tiempo de respuesta.
- **Verificación Visual:** Integración de matplotlib dentro del Notebook para la confirmación visual de la recuperación de imágenes similares.

## Conjunto de Datos
Debido al gran tamaño del conjunto de datos (25GB), no está incluido en el repositorio. Para utilizar este proyecto correctamente, deberás descargar el conjunto de datos y colocarlo en la estructura del proyecto.

### Descarga e Instalación del Conjunto de Datos
1. Descarga el conjunto de datos desde [Fashion Product Images Dataset on Kaggle](https://www.kaggle.com/paramaggarwal/fashion-product-images-dataset).
2. Extrae el archivo descargado en la carpeta `data` en la raíz de este proyecto. Si la carpeta no existe, créala.
   ```bash
   mkdir -p data
   unzip fashion-product-images-large.zip -d data

## Prerrequisitos
- Jupyter Notebook
- Python 3.8+
- TensorFlow 2.x
- NumPy
- Pandas
- Matplotlib
- PIL
- Scikit-learn

## Configuración e Instalación
1. Clona el repositorio:
   ```bash
   git clone https://github.com/LargoLujan/fashion_image_search_engine.git
   ```
2. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```
3. Abre el Jupyter Notebook:
   ```bash
   jupyter notebook image_recognition.ipynb
   ```

## Uso
Dentro del Jupyter Notebook, sigue las celdas paso a paso para cargar el conjunto de datos, preprocesar las imágenes, extraer características y realizar búsquedas de imágenes similares.

## Ejemplo de Uso
Para encontrar artículos de moda similares a una imagen de producto dada, sigue las instrucciones dentro del notebook para cargar la imagen y ejecutar la celda de búsqueda.

## Contribuciones
¡Las contribuciones a este proyecto son bienvenidas! Por favor, consulta las pautas de contribución para más detalles.

## Contacto
- **Manuel Lujan Vilchez**
- Correo: mlujan@invokeapp.io
- LinkedIn: [Manuel Lujan Vilchez](https://www.linkedin.com/in/manuel-lujan-vilchez-166499b1)

## Licencia
Este proyecto está licenciado bajo la Licencia MIT - ver el archivo [LICENSE.md](LICENSE) para detalles.

## Agradecimientos
Gracias a Param Aggarwal por proporcionar el conjunto de datos e inspirar el desarrollo de este proyecto.
