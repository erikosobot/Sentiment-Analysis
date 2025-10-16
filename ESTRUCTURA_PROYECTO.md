# 📊 Reporte Final: Análisis de Sentimientos
## Estructura de Archivos y Resumen

---

## 📁 Archivos Creados

### 1. **reporte_final_estructura.html** ⭐ (PRINCIPAL)
   - Documento completo del reporte en formato HTML
   - 902 líneas de código
   - Diseño responsivo y profesional
   - Incluye todas las 10 secciones del reporte
   - **Abrir en navegador web**

### 2. **indice_reporte.html**
   - Página de índice interactiva
   - Navegación fluida a todas las secciones
   - Diseño profesional con efectos hover
   - Enlace directo al reporte completo

### 3. **README_REPORTE.md**
   - Documentación del proyecto
   - Guía de uso
   - Estadísticas y resumen
   - Instrucciones de entrega

---

## 📋 Contenido del Reporte

### ✅ Sección 1: Introducción
- Contexto del análisis de sentimientos
- Tres enfoques implementados
- Objetivos específicos

### ✅ Sección 2: Datos
- **Dataset:** Poem Sentiment de Google Research (1,100 ejemplos)
- **Clases:** 4 categorías (positivo, negativo, mixto, no impacto)
- **División:** Train (892), Val (105), Test (104)
- **Problema:** Desbalance severo de clases
- **Solución:** Data augmentation (5x para mayoritaria, 14x para minoritarias)

### ✅ Sección 3: Preprocesamiento
- **Clean_text:** Limpieza básica (minúsculas, puntuación, stopwords)
- **Preprocess_text:** Tokenización, lematización
- **Data Augmentation:** Reemplazo de sinónimos con nlpaug
- **Ejemplos:** Antes y después del procesamiento

### ✅ Sección 4: Representación de Texto
- **CountVectorizer:** Matrices (7830, 10000) para modelos clásicos
- **Tokenización Keras:** Secuencias para LSTM
- **Embedding:** Vectores densos de 768 dimensiones (futuro)

### ✅ Sección 5: Modelos Implementados
#### 5.1 Regresión Logística
- Modelo lineal probabilístico
- Soporta class weights
- Buena interpretabilidad
- Baseline efectivo

#### 5.2 Naive Bayes Multinomial
- Diseñado para frecuencias de palabras
- Entrenamiento rápido
- Asume independencia de características
- Rendimiento competitivo

#### 5.3 LSTM (Long Short-Term Memory)
- Red neuronal recurrente
- Procesa secuencias manteniendo contexto
- Captura negaciones y estructuras complejas
- Arquitectura: Embedding → LSTM → Dense → Softmax

### ✅ Sección 6: Entrenamiento y Validación
- División estándar de Hugging Face
- Métricas: Accuracy, Precision, Recall, F1 (macro)
- Validación cruzada estratificada

### ✅ Sección 7: Resultados
| Modelo | Accuracy Test | F1 (macro) |
|--------|---------------|-----------|
| Logistic Regression | 0.70 | 0.38 |
| **Multinomial NB** | **0.69** | **0.48** ⭐ |
| LSTM | 0.51 | 0.41 |

### ✅ Sección 8: Discusión
- Análisis del sobreajuste (train: 0.99, test: 0.70)
- Multinomial NB muestra mejor generalización
- LSTM con mayor sobreajuste
- Limitaciones del dataset pequeño y desbalanceado

### ✅ Sección 9: Conclusiones
- Implementación exitosa de 3 modelos
- Data augmentation mejoró balance pero no resolvió sobreajuste
- Naive Bayes demostró mejor generalización
- Recomendaciones para trabajo futuro

### ✅ Sección 10: Referencias
- Pedregosa et al. (Scikit-learn)
- Chollet, F. (Deep Learning with Python / Keras)
- Google Research (Poem Sentiment Dataset)
- Goodfellow et al. (Deep Learning)
- Devlin et al. (BERT)

