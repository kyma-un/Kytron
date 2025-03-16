# Proyecto de Identificación de Circuitos Eléctricos con Computer Vision ⚡👁️

Este proyecto tiene como objetivo desarrollar una herramienta que utiliza modelos de *computer vision* para identificar elementos (símbolos) y sus conexiones en diagramas de circuitos eléctricos, y generar automáticamente un archivo SPICE que puede ser cargado en simuladores como **LTSpice**. Utilizamos técnicas avanzadas como **detección de múltiples objetos**, **transformadas de Hough** y **descriptores ORB** para lograr esta tarea.

## 🚀 Descripción

La idea principal del proyecto es automatizar la conversión de diagramas de circuitos eléctricos a archivos SPICE, lo que facilita la simulación y el análisis de circuitos sin necesidad de ingresar manualmente los componentes en el simulador.

### Técnicas clave:
- **Detección de múltiples objetos (multi-object detection):** Identificación de componentes y conexiones en el circuito.
- **Transformadas de Hough:** Para detectar líneas y patrones geométricos en el diagrama.
- **Descriptores ORB (Oriented FAST and Rotated BRIEF):** Para extraer características robustas de los símbolos del circuito y emparejar objetos entre imágenes.

## 🎯 Objetivos

- **Identificación de elementos**: Detectar componentes eléctricos como resistencias, condensadores, transistores, etc.
- **Detección de conexiones**: Identificar las conexiones entre los componentes en un diagrama de circuito.
- **Generación de archivo SPICE**: Convertir la información del circuito identificado en un archivo SPICE compatible con simuladores como LTSpice.
- **Automatización del proceso de simulación**: Facilitar la creación de simulaciones de circuitos a partir de diagramas en papel o imágenes.

## 🧠 Técnicas Utilizadas

1. **Detección de múltiples objetos (Multi-object Detection)**:
   - Utilizamos redes neuronales o técnicas de visión por computadora, como *YOLO* o *Faster R-CNN*, para detectar y clasificar los componentes eléctricos del diagrama.
   
2. **Transformadas de Hough**:
   - Aplicamos la transformada de Hough para identificar líneas y formas geométricas que representan las conexiones entre los componentes del circuito. Esto es útil para reconstruir las conexiones eléctricas.

3. **Descriptores ORB**:
   - Los descriptores ORB son útiles para detectar características clave en los componentes del circuito. Son resistentes a cambios de escala y rotación, lo que facilita la correspondencia entre imágenes de circuitos de diferentes perspectivas o tamaños.

## 🛠️ Instalación

### Requisitos:
- Python 3.x
- OpenCV
- NumPy
- Matplotlib
- TensorFlow / PyTorch (dependiendo de la implementación de detección de objetos)
- SPICE-compatible simulador como **LTSpice** o **NgSpice**

### Instalación de dependencias:

```bash
pip install opencv-python numpy matplotlib tensorflow
```

