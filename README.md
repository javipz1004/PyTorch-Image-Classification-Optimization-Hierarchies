# 🧠 Clasificación Avanzada y Optimización en PyTorch (CIFAR)

Este repositorio contiene un estudio profundo sobre la optimización de procesos de entrenamiento y la implementación de lógica probabilística en redes neuronales utilizando el framework **PyTorch**.

## 🚀 Contenido del Proyecto

El proyecto se divide en dos fases técnicas complementarias:

### Fase 1: Optimización y Aceleración de Hardware (CIFAR-10)
En esta etapa, el foco principal fue la eficiencia del entrenamiento y la gestión de recursos de cómputo.
- **Benchmark CPU vs GPU:** Evaluación del factor de aceleración al utilizar dispositivos CUDA.
- **Data Pipeline Optimizado:** Implementación de carga de datos eficiente enviando tensores directamente a la VRAM.
- **Control de Overfitting:** Integración de *Early Stopping* basado en la pérdida de validación.

### Fase 2: Clasificación Jerárquica con Probabilidad Condicionada (CIFAR-100)
Aquí se abordó un problema complejo de 100 clases utilizando la estructura de superclases (*coarse labels*) para mejorar la coherencia de las predicciones.
- **Arquitectura Multitarea:** El modelo predice simultáneamente etiquetas finas y gruesas.
- **Lógica Bayesiana:** Aplicación de probabilidad condicionada $P(A|B)$ para filtrar predicciones. Por ejemplo, el sistema valida que una predicción de "Perro" sea coherente con la superclase "Mamíferos".

## 📂 Estructura del Repositorio
- `notebooks/`: Contiene los archivos `.ipynb` con el código y las explicaciones paso a paso.
- `requirements.txt`: Librerías necesarias para replicar el entorno.
- `images/`: Capturas de las métricas de entrenamiento y comparativas de tiempo.

## 🛠️ Instalación y Uso
1. Clona este repositorio:
   ```bash
   git clone [https://github.com/TU_USUARIO/TU_REPO.git](https://github.com/TU_USUARIO/TU_REPO.git)

2. Instala las dependencias:
   ```bash
   pip install -r requirements.txt

## 📊 Resultados Destacados

* Se logró una aceleración significativa mediante el uso de **GPU T4**, optimizando los tiempos de entrenamiento frente a la ejecución en CPU.
* La implementación de la lógica jerárquica permitió estructurar mejor las predicciones en el dataset **CIFAR-100**, utilizando probabilidad condicionada para reducir errores semánticos entre clases finas y superclases.

---
**Autor:** Francisco Javier Pérez Cazorla  
*Proyecto académico para la asignatura de Programación para la Inteligencia Artificial.*
