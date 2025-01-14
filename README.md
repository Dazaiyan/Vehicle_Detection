# Vehicle Detection

Este proyecto utiliza modelos de deep learning para detectar y clasificar vehículos en videos. Los vehículos detectados incluyen autos, camionetas, camiones, motos, buses, entre otros.

# Descargar Proyecto

[Proyecto](https://drive.google.com/file/d/1TtR5P2KY3zo9Z33sl-ku-Hlg9ZPJhv26/view?usp=drive_link)

## Tabla de Contenidos

1. [Requisitos](#requisitos)
2. [Estructura del Proyecto](#estructura-del-proyecto)
3. [Cómo Usar el Proyecto](#cómo-usar-el-proyecto)
4. [Dataset](#dataset)
5. [Resultados](#resultados)
6. [Autores](#autores)

---

## Requisitos

Antes de ejecutar este proyecto, asegúrate de cumplir con los siguientes requisitos:

- Python 3.8 o superior.
- Dependencias incluidas en el archivo `requirements.txt`. Puedes instalarlas ejecutando:

  ```bash
  pip install -r requirements.txt
  ```

- Sistema operativo: Windows, macOS o Linux.

---

## Estructura del Proyecto

```plaintext
project/
│
├── data/               # Carpeta para el dataset (VOC, imágenes, anotaciones)
├── models/             # Carpeta para los modelos entrenados
│   ├── modelo_entrenado_final.pth  # Modelo entrenado final
├── outputs/            # Carpeta para los videos de salida
├── scripts/            # Carpeta para los scripts
│   ├── predict.py      # Script para la detección en video
│   ├── train.py        # Script para entrenar el modelo
│   ├── model_utils.py  # Funciones para cargar y procesar el modelo
│   └── data_utils.py   # Funciones para manejar los datasets y preparar los datos
├── video/              # Carpeta para los videos de entrada
├── .gitignore          # Archivos ignorados por Git
└── requirements.txt    # Archivo para las dependencias
```

---

## Cómo Usar el Proyecto

1. **Clonar el repositorio:**

   ```bash
   git clone https://github.com/Dazaiyan/Vehicle_Detection.git
   cd Vehicle_Detection
   ```

2. **Crear y activar un entorno virtual:**

   ```bash
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate     # Windows
   ```

3. **Instalar las dependencias:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Asegúrate de tener el dataset en la carpeta `dataset/`.**
   - Descarga el dataset desde [este enlace](http://host.robots.ox.ac.uk/pascal/VOC/voc2007/VOCtrainval_06-Nov-2007.tar) y colócalo en la carpeta `dataset/`.

5. **Ejecutar el pipeline completo:**
6. 
   Entrenar al modelo con el dataset

    ```bash
   python scripts/train.py
   ```

   Ejecuta el script principal para procesar el video y generar las métricas de desempeño:

   ```bash
   python scripts/predict.py
   ```

7. **Ver los resultados:**
   - El video procesado se guardará en la carpeta `outputs/`.
   - Los gráficos de métricas se mostrarán en una ventana emergente.

---

## Dataset

El dataset utilizado para entrenar el modelo no está incluido en el repositorio debido a restricciones de tamaño. Puedes descargarlo desde [este enlace](http://host.robots.ox.ac.uk/pascal/VOC/voc2007/VOCtrainval_06-Nov-2007.tar) y colocarlo en la carpeta `dataset/`.

---

## Resultados

Al procesar el video, el modelo genera:

1. Un video con las detecciones realizadas, almacenado en `outputs/output_video.avi`.
2. Métricas de desempeño como precisión, recall, F1-score y una matriz de confusión.

**Ejemplo de gráficos generados:**

![Gráficos de Métricas](https://via.placeholder.com/800x400?text=Ejemplo+de+gráficos+de+precisión%2C+recall%2C+F1-score+y+matriz+de+confusión)

---

## Autores

- **Juan Sebastián Daza Menéndez**  
  - [GitHub](https://github.com/Dazaiyan)

---

¡Gracias por revisar este proyecto! Si tienes preguntas o sugerencias, no dudes en abrir un issue.



dame esto en
