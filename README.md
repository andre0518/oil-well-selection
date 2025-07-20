# Selección de región para pozos petrolíferos (OilyGiant)

Este proyecto forma parte del Sprint 11 del Bootcamp de Data Science de TripleTen. El objetivo es ayudar a la empresa OilyGiant a seleccionar la mejor región para perforar **200 nuevos pozos petrolíferos**, a partir de datos geológicos sintéticos de tres regiones distintas.

---

## 🎯 Objetivo

- Predecir el volumen de reservas (en miles de barriles) para cada pozo.
- Seleccionar los 200 pozos más prometedores de cada región.
- Calcular la ganancia esperada y el riesgo de pérdida por región.
- Aplicar técnicas estadísticas como **regresión lineal** y **bootstrapping** para una decisión informada.
- Recomendar la mejor región considerando **rentabilidad y riesgo financiero**.

---

## 📁 Archivos

- `Proyecto_11_OilyGiant.ipynb`: Notebook principal con todo el análisis, entrenamiento y resultados.
- `README.md`: Este archivo.

---

## 🧪 Tecnologías utilizadas

- Python
- Pandas
- Numpy
- Scikit-learn
- Matplotlib / Seaborn

---

## 🗂️ Datos

Los datasets utilizados son sintéticos y provienen de las siguientes fuentes (vía plataforma de entrenamiento):

- `/datasets/geo_data_0.csv`
- `/datasets/geo_data_1.csv`
- `/datasets/geo_data_2.csv`

Cada archivo contiene:
- `id`: Identificador del pozo.
- `f0`, `f1`, `f2`: Características geológicas.
- `product`: Volumen de reservas (objetivo de predicción).

---

## 💰 Condiciones del negocio

- Se perforarán 200 pozos de entre 500 disponibles por región.
- Presupuesto: **100 millones USD**.
- Ganancia por mil barriles: **$4,500 USD**.
- Umbral de rentabilidad: **111.1 unidades (mil barriles) por pozo**.
- La región elegida debe tener un riesgo de pérdida menor al 2.5%.

---

## 📊 Resultados

Tras aplicar regresión lineal y simulaciones con bootstrapping:

| Región   | Ganancia promedio (USD) | Intervalo de confianza 95%      | Riesgo de pérdida |
|----------|--------------------------|----------------------------------|--------------------|
| Región 0 | $33,114,819.57           | $29,851,975.21 – $36,131,172.69 | 0.00%              |
| Región 1 | $24,150,866.97           | $24,150,866.97 – $24,150,866.97 | 0.00%              |
| Región 2 | $27,147,417.89           | $23,795,874.85 – $30,629,774.58 | 0.00%              |

---

## ✅ Conclusión

> Se recomienda **perforar en la Región 0**, ya que ofrece la mayor ganancia promedio, un intervalo de confianza favorable y un riesgo nulo de pérdida.

---

## 👩‍💻 Autora

**Andreina Moreno**  
[LinkedIn](https://www.linkedin.com/in/andreina-moreno-franco)  
[GitHub](https://github.com/andre0518)