# 🧠 Motivational Quote Generator (NLP Final Project)

Este proyecto implementa un sistema completo de procesamiento de lenguaje natural (NLP) capaz de generar frases motivacionales originales y clasificarlas según su tema utilizando modelos de última generación.

Desarrollado como **proyecto final del curso de NLP – PUCMM**.

---

## ✨ Características principales

- 🧹 **Limpieza de frases**: Filtrado de citas irrelevantes o con ruido (fechas, URLs, medios, etc.).
- 🧠 **Clasificación semántica**: Uso de DeBERTa para detectar si una frase tiene "sentido" (`meaningful`) y su categoría temática.
- 📝 **Generación creativa**: Generación de frases motivacionales originales por tema usando `Mixtral 8x7B Instruct`.
- ✅ **Validación automática**: Solo se conservan frases coherentes con alto puntaje temático y semántico.
- 📊 **Análisis final**: Distribución temática, frases destacadas y visualización de resultados.

---

## 📂 Estructura del repositorio

motivational-quote-generator-nlp/
│
├── Proyecto_Final_NLP.ipynb # Notebook principal con todo el flujo
├── quotes-wisdom.csv # Dataset base de frases
├── frases_validadas_con_tema.csv # Frases limpias clasificadas
├── nuevas_frases_por_tema.csv # Frases generadas por el modelo
├── frases_generadas_validadas.csv # Frases finales validadas
├── frases_generadas_descartadas.csv # Frases rechazadas con motivo
├── README.md # Descripción del proyecto


---

## 🛠 Tecnologías utilizadas

- Python + Google Colab
- HuggingFace Transformers
  - `Mixtral 8x7B Instruct` para generación
  - `MoritzLaurer/deberta-v3-large-zeroshot-v2.0` para clasificación
- pandas, scikit-learn, matplotlib, tqdm
- GPU (CUDA) para acelerar procesamiento

---

## 🚀 Cómo ejecutarlo

1. Abre `Proyecto_Final_NLP.ipynb` en [Google Colab](https://colab.research.google.com/)
2. Instala las dependencias:
   ```python
   !pip install -U bitsandbytes transformers accelerate
[Wilkin Vargas]
Estudiante de Ingeniería en Ciencias de la Computación
Pontificia Universidad Católica Madre y Maestra (PUCMM)
Proyecto final – Natural Language Processing (NLP)
