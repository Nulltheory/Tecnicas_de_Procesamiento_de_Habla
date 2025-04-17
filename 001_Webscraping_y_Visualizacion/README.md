# Web Scraping y Visualización de Texto

Este proyecto realiza un análisis de texto utilizando técnicas de **web scraping**, limpieza de datos y visualización mediante una nube de palabras. El texto fuente es un libro del **Proyecto Gutenberg**.

## 🧠 Descripción

Se extrae el texto de la obra _"Martín Fierro"_ desde el sitio de Project Gutenberg. Luego, se realiza lo siguiente:

- **Web Scraping**: Se descarga y parsea el contenido HTML.
- **Preprocesamiento de Texto**: 
  - Conversión a minúsculas
  - Eliminación de signos de puntuación
  - Filtro de stopwords en español + palabras irrelevantes adicionales
- **Visualización**: Se genera una nube de palabras para representar las palabras más frecuentes visualmente.

## 🛠️ Tecnologías Usadas

- `BeautifulSoup` – para parsing HTML
- `requests` – para descargar el contenido web
- `nltk` – para manejo de stopwords
- `WordCloud` – para generar la nube de palabras
- `matplotlib` – para visualizar resultados

## 📌 Requisitos

```bash
pip install beautifulsoup4 requests wordcloud nltk pillow matplotlib
```

Además, es necesario descargar los recursos de `nltk`:

```python
import nltk
nltk.download('stopwords')
```

## ▶️ Cómo Ejecutar

1. Asegúrate de tener Python instalado.
2. Abre el archivo `001_Webscraping y Visualizacion.ipynb` en Jupyter Notebook.
3. Ejecuta todas las celdas.
4. Se mostrará una nube de palabras generada a partir del texto procesado.

## ✍️ Autor

- **Alejandro Schiariti**
