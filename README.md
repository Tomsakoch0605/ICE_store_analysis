Análisis de Ventas Globales de Videojuegos y Predicción para 2017

🎮 Descripción del Proyecto

Este proyecto tiene como objetivo analizar los datos históricos de ventas de videojuegos a nivel global para identificar patrones clave, tendencias y plataformas/géneros más rentables. El análisis se centra en la preparación de un conjunto de datos para construir un modelo de negocio para la planificación de ventas del año 2017.
El análisis incluye la limpieza de datos, el cálculo de ventas totales, la determinación del período actual de interés y la realización de pruebas de hipótesis estadísticas sobre las calificaciones de los juegos.
________________________________________
📁 Archivos del Proyecto

Archivo	Descripción
ICE_store-1.ipynb	El cuaderno Jupyter que contiene el código completo para la carga de datos, limpieza, preprocesamiento, análisis exploratorio y pruebas de hipótesis.
games.csv	El conjunto de datos original utilizado para el análisis, que contiene información sobre nombre, plataforma, año de lanzamiento, género, ventas por región, y calificaciones de críticos y usuarios.
________________________________________
🛠️ Requisitos e Instalación

Para ejecutar el cuaderno ICE_store-1.ipynb, necesitarás tener instalado Python y las siguientes librerías de análisis de datos:
•	pandas
•	numpy
•	matplotlib.pyplot
•	seaborn
•	scipy.stats (para las pruebas de hipótesis)

Instalación de dependencias
Puedes instalar las librerías necesarias usando pip:
pip install pandas numpy matplotlib seaborn scipy
________________________________________
📈 Análisis Realizado

El proyecto realiza las siguientes tareas de análisis y preprocesamiento:
1.	Limpieza de Datos:
o	Conversión de nombres de columnas a minúsculas.
o	Conversión del año de lanzamiento a formato entero (Int64).
o	Conversión de la columna user_score a formato numérico (float64), tratando el valor 'tbd' como valores perdidos (NaN).
o	Eliminación de filas sin información clave (name, genre, year_of_release).
2.	Cálculo de Ventas Totales: Se añade una columna total_sales que es la suma de las ventas en Norteamérica (na_sales), Europa (eu_sales), Japón (jp_sales) y otras regiones (other_sales).
3.	Análisis Exploratorio: Se analiza la cantidad de juegos lanzados por año y las ventas para determinar el período de datos más relevante y la esperanza de vida de las plataformas.
4.	Estudio de Perfil de Usuarios por Región: Análisis de ventas por género y plataforma en las regiones de Norteamérica, Europa y Japón.
5.	Pruebas de Hipótesis:
o	Prueba 1: Las calificaciones promedio de usuarios para las plataformas Xbox One y PC son las mismas.
o	Prueba 2: Las calificaciones promedio de usuarios para los géneros Acción y Deportes son las mismas.
________________________________________
✅ Conclusiones Principales (Pruebas de Hipótesis)

•	Plataformas XOne vs. PC (Calificación de Usuarios): No fue posible rechazar la hipótesis nula, lo que sugiere que las calificaciones promedio de los usuarios para Xbox One y PC son probablemente iguales.
•	Géneros Acción vs. Deportes (Calificación de Usuarios): Se rechazó la hipótesis nula, concluyendo que las calificaciones promedio de los usuarios para los juegos de Acción y Deportes son diferentes.
