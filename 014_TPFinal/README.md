
# 🛍️ Clasificador de Quejas en E-commerce con Gemini y Gradio

Este proyecto implementa un sistema prototipo que **clasifica mensajes de clientes** como quejas o no, utilizando el modelo de lenguaje **Gemini-Pro de Google**.

Diseñado como una solución ligera y demostrativa, el sistema puede integrarse fácilmente en entornos de atención al cliente para priorizar reclamos.

---

## 🧠 Descripción

A partir de una pequeña colección de mensajes pre-clasificados, se consulta a **Gemini** con prompts cuidadosamente diseñados para determinar si el contenido representa una queja.

El sistema se compone de:

- Un conjunto de datos base de ejemplo
- Prompts adaptados a Gemini para evaluar mensajes
- Predicción y evaluación de los resultados del modelo
- Una app interactiva en **Gradio** para pruebas en tiempo real

---

## ⚙️ ¿Cómo funciona?

1. Se definen mensajes simulados con etiquetas manuales: "queja" / "no queja"
2. Se construye un prompt tipo:
   ```
   ¿Este mensaje representa una queja de cliente?
   Mensaje: "<texto>"
   ```
3. Se envía el prompt al modelo `gemini-pro` usando la API de Google Generative AI
4. El modelo responde y la predicción se compara contra la etiqueta real
5. Se lanza una app web con **Gradio** donde el usuario puede probar el sistema libremente

---

## 🛠️ Tecnologías Usadas

- `google.generativeai` – Acceso al modelo Gemini-Pro
- `Gradio` – Interfaz web para probar el clasificador
- `Python` / `Jupyter Notebook` – Lógica del prototipo

---

## 📦 Instalación

1. Clona este repositorio o descarga el notebook:
   ```bash
   git clone https://github.com/Nulltheory/Tecnicas_de_Procesamiento_de_Habla.git
   cd Tecnicas_de_Procesamiento_de_Habla/014_TPFinal
   ```

2. Instala los paquetes necesarios:
   ```bash
   pip install google-generativeai gradio
   ```

3. Crea una clave de API para Gemini:
   - Visita [Google AI Studio](https://makersuite.google.com/)
   - Copia tu API key

4. Configura tu API key en el entorno (recomendado):
   ```bash
   export GOOGLE_API_KEY="TU_API_KEY"
   ```

   O reemplaza directamente en el código:
   ```python
   genai.configure(api_key="TU_API_KEY")
   ```

---

## ▶️ Cómo usar

1. Abre el archivo `014_TPFinal.ipynb` en Jupyter Notebook
2. Ejecuta todas las celdas en orden
3. Al final, se lanzará una interfaz web de Gradio
4. Ingresa cualquier mensaje de cliente y obtén la predicción de Gemini

---

## 💬 Ejemplo

```text
Mensaje: "Hace 3 días que espero el envío y no recibí nada"
Respuesta del modelo: "Sí, es una queja"
```

---

## 🎯 Limitaciones y Futuro

- El dataset es pequeño y simulado, lo que limita su evaluación formal
- El prompt podría refinarse para mayor precisión o multiclase
- Puede ampliarse para múltiples idiomas o emociones

---

## 📚 Créditos

Trabajo realizado para la asignatura **Técnicas de Procesamiento del Habla**  
Autores:
* [Mujica, Mauricio](https://github.com/mauriciomujica/)
*	[Poblete, Alfredo](https://github.com/AlfredoPoblete/)
*	[Schiariti, Alejandro](https://github.com/Nulltheory)

