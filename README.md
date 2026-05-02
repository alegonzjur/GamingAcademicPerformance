# 🎮 Gaming vs Academic Performance

**Autor:** Alejandro Román González · [@alegonzjur](https://github.com/alegonzjur)

**Repositorio:** [GamingAcademicPerformance](https://github.com/alegonzjur/GamingAcademicPerformance)

**Dataset:** [Kaggle — Gaming vs Academic Performance](https://www.kaggle.com/datasets/aiexplorer77/gaming-vs-academic-performance) 


![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas&logoColor=white) ![Power BI|128](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black) ![Status](https://img.shields.io/badge/Estado-En%20desarrollo-orange)

## 📌 Descripción 

Proyecto end-to-end de análisis y ciencia de datos que estudia la relación entre los hábitos de entretenimiento gaming y el rendimiento académico de aproximadamente 8000 estudiantes universitarios.

El pipeline abarca desde la limpieza de datos hasta el modelado predictivo con Machine Learning, con los resultados finales visualizados en un dashboard interactivo de PowerBI. 

**Preguntas que responde este proyecto:**
- ¿Las horas de gaming tienen importancia en el rendimiento académico?
- ¿Existe un umbral de horas de juego a partir del cual el impacto es significativo?
- ¿Qué variables protegen el rendimiento pese a un gaming intensivo?
- ¿Es posible identificar perfiles de estudiante en riesgo académico?

## 🔄 Pipeline

01_limpieza_datos.ipynb
		↓
02_eda.ipynb
		↓
03_modelo_ml.ipynb
		↓
Dashboard Power BI

| Fase | Notebook                  | Descripción                                              | Estado         |
| ---- | ------------------------- | -------------------------------------------------------- | -------------- |
| 1    | `01_limpieza_datos.ipynb` | Auditoría, corrección de anomalías y variables derivadas | ✅ Completado   |
| 2    | `02_eda.ipynb`            | Análisis exploratorio y visualizaciones                  | ✅ Completado   |
| 3    | `03_modelo_ml.ipynb`      | Clasificación, regresión y clustering                    | 🔄 En progreso |
| 4    | Power BI                  | Dashboard ejecutivo interactivo                          | ⏳ Pendiente    |

## 🛠️ Tecnologías

| Herramienta                | Uso en el proyecto                               |
| -------------------------- | ------------------------------------------------ |
| Python 3.11                | Lenguaje principal                               |
| Pandas / NumPy             | Limpieza y manipulación de datos                 |
| Matplotlib / Seaborn       | Visualización y análisis exploratorio            |
| Scikit-learn               | Modelos de clasificación, regresión y clustering |
| XGBoost                    | Gradient Boosting                                |
| VS Code / Jupyter Notebook | Entorno de desarrollo                            |
| Power BI                   | Dashboard ejecutivo interactivo                  |
## ## 📁 Estructura del repositorio

```
GamingAcademicPerformance/
│
├── data/
│   ├── Gaming_Academic_Performance.csv          # Dataset original
│   └── GAP_clean.csv                            # Dataset tras limpieza
│
├── img/                                  # Guarda los gráficos creados.
│   ├── fig_anomalias_previas.png
│   ├── fig_distribuciones_numericas.png
│   ├── fig_correlacion.png
│   ├── fig_gaming_vs_grades.png
│   ├── fig_perfil_riesgo.png
│   ├── fig_multivariado_gaming_estudio.png
│   └── fig_pairplot.png
│
├── 01_data_cleaning.ipynb
├── 02_eda.ipynb
├── 03_ml_modeling.ipynb        # Próximamente
└── README.md
```

## 🔍 Hallazgos principales

Estas son las conclusiones extraídas del análisis exploratorio sobre 8000 estudiantes universitarios.

### Gaming y rendimiento:

- Las horas de gaming muestran una relación negativa con las calificaciones, por supuesto más intensa cuanto mayores son las horas de gaming.

- El 'addiction_score' refuerza el patrón; los estudiantes con mayor puntuación de adicción tienden a obtener peores notas.

- El género del juego no tiene demasiado impacto en las notas o la puntuación de adicción.

### Factores protectores del rendimiento:

- Más horas de sueño se asocian consistentemente a mejores calificaciones.

- Mayor asistencia a clase muestra mejores notas, pero una diferencia poco significante.

- Las horas de estudio son el predictor positivo más claro de las calificaciones.

### Hallazgos contraintuitivos:

- Los estudiantes con mayor nivel de estrés obtienen mejores notas en promedio. La interpretación dada es que el estrés académico puede ser indicador de mayor implicación y exigencia personal sobre los estudios.

- Los estudiantes en riesgo reaccionan más rápido que aquellos con mejores notas. Esto quiere decir que el gaming intensivo desarrolla mayor agilidad cognitiva. Por otro lado, implica mayor dejadez en los estudios.

### Perfil del estudiante en riesgo:

- Más horas de gaming y mayor 'addiction_score'.

- Menos horas de estudio y menor asistencia a clase.

- Mayor velocidad de reacción.


## 📊 Visualizaciones destacadas

### Matriz de correlación

![Correlacion](./img/fig_matriz_correlacion.png)

### Perfil comparativo: En riesgo vs Sin riesgo

![Perfil de riesgo](./img/fig_perfil_riesgo.png)

### Gaming, estudio y riesgo académico

![Multivariado](./img/fig_multivariado_gaming_estudio.png)

