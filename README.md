# 📊 Análisis de Tasa de Supervivencia en Pacientes con Tumores Cerebrales 🧠

![Estudio Galant Logo](https://via.placeholder.com/150x50?text=Estudio+Galant) *(Logo representativo)*

## 📌 Resumen Ejecutivo  
Este proyecto analiza factores clínicos que influyen en la supervivencia de pacientes con tumores cerebrales, utilizando datos médicos para optimizar protocolos de tratamiento. Los hallazgos clave incluyen correlaciones entre tipo de tumor, tratamientos y tasas de supervivencia.

---

## 📚 Tabla de Contenidos  
- [Motivación](#-motivación)  
- [Audiencia](#-audiencia)  
- [Metadatos](#-metadatos)  
- [Preguntas e Hipótesis](#-preguntas-e-hipótesis)  
- [Visualizaciones](#-visualizaciones-clave)  
- [Insights](#-insights-preliminares)  
- [Recomendaciones](#-recomendaciones)  
- [Contacto](#-contacto)  

---

## 🎯 Motivación  
Los tumores cerebrales son una de las principales causas de mortalidad por cáncer. Este estudio busca:  
🔍 Identificar factores clave que impactan la supervivencia.  
💡 Mejorar protocolos de tratamiento basados en evidencia.  

---

## 👥 Audiencia  
Este análisis está dirigido a:  
- **Oncólogos** 🩺  
- **Investigadores médicos** 🔬  
- **Gestores de políticas de salud** 📋  

---

## 📊 Metadatos  
### Variables Analizadas  
| Tipo           | Variables Principales                                                                 |
|----------------|--------------------------------------------------------------------------------------|
| **Enteras**    | `Age`, `Genetic_Risk`, `Survival_Rate (%)`                                           |
| **Categóricas**| `Gender`, `Tumor_Type`, `Treatment_Received`, `Symptom_Severity`, `Tumor_Location`   |
| **Flotantes**  | `Tumor_Size`                                                                         |

*Descripción detallada de variables en [páginas 6-7 del PDF](#).*

---

## ❓ Preguntas e Hipótesis  
1. **¿El tamaño del tumor afecta la supervivencia?** 📏  
2. **¿El género influye en el tratamiento recibido?** ♀️♂️  
3. **¿La exposición a radiación aumenta el tamaño del tumor?** ☢️  
4. **¿La ubicación del tumor impacta su crecimiento?** 🧠📍  
5. **¿Diferencias en supervivencia entre países?** 🌍  

*10 preguntas totales ([ver páginas 8-9](#)).*

---

## 📈 Visualizaciones Clave  
### 1. Distribución de Supervivencia  
![Histograma](https://via.placeholder.com/400x200?text=Histograma+Supervivencia)  
*Tasa de supervivencia concentrada entre 40-80%.*

### 2. Supervivencia por Tratamiento  
![Boxplot](https://via.placeholder.com/400x200?text=Boxplot+Tratamientos)  
**Cirugía** 🏥 muestra mayor tasa vs. quimioterapia/radiación.

### 3. Relación Presión Arterial vs. Supervivencia  
![Scatterplot](https://via.placeholder.com/400x200?text=Scatterplot+Presión)  
Sin correlación clara (`r = 0.12`).

---

## 🔍 Insights Preliminares  
✅ **Tumores malignos** tienen supervivencia 30% menor que benignos.  
✅ **Cirugía** es el tratamiento más efectivo (+25% supervivencia).  
✅ **Lóbulo frontal** tiene pronóstico más favorable.  

---

## 🚀 Recomendaciones  
| Audiencia           | Acción Propuesta                                                                 |
|---------------------|---------------------------------------------------------------------------------|
| **Oncólogos**       | Priorizar cirugía en tumores malignos.                                          |
| **Investigadores**  | Estudiar tumores en lóbulo frontal para entender mejor pronóstico.              |
| **Gestores de salud**| Asignar recursos a tratamientos quirúrgicos y seguimiento postoperatorio.       |

---
## 📊 Análisis de Tasa de Supervivencia en Pacientes con Tumores Cerebrales 🧠 + 🤖 ML Predictivo
Estudio Galant Logo
(Análisis clínico y predictivo integrado)

### 🔍 Resumen Ampliado
Este proyecto combina análisis exploratorio y modelado predictivo para entender factores asociados a tumores cerebrales. Incluye:

- **📈 Análisis estadístico de supervivencia**

- **🤖 Modelos de ML para predecir presencia de tumor**

- **🎯 Recomendaciones clínicas basadas en datos**

### 🛠️ Actualización: Modelado Predictivo
### 🎯 Objetivo del ML
Desarrollar un modelo de clasificación binaria para predecir Brain_Tumor_Present (presencia/ausencia de tumor) usando variables clínicas disponibles.

## 📊 Metodología ML
### 🔄 Pipeline de Trabajo
graph TD
    A[Preprocesamiento] --> B[Balanceo de Datos]
    B --> C[Selección de Features]
    C --> D[Modelado]
    D --> E[Optimización]
    E --> F[Evaluación]

### 1. 🔧 Preprocesamiento
- **Codificación:**
🏷️ OneHotEncoding para categóricas nominales
🔢 LabelEncoding para ordinales

- **Limpieza:**
🧹 Imputación de valores faltantes
✂️ Normalización con StandardScaler

### 2. ⚖️ Balanceo de Datos
- **📉 Verificación de distribución de clases**

- **🔄 Técnicas aplicadas:**

-- **Submuestreo (undersampling)**

-- **Validación cruzada estratificada (StratifiedKFold)**

### 3. 🤖 Modelos Implementados

Modelo	                      Librería	                   Hiperparámetros Optimizados
Regresión Logística	          sklearn.linear_model	       Penalización, C
Random Forest Classifier	  sklearn.ensemble	           n_estimators, max_depth

### 4. 📏 Métricas de Evaluación

   metrics = {
    "accuracy": "Balanced Accuracy Score",
    "precision": "Precision Score",
    "recall": "Recall Score",
    "f1": "F1-Score",
    "conf_matrix": "Matriz de Confusión"
}

## 📌 Resultados Clave
### 🏆 Performance de Modelos

Modelo	               Accuracy (⌀)	          ±SD	            Precisión	          Recall
Regresión Logística	   0.5019	              ±0.0007	        0.48	              0.51
Random Forest	       0.5001	              ±0.0011	        0.49	              0.50

## 📉 Limitaciones Identificadas

- **🎯 Poder predictivo bajo: Accuracy ~50% (similar a azar)**

- **🔍 Posibles causas:**

-- **Variables insuficientemente informativas**

-- **Necesidad de biomarcadores adicionales**

-- **Ruido en codificación de datos**


## 🧠 Insights Integrados

### 🔗 Relación con Análisis Exploratorio

1- Variables clave no predictivas:

- **Aunque Tumor_Size y Location afectan supervivencia, no predicen bien presencia inicial de tumor.**

2- Recomendación dual:

- **Para diagnóstico temprano: 🆕 Buscar nuevos biomarcadores**

- **Para tratamiento: 🏥 Priorizar cirugía en casos confirmados (según EDA previo)**

## 🚀 Próximos Pasos

### 🔄 Mejoras al Modelo

- **[+] Incorporar técnicas avanzadas de balanceo (SMOTE)**

 - **[+] Ensamblar modelos con VotingClassifier**

 - **[+] Probar arquitecturas neuronales simples**

### 🧪 Requerimientos de Datos

- **🔬 Incluir marcadores genéticos específicos**

- **🧬 Datos de neuroimagen estructurados (MRI cuantitativos)**

## 📂 Estructura Actualizada del Repo

├── ml/
│   ├── preprocessing.py    # Scripts de limpieza
│   ├── modeling.py        # Entrenamiento de modelos
│   └── evaluation/        # Métricas y gráficos
├── data/
│   ├── raw/               # Datos originales
│   └── processed/        # Datos para ML
└── notebooks/
    ├── EDA.ipynb         # Análisis exploratorio
    └── ML_Pipeline.ipynb # Flujo predictivo

## 📞 Contacto  
✉️ **Email**: [galant@ficticio.ar](mailto:galant@ficticio.ar)  
🌐 **Web**: [www.rdgficticio.ar](http://www.rdgficticio.ar)  
📱 **Teléfono**: 911-0000-0000  
🏢 **Dirección**: Calle Cualquiera 123, Cualquier Lugar, CP: 12345  

---

## 🔗 Repositorio GitHub  
📂 **Estructura del Proyecto**:  
```
├── data/               # Datos crudos y procesados
├── notebooks/          # Jupyter Notebooks de análisis
├── visuals/            # Gráficos y dashboards
└── README.md           # Este archivo
```

🛠️ **Tecnologías Usadas**:  
- Python 🐍 (Pandas, Matplotlib, Seaborn)  
- Jupyter Notebook 📓  
- GitHub Actions 🤖 (para CI/CD)  

⭐ **¡Dale una estrella al repo si te resulta útil!**  

---

*© 2023 Estudio Galant. Todos los derechos reservados.*  

--- 

### 📌 Notas Adicionales  
- Los datos son anónimos y cumplen con regulaciones HIPAA.  
- Para contribuciones, abre un **Pull Request** siguiendo las [guías de contribución](CONTRIBUTING.md).  

![Footer](https://via.placeholder.com/800x50?text=Gracias+por+visitar+el+proyecto!+🧠💙)
