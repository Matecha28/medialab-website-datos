# medialab-website-datos
Proyecto: Titulares del Blog de Python
Idea: Este proyecto muestra cómo un estudiante de comunicaciones puede extraer información de una página web, ordenarla en un archivo de datos y publicarla en una página web académica usando herramientas básicas de Python y GitHub.

Pregunta
¿Qué temas aparecen con mayor frecuencia en los titulares del Blog oficial de Python?

Fuente
Sitio web: https://blog.python.org/
Fecha de extracción: 19 de enero de 2026

Metodología
Scraping:
Se descargó el contenido HTML de la página principal del Blog de Python usando Python y la librería requests.
Extracción:
Se identificaron los títulos de las publicaciones y sus enlaces mediante BeautifulSoup.
Limpieza:
Se eliminaron caracteres especiales y palabras vacías (stopwords) para facilitar el análisis.
Procesamiento:
Se calculó la longitud de cada titular y se identificaron las palabras más frecuentes.
Outputs:
Los resultados se guardaron en archivos CSV y se mostraron en una página web pública.


Reproducibilidad
Para repetir este proyecto en otra computadora:
Instalar Python
Instalar librerías:
python -m pip install requests beautifulsoup4 pandas
Ejecutar los scripts:
python src/scrape_python_blog.py
python src/process_posts.py
Publicar la carpeta docs/ con GitHub Pages.

Outputs
posts_python_blog.csv
Contiene los títulos y enlaces extraídos del blog.
posts_python_blog_procesado.csv
Incluye la longitud de cada titular.
top_palabras_titulos.csv
Muestra las palabras más frecuentes en los titulares.
Website académico:
Página web publicada con GitHub Pages que muestra los resultados de forma visual.
