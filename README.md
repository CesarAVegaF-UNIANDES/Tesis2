En el presente repositorio encontrara los scripts utilizados en esta investigación, donde se presentan los experimentos realizados, teniendo en cuenta las siguientes componentes: 

  * Los sistemas FAS seleccionados: Silent FAS, Liveness Detection FAS y Object FAS.
  * los conjuntos de imágenes con ejemplos de ataques de presentación: CASIA y Sustitución (Generado en esta investigación).
  * Los conjuntos de imágenes con ejemplos de manipulación digital: StyleGAN (Generadas por NVIDIA) y Difusión (Generado en esta investigación).


En la carpeta Fine_Tuning se encuentra el script de google colab con el cual se hiso los Experimentos mencionados en esta investigación, en el cual encontrara las instrucciones para la ejecución y replicación del entrenamiento de los modelos. Para esto se requiere descargar los conjuntos de datos en el siguiente enlace

https://drive.google.com/drive/folders/1gycc4CS_B1LZeisjAYcC4dvhTNS1hZYV?usp=share_link


En la carpeta métricas encontrará el script usado para leer las métricas obtenidas sin Fine Tuning (Experimento 1) y también encontrará las métricas obtenidas para cada uno de los experimentos divididos por sistema FAS, donde Silent FAS es equivalente a lo planteado en el Experimento 2, Liveness Detection FAS es equivalente Experimento 3 y Object FAS equivalente al Experimento 4. Las métricas del Experimento 5 son equivalentes a la subsección ALL en cada uno de los sistemas FAS.


Adicional en la carpeta Train, encontrará los datos de entrenamiento usados en cada uno de los sistemas FAS, esta es requerida si desea replicar la experimentación de Fine Tuning.
