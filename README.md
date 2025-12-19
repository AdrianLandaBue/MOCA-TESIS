En esta tesis se presenta el desarrollo e implementación de un sistema basado en aprendizaje profundo para el análisis y clasificación de actividades de conducción a partir de imágenes, con el objetivo de identificar comportamientos potencialmente peligrosos del conductor. La propuesta se apoya en técnicas de visión artificial y en arquitecturas de redes neuronales convolucionales, diseñadas para extraer características visuales relevantes que permitan modelar patrones de comportamiento durante la conducción.

El trabajo considera tanto bases de datos públicas como un conjunto de imágenes recopiladas en escenarios reales, lo que permite evaluar el desempeño del modelo en condiciones controladas y en entornos prácticos. Adicionalmente, se exploran estrategias de preprocesamiento y representación de la información visual, orientadas a simplificar el flujo de datos y mejorar la capacidad discriminativa del modelo.# MOCA-TESIS
 # Identificación de actividades de conducción mediante visión artificial

Este repositorio contiene el código y los recursos utilizados para el desarrollo de la tesis
**"Identificación de patrones de conducción peligrosos mediante visión artificial y aprendizaje profundo"**,
realizada en el marco del programa de Maestría en Optimización y Cómputo Aplicado (MOCA).

---

## 📄 Artículo / Documento de tesis

- 📘 **Tesis completa (PDF)**: [Descargar](docs/Tesis_Adrian_Landa_Buendia.pdf)
- 📝 **Resumen extendido**: [Ver PDF](docs/Resumen_Extendido.pdf)

---

## 🧠 Descripción del proyecto

En esta tesis se propone un sistema basado en redes neuronales convolucionales para la
clasificación automática de actividades de conducción a partir de imágenes, con el objetivo
de identificar comportamientos distractores y potencialmente peligrosos del conductor.

---

## 🗂️ Conjuntos de datos utilizados

- **StateFarm Distracted Driver Detection**
- **Base de datos propia**, capturada en escenarios reales de conducción

> ⚠️ Por motivos de privacidad, las imágenes originales no se distribuyen públicamente.

---

## 🏗️ Arquitecturas implementadas

- CNN secuencial (4 bloques Conv + MaxPooling)
- CNN + Depth Map
- YOLOv8 (Nano / Large)
- Estudio de ablación sobre número de capas y filtros

---

## 📊 Resultados experimentales

| Modelo | Precisión | Parámetros |
|------|-----------|------------|
| CNN Base | 97.1% | 18 MB |
| CNN + Depth | 96.4% | 19 MB |
| YOLOv8n | 98.2% | 6.2 M |

---

## 📦 Estructura del repositorio

```text
├── data/
├── docs/
├── models/
├── notebooks/
├── results/
└── README.md
