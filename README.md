Este repositorio contiene el código y los recursos utilizados para el desarrollo de la tesis
**"Identificación de Comportamientos de Conducción Peligrosos en Servicios de Transporte Mediante aprendizaje profundo."**,
realizada en el marco del programa de Maestría en Optimización y Cómputo Aplicado (MOCA).

Asi mismo, la tesis presenta el desarrollo e implementación de un sistema basado en aprendizaje profundo para el análisis y clasificación de actividades de conducción a partir de imágenes, con el objetivo de identificar comportamientos potencialmente peligrosos del conductor. La propuesta se apoya en técnicas de visión artificial y en arquitecturas de redes neuronales convolucionales, diseñadas para extraer características visuales relevantes que permitan modelar patrones de comportamiento durante la conducción. 
<img width="5374" height="1280" alt="Input 150 x 150" src="https://github.com/user-attachments/assets/b23c1e0a-936b-48cc-a571-79d0c2a989bf" />


El trabajo considera tanto bases de datos públicas como un conjunto de imágenes recopiladas en escenarios reales, lo que permite evaluar el desempeño del modelo en condiciones controladas y en entornos prácticos. Adicionalmente, se exploran estrategias de preprocesamiento y representación de la información visual, orientadas a simplificar el flujo de datos y mejorar la capacidad discriminativa del modelo.# MOCA-TESIS
 # Identificación de Comportamientos de Conducción Peligrosos en Servicios de Transporte Mediante aprendizaje profundo.


---

## 📄 Artículo / Documento de tesis

- 📘 **Tesis completa (PDF)**: [Descargar](docs/Tesis_Adrian_Landa_Buendia.pdf)
- 📝 **Articulo publicado**: [Ver PDF](https://link.springer.com/book/10.1007/978-3-031-97907-1)

---

## 🧠 Descripción del proyecto

En esta tesis se propone un sistema basado en redes neuronales convolucionales para la
clasificación automática de actividades de conducción a partir de imágenes, con el objetivo
de identificar comportamientos distractores y potencialmente peligrosos del conductor.

---

## 🗂️ Conjuntos de datos utilizados

- **StateFarm Distracted Driver Detection** (https://www.kaggle.com/c/state-FARM-distracted-driver-detection)
- **Base de datos propia**, capturada en escenarios reales de conducción

> ⚠️ Por motivos de privacidad, las imágenes originales no se distribuyen públicamente.

---

## 🏗️ Arquitecturas implementadas

- CNN secuencial (4 bloques Conv + MaxPooling)
- CNN + Depth Map
- YOLOv8 (Nano / Large)
- CNN + KNN / RF
- Estudio de ablación sobre número de capas y filtros

---

## 📊 Resultados experimentales

| Modelo                                               | Base de datos     | Precisión  |
| ---------------------------------------------------- | ----------------- | ---------- |
| **CNN (This Research)**                              | State Farm D.D.D. | **98.10%** |
| **CNN + Algoritmo de clasificación (This Research)** | -                 | –          |
| KNN                                                  | State Farm D.D.D. | 86.67%     |
| Random Forest (RF)                                   | State Farm D.D.D. | 81.71%     |
| **YOLOv8 (This Research)**                           | State Farm D.D.D. | 96.40%     |
| **CNN + Depth Map (This Research)**                  | State Farm D.D.D. | **98.55%** |


---

