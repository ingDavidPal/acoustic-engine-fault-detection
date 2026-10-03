# acoustic-engine-fault-detection
Machine learning system for detecting and classifying industrial engine faults from acoustic signals using MFCCs and multiple classification models.
# Detección y clasificación de fallos en motores mediante señales acústicas

Proyecto académico desarrollado en la **Escola d'Enginyeria de la Universitat Autònoma de Barcelona (UAB)** para la asignatura de Procesamiento de Señal y Vídeo.

El proyecto desarrolla un sistema de detección y clasificación de fallos en motores industriales a partir del análisis de sus **señales acústicas**, utilizando técnicas de procesamiento digital de señales y aprendizaje automático.

## Autores

- David Pal
- Nicolás Rivard
- Pau Fernández
- Iván Arias

## Descripción

El objetivo del proyecto es analizar grabaciones acústicas de motores industriales para determinar si un motor funciona correctamente o presenta algún tipo de anomalía.

Para ello se utiliza el dataset **MIMII (Malfunctioning Industrial Machine Investigation and Inspection)**, concretamente las grabaciones correspondientes a ventiladores (`fan`).

El sistema transforma las señales de audio en características numéricas mediante **MFCC (Mel-Frequency Cepstral Coefficients)** y utiliza diferentes modelos de aprendizaje automático para realizar la clasificación.

El proyecto contempla tanto:

- **Clasificación multiclase:** distinguir entre motores sanos y diferentes máquinas con fallo.
- **Clasificación binaria:** determinar únicamente si un motor está sano o averiado.

## Pipeline del proyecto

El procesamiento sigue principalmente las siguientes etapas:

```text
Audio del motor
      ↓
Carga de la señal
      ↓
Filtrado pasa-alto
      ↓
Análisis espectral / Espectrograma
      ↓
Extracción de MFCC
      ↓
Normalización de características
      ↓
Clasificación
      ↓
Evaluación de resultados
