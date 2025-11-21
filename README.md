Este repositorio contiene un proyecto de **Machine Learning** para predecir diabetes a partir de datos clínicos.

## Descripción del proyecto

El objetivo de este proyecto es desarrollar y evaluar diferentes modelos de clasificación para predecir si un paciente tiene diabetes, utilizando variables como glicemia, presión sanguínea, índice de masa corporal (BMI), edad, entre otras.

El proyecto incluye:

- Análisis exploratorio de datos (EDA)  
- Preprocesamiento de datos  
- Entrenamiento de varios modelos de ML (regresión logística, KNN, árbol de decisión, Random Forest...)  
- Evaluación de modelos (precisión, recall, AUC, matriz de confusión)  
- Interpretabilidad de modelo (importancia de variables)  
- Notebook con todo el flujo de trabajo + script para entrenar el modelo

## Contenido del repositorio

Actualmente el repositorio incluye:

- **Diabetes.ipynb**
  Notebook principal donde se realiza:
  - Exploracion de datos (EDA)
  - Preprocesamiento
  - Entrenamiento de varios modelos de clasificacion
  - Evaluacion mediante metricas (accuracy, ROC-AUC, matriz de confusion, etc.)
 
-**SHAP_diabegtes.ipynb**
  Notebook donde se profundiza en la intepretabilidad del modelo usando SHAP:
  - Calculo de valores SHAP
  - Summary plots
  - Feature importance explicativa
  - Intepretacion del comportamiento del modelo

## Tecnologías usadas

- Python  
- Pandas  
- NumPy  
- Scikit-Learn  
- Jupyter Notebook  
- Matplotlib / Seaborn  

## Flujo de trabajo

1. Cargar los datos desde `data/diabetes_data.csv`  
2. Realizar análisis exploratorio (distribución de variables, correlaciones...)  
3. Preprocesar datos (missing values, escalado, codificación si es necesario)  
4. Entrenar varios modelos de ML  
5. Evaluar los modelos usando métricas como AUC, accuracy, F1-score  
6. Interpretar los modelos para entender qué variables son más importantes  
7. Guardar el modelo final en `models/`

## Cómo reproducir

1. Clona este repositorio  
   git clone https://github.com/MarinaVBsc/ML_Diabetes.git
   cd ML_Diabetes

2. Crea un entorno virtual (opcional, pero recomendado)
   python -m venv venv
   source venv/bin/activate #en Windows: venv\Scritps\activate

3. Instala las dependencias
   pip install -r requirements.txt

4. Ejecuta el notebook para ver el analisis y los modelos:
   jupyter notebook notebooks/diabetes_analysis.ipynb

## Métricas de evaluación

Algunos de los modelos se pueden evaluar con:

Exactitud (accuracy)

Precisión, recall, F1-score

Curva ROC / AUC

Matriz de confusión

# Interpretabilidad

Para interpretar los modelos, se puede usar:

Importancia de características (feature importance) para árboles y bosques aleatorios

Técnicas más avanzadas (SHAP, LIME) si se quieren ver contribuciones individuales

## Contribuciones

¡Bienvenidas! Si quieres contribuir:

1. Haz fork del repositorio

2. Crea una rama con tu función: git checkout -b mi-feature

3. Haz commit de tus cambios: git commit -m "Añadida nueva función"

4. Empuja a tu fork: git push origin mi-feature

5. Abre un pull request y describe tus cambios
