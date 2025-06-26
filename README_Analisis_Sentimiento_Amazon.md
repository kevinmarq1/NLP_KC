# 📘 Análisis de Sentimiento en Reseñas de Amazon

Este proyecto es parte de la práctica final del módulo de NLP del bootcamp de Big Data y Machine Learning de KeepCoding. Su objetivo es construir un modelo capaz de analizar reseñas de productos en Amazon y clasificar si el sentimiento es **positivo** o **negativo**, aplicando técnicas de procesamiento de lenguaje natural y aprendizaje automático.

---

## 🚀 ¿Qué hace este proyecto?

- Carga y limpia texto de reseñas reales de Amazon.
- Preprocesa eliminando ruido textual, stopwords, números, etc.
- Vectoriza el texto con TF-IDF.
- Entrena y compara 4 modelos de clasificación:
  - Regresión Logística
  - Naive Bayes
  - Support Vector Machine (SVM)
  - Random Forest
- Evalúa con métricas como accuracy, precisión, recall y matrices de confusión.
- Permite probar manualmente una reseña nueva.

---

## 🧩 Dataset

Utiliza un dataset de reseñas de productos en Amazon, accesible desde este enlace de Google Drive:

🔗 https://drive.google.com/drive/folders/1MJUVu6oP0vfOrW-4gUgH6lAtQZxnTYRB?usp=drive_link

Solo debes montarlo en Google Colab con:

```python
from google.colab import drive
drive.mount('/content/drive')
ruta = '/content/drive/MyDrive/NLP/reviews_Books_5.json.gz'
```

El notebook se encargará de realizar un muestreo balanceado (3000 positivas y 3000 negativas).


## ▶️ Cómo usar el notebook

1. Abre el notebook en Google Colab.
2. Ejecuta paso a paso:
   - Montaje de Drive
   - Preprocesamiento
   - Vectorización
   - Entrenamiento de modelos
   - Evaluación y comparación
3. Puedes probar una nueva reseña editando esta línea:

```python
nueva_reseña = "This product is amazing, I loved it!"
```

---

## 📊 Resultados

El modelo con mejor desempeño fue **Naive Bayes**, alcanzando más de **93% de accuracy**. Todos los modelos entrenados obtuvieron resultados sólidos, validados con matrices de confusión y análisis de palabras más influyentes.

---

## 🛠️ Tecnologías usadas

- Python 3
- NLTK
- Scikit-learn
- Pandas, NumPy
- Matplotlib, Seaborn
- Google Colab

---

## 👤 Autor

Kevin Márquez  
📧 kevinmarq1504@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/kevin-marquez-360227169/)
