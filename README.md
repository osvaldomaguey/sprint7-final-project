# 📱 Análisis de Comportamiento de Usuarios - ConnectaTel

## 🎯 Objetivo del Proyecto

Este proyecto analiza el comportamiento de uso de servicios móviles (llamadas y mensajes) de **ConnectaTel**, una empresa de telecomunicaciones con operaciones en México y Colombia.

**Objetivos principales:**
- Identificar **patrones de uso** de llamadas y mensajes por segmentos de clientes
- Detectar **comportamientos atípicos** que puedan indicar fraude o errores de registro
- Analizar cómo varía el uso según **edad** y **tipo de plan contratado**
- Generar **insights comerciales** para optimizar la oferta de planes y mejorar la experiencia del usuario

## 📊 Datasets Utilizados

El análisis se basa en **tres fuentes de datos principales**:

| Dataset | Descripción | Campos Principales |
|---------|-------------|-------------------|
| `plans.csv` | Catálogo de planes disponibles | precio, minutos incluidos, GB incluidos, costo por extra |
| `users_latam.csv` | Información de clientes | edad, ciudad, fecha de registro, plan contratado, churn |
| `usage.csv` | Detalle de uso real | llamadas (duración), mensajes (longitud), usuario_id |

## 🔍 Etapas del Análisis

### 1. **Exploración y Limpieza de Datos**
- Carga y exploración inicial de los datasets
- Identificación y tratamiento de valores faltantes
- Estandarización de tipos de datos
- Validación de consistencia entre datasets

### 2. **Integración de Datos**
- Unión de las tres fuentes de información
- Creación del dataset consolidado `user_profile`
- Validación de la integridad de los datos integrados

### 3. **Análisis Estadístico Descriptivo**
- Estadísticas descriptivas por segmentos
- Distribución de usuarios por planes y países
- Análisis de patrones de uso (llamadas y mensajes)

### 4. **Detección de Outliers**
- Identificación de valores atípicos en uso de llamadas y mensajes
- Análisis de comportamientos inusuales por segmentos

### 5. **Segmentación de Clientes**
- Creación de grupos por edad: Joven (<30), Adulto (30-60), Adulto Mayor (>60)
- Clasificación por nivel de uso: Bajo, Medio, Alto
- Análisis comparativo entre segmentos

### 6. **Visualización y Insights**
- Gráficos de distribución y comparación
- Análisis visual de patrones por segmentos
- Generación de insights comerciales

## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:
[Google Colab](https://colab.research.google.com/drive/1ovdOllUuPAM9UhAapG6Y8ls37TMBmYNW?usp=sharing)

## 📘 Cómo reproducir el análisis

1. Abre `notebooks/sprint7-final-project.ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/`