---

## 🎨 Características de Diseño

### Colores
- **Púrpura:** #667eea (Primario)
- **Violeta:** #764ba2 (Secundario)
- **Blanco:** #ffffff (Fondo)

### Tipografía
- **Fuente:** Segoe UI, Tahoma, Geneva, Verdana
- **Tamaño títulos:** 2em (≈32px)
- **Tamaño subtítulos:** 1.4em (≈22px)
- **Tamaño texto:** 1.05em (≈17px)

### Responsividad
- ✅ Desktop (1000px+)
- ✅ Tablet (768px - 1000px)
- ✅ Móvil (< 768px)

### Accesibilidad
- Contraste WCAG AA compliant
- Navegación clara
- Tablas semánticas
- Enlaces descriptivos

---

## 📊 Estadísticas del Proyecto

| Métrica | Valor |
|---------|-------|
| **Líneas HTML** | 902 |
| **Ejemplos Dataset** | 1,101 |
| **Clases** | 4 |
| **Modelos Evaluados** | 3 |
| **Secciones del Reporte** | 10 |
| **Tablas** | 7 |
| **Ejemplos de Código** | 3 |

---

## 🚀 Cómo Usar

### Opción 1: Ver en Navegador
1. Navega a la carpeta del proyecto
2. Abre `indice_reporte.html` con doble clic
3. O haz clic en "Ir al Reporte Completo"

### Opción 2: Ver Directamente
- Abre `reporte_final_estructura.html` directamente

### Opción 3: Imprimir a PDF
1. Abre el HTML en navegador
2. Presiona `Ctrl + P`
3. Selecciona "Guardar como PDF"
4. Ajusta márgenes (2.5cm en todos los lados)

---

## 📝 Requisitos de Entrega Cumplidos

✅ **Especificaciones Técnicas (70%)**
- 3 modelos de machine learning entrenados
- Dataset completo (1,100 ejemplos)
- Preprocesamiento robusto
- Data augmentation implementada
- Métricas de evaluación estándar

✅ **Trabajo Escrito (20%)**
- 10 secciones completas
- Contenido técnico detallado
- Análisis y discusión profunda
- Referencias bibliográficas en APA
- Ejemplos de código incluidos

✅ **Presentación (10%)**
- Diseño profesional
- Estructura clara
- Navegación intuitiva
- Formato imprimible

---

## 🔗 Navegación Rápida

```
📚 Reporte Completo
├── 📖 Indice (indice_reporte.html)
├── 📄 Reporte Principal (reporte_final_estructura.html)
├── 📊 Notebooks
│   ├── SentimentAnalysis.ipynb
│   └── MPNet_Embeddings_Analysis.ipynb
└── 📋 Documentación
    └── README_REPORTE.md
```

---

## 💡 Información Técnica

### Herramientas Utilizadas
- **HTML5** - Estructura semántica
- **CSS3** - Diseño responsivo con gradientes
- **JavaScript** - (Potencial para futuras mejoras)
- **Figuras/Gráficos** - Descritos en tablas

### Compatibilidad
- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Navegadores móviles

---

## 📞 Información del Autor

| Campo | Valor |
|-------|-------|
| **Nombre** | Erik Osornio Botello |
| **Proyecto** | Análisis de Sentimientos |
| **Institución** | Centro de Investigación en Computación (CIC) |
| **Programa** | Diplomado en Inteligencia Artificial |
| **Fecha** | Octubre 2025 |

---

## ✨ Notas Finales

Este reporte representa un análisis completo del problema de clasificación de sentimientos, comparando tres enfoques distintos de machine learning. El documento está diseñado para ser tanto un archivo técnico como un recurso educativo, facilitando la comprensión de conceptos de NLP y machine learning aplicados a un caso real.

**¡Gracias por revisarlo! 🙏**
