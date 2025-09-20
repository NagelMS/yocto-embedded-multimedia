# Bitacora Nagel Eduardo Mejía Segura

## 31 de Agosto de 2025

- Se realizó una investigación inicial, así como la instalación de GStreamer y OpenCV.
- Siguiendo los tutoriales para ambas herramientas, se verificó el correcto funcionamiento inicial por medio de programas simples de Python.

Referencias: 
- https://docs.opencv.org/4.x/d3/d96/tutorial_basic_geometric_drawing.html 
- https://gstreamer.freedesktop.org/

## 15 de setiembre de 2025

- Se realizaron pruebas en opencv para poder realizar la detección de las cajas, primero se realizó por cuenta propia un código que utilizaba detector de bordes Canny, y seguidamente se utilizaba opencv para obtener los contornos.

Problemas Encontrados: No lograba detectar la mayoría de cajas, al revisar la imagen generada tras la detección de bordes, había mucho ruido esto provocaba que algunas cajas no se detectaran como tal ya que no concordaba con la forma del poligono buscado.

## 16 de setiembre de 2025

- Se investigó sobre formas de hacer la detección de cajas, se implementó un diseño de un repositorio coreano el cual resultó ser más robusto, de igual forma se seguirá investigando formas alternativas.

Problemas: Si bien el detector es robusto, aveces detecta poligonos "cuadrados" como cajas.

Referencias: https://github.com/KEG012/Project_openCV_Box_Detector

## 19 de setiembre de 2025

- Se organizó de mejor forma los códigos de python generando un programa principa (main.py), que utiliza los códigos de python del nuevo directorio de fuentes (src) para la detección de cajas (detector.py), el procesamiento del video (video_processor.py) y un código para implementar configuraciones generales (config.py).

Problemas: **ERROR** el programa de python no está funcionando por medio del pipeline de gstreamer, con opencv puro sí lo logra.
