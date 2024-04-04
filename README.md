#Codigo realizado por Juan Ignacio Muñoz 4/4/2024 

# Simulación de Semáforos con Detección de Vehículos

Este proyecto simula un sistema de semáforos inteligente que ajusta su temporización en función de la detección de vehículos en la intersección. Utiliza la detección de objetos YOLOv5 para contar vehículos en un video y ajusta el estado de seis semáforos en una interfaz gráfica de usuario (GUI) desarrollada con Tkinter.

## Características

- **Detección de vehículos:** Utiliza YOLOv5 para detectar vehículos en tiempo real a través de un video.
- **Simulación de semáforos:** Cambia el estado de los semáforos (verde, amarillo, rojo) basándose en la detección de vehículos.
- **GUI con Tkinter:** Muestra una interfaz gráfica con seis semáforos y su estado actual.
- **Ajuste inteligente:** El semáforo principal (Semáforo 1) puede prolongar su luz verde si detecta una cantidad significativa de vehículos esperando.

## Tecnologías Utilizadas

- Python 3
- [YOLOv5](https://github.com/ultralytics/yolov5) para detección de vehículos
- [Tkinter](https://docs.python.org/3/library/tkinter.html) para la interfaz gráfica

## Estructura del Proyecto

El proyecto consta de varios componentes principales:

- `main.py`: El script principal que ejecuta la simulación.
- `semaphore_simulation.py`: Contiene la lógica para la simulación de semáforos y la GUI.
- `vehicle_detection.py`: Encargado de la detección de vehículos utilizando YOLOv5.
- `data/`: Directorio que contiene el video de entrada para la detección de vehículos.

## Requisitos

Para ejecutar este proyecto, necesitarás:

- Python 3.6 o superior
- Dependencias listadas en `requirements.txt`

## Instalación

1. Clona este repositorio en tu máquina local.
2. Instala las dependencias necesarias:
   ```bash
   pip install -r requirements.txt
