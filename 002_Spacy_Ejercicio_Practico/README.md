# Análisis NLP con spaCy y Web Scraping

Este proyecto realiza un ejercicio práctico de procesamiento de lenguaje natural (PLN) utilizando **spaCy**, junto con técnicas de **web scraping** y visualización. Se trabaja sobre una noticia de *Infobae* relacionada con tecnología médica.

## 🧠 Descripción

1. **Web Scraping**  
   Se obtiene el contenido de una noticia desde Infobae usando `BeautifulSoup`.

2. **Preprocesamiento del Texto**  
   - Eliminación de etiquetas HTML irrelevantes.
   - Conversión a minúsculas y limpieza de signos de puntuación.
   - Eliminación de *stopwords* y palabras irrelevantes.

3. **Procesamiento con spaCy**  
   - Tokenización del texto.
   - Extracción y visualización de entidades nombradas (NER).
   - Análisis de dependencias sintácticas.

4. **Visualización**  
   Se generan visualizaciones con `displacy` y se construye una nube de palabras (`WordCloud`) con las palabras más relevantes.

## 🛠️ Tecnologías Usadas

- `spaCy` + `es_core_news_lg`
- `BeautifulSoup`, `requests`
- `matplotlib`, `WordCloud`
- `nltk` para stopwords

## 📌 Requisitos

```bash
pip install spacy beautifulsoup4 requests nltk wordcloud matplotlib
python -m spacy download es_core_news_lg

También es necesario descargar los recursos de stopwords de NLTK:
import nltk
nltk.download('stopwords')

▶️ Cómo Ejecutar
1. Asegúrate de tener Python y Jupyter Notebook instalados.
2. Abre el archivo 002_Spacy_Ejercicio_Practico.ipynb.
3. Ejecuta todas las celdas paso a paso.
4. Se mostrarán visualizaciones del análisis de entidades y relaciones del texto, así como una nube de palabras.
