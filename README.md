# 📊 Comparación de Modelos de Aprendizaje Supervisado — Regresión

Este proyecto corresponde a la **Tarea 1** del ramo *Taller de Inteligencia Artificial*. El objetivo es comparar el desempeño de tres modelos de aprendizaje supervisado aplicados a un problema de **regresión** usando una base de datos pública.

---

## 📚 Descripción del problema

Se utilizó el **California Housing Dataset**, una base de datos pública proveniente del censo de 1990 en California. El objetivo es **predecir el valor medio de las viviendas** en diferentes zonas geográficas, a partir de variables socioeconómicas y demográficas como:

- Ingreso medio por hogar
- Edad promedio de las viviendas
- Número promedio de habitaciones y dormitorios
- Población total
- Ubicación geográfica (latitud y longitud)

Este es un problema clásico de **regresión supervisada**, ya que el valor de la vivienda es una variable continua.

---

## 🧠 Modelos utilizados

Se entrenaron y evaluaron los siguientes modelos:

1. **Regresión Lineal**
2. **Random Forest Regressor**
3. **Support Vector Regressor (SVR)**

Cada modelo fue desarrollado y ejecutado por separado, respetando las buenas prácticas de preprocesamiento y evaluación.

---

## 🗂️ Estructura del repositorio


---

## ⚙️ Preprocesamiento

- Se separaron los datos en **features** (`X`) y **target** (`y`).
- Se realizó una división en conjuntos de entrenamiento y prueba (80% - 20%).
- Se aplicó **escalado estándar (`StandardScaler`)** a los datos para modelos sensibles a la escala (Regresión Lineal y SVR).
- No se aplicó escalado para Random Forest, ya que no lo requiere.

---

## 📈 Resultados y métricas

Las métricas utilizadas fueron:

- **RMSE (Root Mean Squared Error)**: mide el error cuadrático medio.
- **MAE (Mean Absolute Error)**: mide el error absoluto medio.
- **R² (Coeficiente de determinación)**: mide qué tan bien el modelo explica la variabilidad del target.

| Modelo            | RMSE  | MAE   | R²    |
|-------------------|-------|-------|-------|
| Regresión Lineal  | 0.728 | 0.527 | 0.596 |
| Random Forest     | 0.506 | 0.332 | 0.805 |
| SVR               | 0.557 | 0.371 | 0.764 |

---

## ✅ Conclusiones

- El **modelo Random Forest** fue el que obtuvo **mejor desempeño** general en las tres métricas.
- El **modelo SVR** también mostró buenos resultados, mejorando significativamente respecto a la regresión lineal.
- La **regresión lineal** tuvo el rendimiento más bajo, pero es el modelo más simple y explicable, útil como línea base.

---

## 💻 Requisitos

Para ejecutar los scripts es necesario instalar las siguientes librerías:

```bash
pip install -r requirements.txt

