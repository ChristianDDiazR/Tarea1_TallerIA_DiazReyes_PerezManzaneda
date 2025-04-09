# Comparación de Modelos de Aprendizaje Supervisado

Este respositorio contiene la implementación de la tarea 1 del taller de IA que consistía en comparar modelos de aprendizaje supervisado.

---

## Problema

Para este caso se utilizó el **California Housing Dataset**, la cual posee diversos datos proveniente del censo de 1990 en California. El obejtivo de este problema es poder predecir el valor promedio de viviendas a partir de los siguientes datos:

- Ingreso medio por hogar
- Edad promedio de las viviendas
- Número promedio de habitaciones y dormitorios
- Población total
- Ubicación geográfica (latitud y longitud)

Este es un problema de regresión, ya que el valor de la vivienda es una variable continua.

---

## Modelos utilizados

1. **Regresión Lineal**
2. **Random Forest Regressor**
3. **Support Vector Regressor**

Los modelos fueron desarrollados de manera independiente con el fin de evitar confusiones, mantener un orden dentro del desarrollo y poder comparar mejor los resultados.

---

## Resultados y métricas

Las métricas utilizadas fueron:

- **RMSE (Root Mean Squared Error)**: mide el error cuadrático medio.
- **MAE (Mean Absolute Error)**: mide el error absoluto medio.
- **R² (Coeficiente de determinación)**: mide qué tan bien el modelo explica la variabilidad del target.

Para efectos de este trabajo, los resultados de las metricas se encuentran en miles de dolares. Esta información es clave para su interpretación.

| Modelo            | RMSE  | MAE   | R²    |
|-------------------|-------|-------|-------|
| Regresión Lineal  | 0.728 | 0.527 | 0.596 |
| Random Forest     | 0.506 | 0.332 | 0.805 |
| SVR               | 0.557 | 0.371 | 0.764 |

---

## Requisitos

Para ejecutar los scripts es necesario instalar las siguientes librerías:

```bash
pip install -r requirements.txt

