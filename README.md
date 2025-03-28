# Análisis de Datos con Spark: Explorando el Universo Musical de Spotify

## Descripción del Proyecto

Este proyecto utiliza Apache Spark para analizar tendencias musicales en Spotify a gran escala. Se realizan tareas de limpieza y preparación de datos, análisis exploratorio (EDA), modelado de popularidad de canciones y desarrollo de un sistema de recomendación musical basado en Big Data.

## Tecnologías Utilizadas

- **Apache Spark**
- **Python**
- **PySpark** 
- **Pandas y NumPy** 

## Datasets
- https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks

Este dataset contiene información sobre canciones y artistas, ideal para análisis musical y proyectos de recomendación. Está compuesto por dos archivos principales:

- **tracks.csv**: Contiene información detallada sobre más de 600,000 canciones.
- **artists.csv**: Información sobre los artistas que participaron en las canciones.

## Archivos del Dataset

### tracks.csv

Este archivo incluye más de 600,000 canciones con las siguientes características:

| Columna         | Descripción                                                    |
|-----------------|----------------------------------------------------------------|
| `track_id`      | Identificador único de la canción                              |
| `name`          | Nombre de la canción                                           |
| `popularity`    | Puntuación de popularidad de la canción (0-100)                 |
| `duration_ms`   | Duración de la canción en milisegundos                          |
| `explicit`      | Si la canción tiene contenido explícito (True/False)            |
| `artists`       | Artistas que participaron en la canción                         |
| `id_artists`    | IDs de los artistas                                            |
| `release_date`  | Fecha de lanzamiento de la canción                              |
| `danceability`  | Qué tan adecuada es la canción para bailar (0.0-1.0)            |
| `energy`        | Medida de intensidad y actividad de la canción (0.0-1.0)        |
| `key`           | Tonalidad de la canción (0-11)                                  |
| `loudness`      | Volumen general en decibelios (dB)                              |
| `mode`          | Modalidad de la canción (mayor o menor)                         |
| `speechiness`   | Presencia de palabras habladas en la canción (0.0-1.0)          |
| `acousticness`  | Medida de si la canción es acústica (0.0-1.0)                   |
| `instrumentalness` | Predice si la canción no contiene vocales (0.0-1.0)           |
| `liveness`      | Detecta presencia de audiencia en la canción (0.0-1.0)         |
| `valence`       | Positividad musical de la canción (0.0-1.0)                     |
| `tempo`         | Velocidad o ritmo estimado en BPM                              |
| `time_signature`| Compás estimado de la canción                                  |

### artists.csv

Este archivo contiene información sobre los artistas, incluyendo:

| Columna        | Descripción                                                   |
|----------------|---------------------------------------------------------------|
| `id`           | ID único del artista                                          |
| `followers`    | Número de seguidores del artista                              |
| `genres`       | Géneros asociados con el artista                               |
| `name`         | Nombre del artista                                            |
| `popularity`   | Puntuación de popularidad del artista (0-100)                  |

## Metodologia

- **Limpieza y Transformación de Datos**: Normalización, eliminación de valores nulos y conversión de tipos.
- **Análisis Exploratorio**: Identificación de patrones en popularidad, duración y características de audio.
- **Modelado de Popularidad**: Implementación de Random Forest para predecir éxito de canciones.
- **Sistema de Recomendación**: Uso de clustering y filtrado colaborativo para generar listas de reproducción personalizadas.

## Mejoras futuras
- Incorporación de embeddings neurales para mejorar recomendaciones.
- Optimización del sistema para consultas en tiempo real.
- Integración con plataformas de streaming para pruebas en producción.

