# 🤖 Sistema de Detección de Quejas en E-commerce

Este proyecto implementa un sistema de clasificación automática de mensajes de clientes para detectar si contienen una **queja** o no. Está diseñado especialmente para ser usado en plataformas de atención al cliente dentro del entorno de e-commerce.

Incluye un prototipo funcional con una interfaz construida en **Gradio** para probar el modelo de forma interactiva.

---

## 🧠 Descripción

Se utiliza un conjunto de datos simulado de mensajes de clientes. El flujo general del proyecto incluye:

- **Carga y preparación de datos**: Dataset simulado con etiquetas (queja / no queja).
- **Preprocesamiento de texto**:
  - Conversión a minúsculas
  - Eliminación de signos de puntuación
  - Eliminación de stopwords en español
- **Entrenamiento de modelo de clasificación**:
  - TF-IDF + Regresión logística
- **Interfaz gráfica**:
  - Se implementa una app en Gradio para ingresar mensajes y recibir una predicción inmediata.

---

## 🛠️ Tecnologías Usadas

- `pandas` – para manipulación del dataset
- `scikit-learn` – para vectorización y modelado (TF-IDF + Logistic Regression)
- `nltk` – para procesamiento de texto y stopwords
- `Gradio` – para construir la interfaz web interactiva

---

## 📌 Requisitos

Instala las dependencias necesarias con:

```bash
pip install pandas scikit-learn nltk gradio
```

Además, asegúrate de descargar los recursos de NLTK:

```python
import nltk
nltk.download('stopwords')
```

---

## ▶️ Cómo Ejecutar

1. Asegúrate de tener **Python 3.8+** y **Jupyter Notebook** instalado.
2. Abre el archivo `014_TPFinal.ipynb` en Jupyter.
3. Ejecuta todas las celdas en orden.
4. Al final del notebook, se abrirá una aplicación web con Gradio donde puedes probar el sistema ingresando tus propios mensajes.

---

## 📷 Vista Previa

_Aquí puedes agregar una captura de pantalla de la app Gradio funcionando._

---

## 📝 Licencia

Este proyecto está disponible bajo la licencia MIT.

---

## 👤 Autor

**[Tu Nombre]** – [Tu perfil de GitHub u otro enlace si lo deseas]
