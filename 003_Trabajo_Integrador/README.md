# 🧠 Trabajo Integrador - Procesamiento de Noticias con Web Scraping y NLP

Este proyecto realiza un procesamiento completo de artículos extraídos de un sitio de noticias, utilizando técnicas de **web scraping**, **preprocesamiento de texto** y **análisis de lenguaje natural (NLP)**. Se busca recolectar enlaces a noticias, limpiar el texto, y aplicar distintas métricas como **TF**, **TF-IDF**, y visualizaciones como **nube de palabras**.

---

## 📌 Descripción del Proyecto

1. **Obtención de Datos**
   - Se utiliza `requests` + `BeautifulSoup` para realizar scraping de un sitio web con paginación.
   - Se extraen enlaces a noticias recorriendo múltiples páginas.
   - Se aplica un `sleep` para evitar sobrecargar el servidor.

2. **Extracción de Texto**
   - Se recorre cada enlace para obtener el cuerpo del artículo.
   - Se almacenan el título, fecha, y contenido de cada noticia.

3. **Limpieza y Normalización**
   - Se eliminan acentos, signos de puntuación, y palabras vacías (stopwords).
   - Se unifica el texto a minúsculas y se normalizan caracteres.

4. **Análisis de Frecuencia**
   - Se aplican modelos `CountVectorizer` y `TfidfVectorizer` de scikit-learn.
   - Se calcula la frecuencia de términos y los valores TF-IDF.

5. **Visualización**
   - Se generan nubes de palabras para visualizar los términos más frecuentes.
   - Se grafican los principales términos según su peso.

---

## 🛠️ Tecnologías Utilizadas

- `requests`, `BeautifulSoup` (web scraping)
- `pandas`, `datetime`, `time`, `warnings`
- `nltk`, `re`, `unicodedata` (limpieza y preprocesamiento)
- `scikit-learn` (TF / TF-IDF)
- `matplotlib`, `WordCloud` (visualización)

---

## 📦 Instalación de Dependencias

```bash
pip install requests beautifulsoup4 pandas nltk scikit-learn wordcloud matplotlib
```

Y también asegurarse de descargar las stopwords en español de NLTK:

```python
import nltk
nltk.download('stopwords')
```

---

## ▶️ Cómo Ejecutar

1. Asegurate de tener Python y Jupyter Notebook instalados.
2. Abrí el archivo `003_Trabajo_Integrador.ipynb`.
3. Ejecutá las celdas una por una.
4. Verás progresivamente:
   - Progreso del scraping.
   - Limpieza del texto.
   - Análisis TF y TF-IDF.
   - Visualizaciones como nubes de palabras y gráficos.
