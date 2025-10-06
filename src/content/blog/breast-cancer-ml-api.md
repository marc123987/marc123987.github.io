---
title: 'Breast Cancer ML Model API'
description: |
  Este proyecto implementa un modelo de Machine Learning para la clasificación del dataset Breast Cancer usando Random Forest, con una API REST construida con Flask y configuración para despliegue en Kubernetes.
pubDate: 'Aug 25 2025'
coverImageCredit: ''
---

Este proyecto implementa un modelo de Machine Learning para la clasificación del dataset Breast Cancer usando Random Forest, con una API REST construida con Flask y configuración para despliegue en Kubernetes.

<a
  class="text-xl text-primary dark:text-primary-dark underline hover:underline underline-offset-4"
  href="https://github.com/marc123987/breast-cancer-ml-api"
  target="_blank"
>
  Ver Repositorio
</a>

## Descripción

El proyecto incluye:
- Modelo de ML: Random Forest Classifier entrenado con el dataset de Breast Cancer
- API REST: Endpoint Flask para realizar predicciones
- Containerización: Dockerfile para crear imagen Docker
- Kubernetes: Archivos YAML para despliegue en K8s

## Objetivo

Desarrollar un sistema completo que integre un modelo de Machine Learning, exponerlo como API REST mediante Flask y contenedorizado con Docker, automatizando el flujo de trabajo usando buenas prácticas de CI/CD.

## Tecnologías Utilizadas

- Python 3.x
- scikit-learn: Machine Learning
- Flask: API REST
- joblib: Serialización del modelo
- numpy: Computación numérica
- Docker: Containerización
- Kubernetes: Orquestación de contenedores

## Notas

- El modelo Random Forest fue entrenado con 80% del dataset completo de Breast cancer (455 muestras)
- Este proyecto es con fines educativos y demostrativos

## Reflexiones de lo aprendido

En este proyecto se implementó un proceso de CI/CD mediante la plataforma de GitHub Actions y Docker Hub para aprovechar las ventajas de utilizar una imagen de Docker con un ambiente que sea consistente para la correcta compilación y ejecución de la aplicación, independiente de la infraestructura de los usuarios que hagan uso del contenedor generado a partir de dicha imagen.

Además de contar con el control de versiones que provee GitHub para los archivos de código, los archivos con configuraciones de pipelines y otros archivos, así como GitHub Actions que se encarga de compilar, probar y desplegar el código y archivos de la aplicación en la imagen de Docker Hub de forma automatizada, así que es más eficiente ya que así se puede verificar que los cambios subidos no afecten negativamente el comportamiento de la aplicación gracias a las pruebas automatizadas y el despliegue se realiza de forma más rápida.gracias a los jobs o etapas definidas en el pipeline.
