# DashboardExcel
# Análisis Exploratorio de Datos de Accidentes de Tráfico en EE.UU.

## Objetivo del Proyecto

Realizar un análisis exploratorio de un conjunto de datos relacionados con accidentes de tráfico, utilizando Excel como herramienta principal. El proyecto tiene como fin limpiar, transformar y analizar los datos para mostrar resultados relevantes a través de un dashboard visual y un informe explicativo.

---

## Dataset Utilizado

- Fuente [Kaggle - US Accidents (3.0 million+ records)](httpswww.kaggle.comsobhanmoosavius-accidents)
- Tamaño original 49 columnas y más de 2.8 millones de registros.
- Muestra utilizada ~2,000 registros y 20+ columnas seleccionadas para agilizar el trabajo en Excel.
- Variables clave `Start_Time`, `Severity`, `Duration`, `City`, `Weather_Condition`, entre otras.

---

## 1. Transformación y Limpieza de Datos

### Acciones realizadas
- Se eliminaron columnas irrelevantes o con muchos valores nulos (`Bump`, `Give_Way`, `No_Exit`, etc.).
- Se crearon nuevas columnas derivadas
  - `Duration (minutes)` diferencia entre `Start_Time` y `End_Time`.
  - `Moment_day` clasificación en Madrugada, Mañana, Tarde, Noche según la hora.
  - `Month` y `Year` extraídos de `Start_Time`.
- Se corrigieron formatos de fecha-hora y se convirtieron a valores numéricos donde fue necesario.
- Se trataron valores faltantes en columnas como `Temperature(F)`, `Visibility(mi)` y `Precipitation(in)`.

---

## 2. Análisis Descriptivo

### Variables Analizadas
- Severidad de accidentes (`Severity`) escala de 1 a 4, siendo 4 la más grave.
- Duración media del accidente.
- Distribución horaria (`Moment_day`).
- Clima predominante (`Weather_Condition`).
- Condiciones de visibilidad y precipitación.
- Frecuencia por ciudad y estado.

### KPIs clave
-  Duración Promedio de los Accidentes `≈ 38 minutos`.
-  Accidentes registrados en 2024 `1.342 eventos`.

---

## 3. Dashboard (en Excel)

El dashboard desarrollado en Excel incluye
- Gráficos de barras y pastel para visualizar
  - Accidentes por hora del día (`Moment_day`).
  - Tipos de clima durante accidentes.
  - Accidentes por ciudad o estado.
- KPIs destacados en paneles visibles.
- Segmentadores y filtros por año, estado y severidad.

---

## 4. Conclusiones del Análisis

- La mayoría de los accidentes ocurrieron durante la mañana y la tarde, coincidiendo con horas pico.
- Las condiciones climáticas más frecuentes durante los accidentes fueron Clear, Overcast, y Rain.
- Estados como California y Texas mostraron mayor frecuencia de incidentes en la muestra.
- Existe una relación entre condiciones meteorológicas y duración del accidente.
- La duración media fue de 38 minutos, con algunas situaciones prolongadas más de 3 horas.

---

## Herramientas Utilizadas

- Microsoft Excel 365
  - Power Query (limpieza inicial)
  - Fórmulas (HORA, TEXTO, FECHA, AÑO, etc.)
  - Segmentadores
  - Tablas dinámicas
  - Gráficos dinámicos

---

## Consideraciones Finales

El análisis demuestra cómo Excel puede ser una herramienta efectiva para realizar análisis exploratorios incluso con datasets complejos, siempre que se trabaje con una muestra bien preparada. Se recomienda migrar a herramientas como Power BI o Python para analizar todo el conjunto completo en caso de escalar el proyecto.



Proyecto Dashboard Excel
