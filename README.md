





**Fase 1: Preguntar**

1. ¿Qué porcentaje de contenido es películas vs series?
2. ¿Cómo ha cambiado el rating (clasificación por edad) con el tiempo?
3. ¿Cuánto dura en promedio una película/serie? ¿Hay diferencias por género?
4. ¿Cuánto dura en promedio una película/serie? ¿Hay diferencias por género?


**Fase 2: Preparar** (10-20 min)*

Ve a Kaggle → busca “netflix shows shivamb” → descarga el CSV (netflix_titles.csv).

* Súbelo a Google Colab, Jupyter o Excel para empezar.


**Fase 3: Procesar** (30-60 min)
Limpieza típica (muy sencilla aquí):* Manejar valores nulos (director, cast, country → rellenar con “Sin dato” o eliminar filas si son pocas).

* Convertir date_added a formato fecha.
* Separar la columna “listed_in” (géneros) que tiene varios separados por coma → puedes crear una lista o explotarla.
* Crear columna “tipo” (Movie o TV Show) ya viene.
* Limpiar duration (separar número y unidad: “142 min” → 142 minutos).

**Fase 4: Analizar** (1-2 horas)
Usa pandas o lo que sepas:

* value_counts() para tipo (pelis vs series), rating, country.
* groupby por release_year o date_added.year → contar títulos por año.
* value_counts() en géneros (después de split y explode).
* Promedios: duración promedio por tipo.
* Tablas cruzadas: géneros más populares por país o por rating.


**Fase 5: Compartir** (1 hora)
Crea visualizaciones bonitas:

* Gráfico de pastel o barras: % películas vs series.
* Línea: evolución de títulos agregados por año.
* Barra horizontal: top 10 países productores.
* Treemap o wordcloud de géneros.
  Herramientas: Matplotlib/Seaborn (Python), o Tableau Public / Power BI (gratis), o incluso Google Data Studio / Looker Studio.
  Haz un dashboard simple con 4-5 gráficos + conclusiones.


**Fase 6: Actuar** (30 min)
Recomendaciones de negocio (ejemplos):

* “Netflix debería invertir más en contenido de [país X] porque es el que más gusta”.
* “Los géneros de [acción/comedia] dominan → priorizarlos en nuevas producciones”.
* “Desde 2018-2019 se agregaron muchos títulos → posible saturación, enfocar en calidad”.
