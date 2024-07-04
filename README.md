# Motor de Búsqueda de Imágenes de Moda

## Descripción General
Este proyecto desarrolla un motor de búsqueda de imágenes de moda utilizando aprendizaje profundo para analizar y recuperar artículos de moda similares de un amplio conjunto de datos. El proyecto utiliza una red neuronal convolucional (CNN) basada en la arquitectura VGG16 para extraer características de las imágenes y realiza comparaciones de similitud utilizando la distancia coseno.

## Características
- **Extracción de Características de Imágenes:** Utiliza VGG16 para extraer características relevantes de imágenes de productos de moda.
- **Búsqueda de Similitudes:** Implementa la similitud del coseno para encontrar los artículos más similares basados en el contenido de la imagen.
- **Búsqueda Eficiente:** Las características y los modelos se precalculan y guardan para mejorar la eficiencia de la búsqueda y el tiempo de respuesta.
- **Verificación Visual:** Integración de matplotlib para la confirmación visual de la recuperación de imágenes similares.

## Conjunto de Datos
El conjunto de datos incluye imágenes de productos de alta resolución tomadas profesionalmente, cada una identificada por un ID único. Los metadatos de cada producto están disponibles en `styles.csv`, con imágenes almacenadas como `images/{product_id}.jpg`.

- **Fuente:** [Conjunto de Imágenes de Productos de Moda en Kaggle](https://www.kaggle.com/paramaggarwal/fashion-product-images-dataset)
- **Contenido:** Imágenes de productos de alta resolución con metadatos asociados que describen las características del producto.

## Prerrequisitos
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
   git clone https://github.com/tuusuario/motor-busqueda-imagenes-moda.git
   ```
2. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```

## Uso
Para empezar a usar el motor de búsqueda de imágenes de moda, sigue estos pasos:
1. Carga el conjunto de datos y preprocesa las imágenes.
2. Ejecuta la extracción de características:
   ```python
   python extraccion_caracteristicas.py
   ```
3. Realiza una búsqueda de imágenes ejecutando:
   ```python
   python buscar.py --ruta_imagen 'ruta/a/imagen.jpg'
   ```

## Ejemplo
Para encontrar artículos de moda similares a una imagen de producto dada:
```bash
python buscar.py --ruta_imagen 'fashion-dataset/images/42431.jpg'
```

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
