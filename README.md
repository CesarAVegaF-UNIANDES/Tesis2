En el presente repositorio encontrara los scripts utilizados en esta investigación, donde se presentan los experimentos realizados, teniendo en cuenta las siguientes componentes: 

  * Los sistemas FAS seleccionados: Silent FAS, Liveness Detection FAS y Object FAS.
  * los conjuntos de imágenes con ejemplos de ataques de presentación: CASIA y Sustitución (Generado en esta investigación).
  * Los conjuntos de imágenes con ejemplos de manipulación digital: StyleGAN (Generadas por NVIDIA) y Difusión (Generado en esta investigación).


En la carpeta Fine_Tuning se encuentra el script de google colab con el cual se hiso los Experimentos mencionados en esta investigación, en el cual encontrara las instrucciones para la ejecución y replicación del entrenamiento de los modelos. Para esto se requiere descargar los conjuntos de datos en el siguiente enlace

https://drive.google.com/drive/folders/1gycc4CS_B1LZeisjAYcC4dvhTNS1hZYV?usp=share_link

Carpeta Fine_tuning

En esta carpeta se encuentra el script "Tesis\_Reentrenamiento\_modelos.ipynb" elaborado en Google Colab con el cual se realizó el tuneo sobre los modelos seleccionados, en primer lugar en la sección "Características del modelo" podrá encontrar una descripción detallada de la arquitectura de cada modelo a usar. En la segunda sección "Preprocesamiento de imágenes para cada uno de las arquitecturas" se realiza la transformación de las imágenes según lo solicita cada uno de los modelos usados. Y por ultimo, en la sección "Reentrenamiento de modelos" se detalla el proceso del tuneo de los modelos seleccionados en cada uno de los experimentos explicados en el Capitulo 3.

Carpeta Métricas

En esta carpeta se encuentra el script "Tesis2\_Metricas.ipynb" elaborado en Google Colab con el cual se calcularon las métricas presentadas en este proyecto, se compone principalmente de 3 secciones "Métricas con todo el conjunto de imágenes", "Métricas con el subconjunto de imágenes de pruebas" y "Métricas con el subconjunto de imágenes de pruebas después de entrenamiento". En la primera sección "Métricas con todo el conjunto de imágenes" se evalúa en una primera instancia los modelos sin el tuneo, esto con el fin de calcular el comportamiento de los modelos con todo el conjunto de datos. En la siguiente sección del programa "Métricas con el subconjunto de imágenes de pruebas" se evalúan los modelos antes del tuneo con el fin de calcular los resultados presentados en el Experimento 1 (Sección 3.3.2) y tener estos como base para la comparación concerniente a los siguientes experimentos. y por ultimo, en la sección "Métricas con el subconjunto de imágenes de pruebas después de entrenamiento" se evalúan los subconjuntos de pruebas con los modelos con Fine Tuning, los resultados obtenidos de esta sección fueron presentados en los Experimentos 2-5 en la sección 3.3 de este documento.

Carpeta Modelos

En esta carpeta se encuentra diferenciados para cada uno de los modelos usados "0\_Silent\_FAS", "1\_Liveness\_Detection\_FAS" y "2\_Objects\_FAS", los modelos resultantes después del Fine Tuning con cada uno de los subconjuntos de entrenamiento, estos modelos se encuentran en las subcarpetas referenciadas para cada conjunto de datos usado: Base, CASIA, SUBSTITUTION, DIFFUSION, StyleGAN y ALL, en sus respectivo formato. En donde la carpeta "Base" es donde se encuentra almacenado el modelo sin tuneo y en la carpeta "ALL", es donde se encuentra almacenado el modelo cuando se hizo Fine Tuning usando todos los subconjuntos de entrenamiento, en caso de los otras carpetas los modelos respectivos para cada unos de los subconjuntos.

Carpeta Prototipo

En esta carpeta se encuentran dos subcarpetas "Códigos" y "Train", en las cuales como su nombre lo indica en la carpeta de "Códigos" se encuentra almacenado el código implementado en cada uno de los modelos usados en este proyecto. Por otro lado en la carpeta "Train" se encuentran los subconjuntos de imágenes transformados para el modelo en formato .zip. Con estos datos es posible replicar los resultados obtenidos en esta investigación ejecutando el script en la carpeta Fine\_tuning y Métricas explicadas anteriormente.
