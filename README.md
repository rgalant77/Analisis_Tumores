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
