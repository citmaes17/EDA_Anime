# 📊 Análisis Exploratorio de Datos - Anime

Análisis exhaustivo del dataset de los Top 15,000 anime de MyAnimeList, explorando las relaciones entre score, tipos de anime y categorías de géneros.

## 📋 Descripción del Proyecto

Este proyecto presenta un análisis exploratorio de datos (EDA) completo sobre una base de datos de anime, con el objetivo de identificar patrones, tendencias y relaciones entre diferentes variables que influyen en la valoración de los anime. El análisis se enfoca especialmente en cómo el tipo de anime y las categorías de géneros afectan el score promedio.

## 🎯 Objetivos

- Realizar una limpieza y preparación exhaustiva del dataset
- Explorar la distribución de scores y características principales de los anime
- Identificar patrones en los tipos de anime y categorías de géneros
- Analizar las relaciones entre tipo, género y valoración
- Generar visualizaciones interactivas para facilitar la comprensión de los datos

## 🗂️ Estructura del Proyecto

```
EDA_Anime/
│
├── EDA.ipynb                    # Notebook principal con el análisis completo
├── EDA.pptx                     # Presentación de resultados
├── top_15000_anime.csv          # Dataset original
└── README.md                    # Este archivo
```

## 📊 Dataset

El dataset utilizado contiene información de los **15,000 anime mejor valorados** de MyAnimeList e incluye las siguientes características:

### Columnas Principales:
- **anime_id**: Identificador único del anime
- **name**: Nombre del anime
- **english_name**: Nombre en inglés
- **japanese_names**: Nombre en japonés
- **score**: Puntuación promedio (escala 0-10)
- **genres**: Géneros del anime
- **themes**: Temas principales
- **demographics**: Demografía objetivo
- **type**: Tipo de anime (TV, Movie, OVA, etc.)
- **episodes**: Número de episodios
- **status**: Estado de emisión
- **aired**: Fecha de emisión
- **producers**: Productoras
- **studios**: Estudios de animación
- **source**: Material fuente
- **duration**: Duración de episodios
- **rating**: Clasificación por edad
- **rank**: Ranking general
- **popularity**: Índice de popularidad
- **favorites**: Número de favoritos
- **scored_by**: Número de usuarios que puntuaron
- **members**: Número de miembros

## 🔍 Metodología de Análisis

### 1. **Carga y Exploración Inicial**
   - Importación del dataset
   - Visualización de estructura y dimensiones
   - Identificación de tipos de datos

### 2. **Limpieza y Preparación de Datos**
   - Análisis de valores nulos
   - Eliminación de columnas con >20% de valores nulos
   - Eliminación de filas duplicadas
   - Imputación de valores faltantes según tipo de dato
   - Verificación de integridad del dataset

### 3. **Procesamiento de Categorías de Géneros**
   - Creación de función de categorización de géneros
   - Agrupación de géneros en categorías principales
   - Análisis de distribución de categorías

### 4. **Análisis Univariable**
   - Estadísticas descriptivas del score
   - Distribución del score con curva normal
   - Análisis de tipos de anime
   - Distribución por categoría de géneros
   - Cantidad de categorías por anime

### 5. **Análisis Bivariable**
   - Score promedio por tipo de anime
   - Boxplot: Score vs Type
   - Score promedio vs categoría de género (gráfico de barras)
   - Boxplot: Score vs Category

### 6. **Análisis Multivariable**
   - Relación Type × Category vs Score
   - Heatmap: Type × Category × Score

## 🛠️ Tecnologías Utilizadas

```python
- Python 3.x
- pandas          # Manipulación de datos
- numpy           # Operaciones numéricas
- plotly          # Visualizaciones interactivas
- scipy           # Análisis estadístico
- collections     # Conteo de frecuencias
```

## 📈 Principales Hallazgos

> **Nota**: Los hallazgos detallados se encuentran en el notebook `EDA.ipynb` y en la presentación `EDA.pptx`

El análisis revela patrones interesantes sobre:
- La distribución de scores y su tendencia central
- Las diferencias en valoración según el tipo de anime
- La influencia de las categorías de géneros en el score
- Las combinaciones de tipo y género más populares y mejor valoradas

## 🚀 Cómo Usar Este Proyecto

### Requisitos Previos

```bash
pip install pandas numpy plotly scipy jupyter
```

### Ejecución

1. **Clonar el repositorio**
```bash
git clone https://github.com/citmaes17/EDA_Anime.git
cd EDA_Anime
```

2. **Abrir el notebook**
```bash
jupyter notebook EDA.ipynb
```

3. **Ejecutar las celdas secuencialmente**
   - Todas las celdas están diseñadas para ejecutarse en orden
   - Las visualizaciones son interactivas gracias a Plotly

## 📊 Visualizaciones

El proyecto incluye múltiples visualizaciones interactivas:
- Histogramas con curvas de distribución normal
- Gráficos de barras comparativos
- Boxplots para análisis de dispersión
- Heatmaps para relaciones multivariables
- Todos los gráficos son interactivos y explorables

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar este análisis:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 👤 Autor

**citmaes17**
- GitHub: [@citmaes17](https://github.com/citmaes17)

## 📧 Contacto

Si tienes preguntas o sugerencias sobre este proyecto, no dudes en abrir un issue en el repositorio.

---

⭐ Si este proyecto te fue útil, considera darle una estrella en GitHub!

## 🙏 Agradecimientos

- Datos obtenidos de [MyAnimeList](https://myanimelist.net/)
- Comunidad de data science y anime por la inspiración

---

**Última actualización**: Octubre 2025
