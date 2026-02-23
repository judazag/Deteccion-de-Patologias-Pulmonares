# Dataset: Chest X-Ray & CT Images for Lung Pathology

El conjunto de datos utilizado en este proyecto proviene de fuentes de acceso abierto para investigación médica, principalmente el repositorio de **Mendeley Data**.

## Fuente Original
- **Dataset:** [COVID-19 Chest X-Ray & CT Scan Dataset](https://data.mendeley.com/datasets/dvntn9yhd2/1)
- **Cita:** *Vania, Natasya (2020), “COVID-19 Chest X-Ray & CT Scan Dataset”, Mendeley Data, V1, doi: 10.17632/dvntn9yhd2.1*

## Descripción del Dataset
El dataset original se estructura en categorías clínicas para tareas de clasificación multiclase:
* **COVID-19:** Imágenes positivas para SARS-CoV-2.
* **Pneumonia:** Casos de neumonía viral/bacteriana no relacionados con COVID-19.
* **Normal:** Pulmones sanos (grupo de control).

## Preparación en este Proyecto
Para asegurar la compatibilidad con el modelo **DINOv2** y las arquitecturas de Deep Learning implementadas:
1.  **Redimensionamiento:** Todas las imágenes fueron normalizadas a una resolución uniforme (ej. 224x224).
2.  **Conversión:** Estandarización a escala de grises/RGB según el requerimiento del extractor de características.
3.  **Split:** División de datos en 80% entrenamiento, 10% validación y 10% test.

## Instrucciones para replicar
Debido al tamaño de las imágenes, los archivos crudos no se alojan en este repositorio. Para ejecutar el notebook:
1.  Descargue el dataset desde el link de Mendeley arriba mencionado.
2.  Extraiga las carpetas en el directorio local `data/raw/`.
3.  Asegúrese de mantener la estructura de carpetas por clase para que el `ImageDataGenerator` o el script de carga de PyTorch/TensorFlow funcione correctamente.
