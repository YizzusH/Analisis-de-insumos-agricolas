# Decisión de Inversión en Insumos Agrícolas mediante Diseño en Cuadrado Latino

> **📊 Ver Reporte Interactivo (HTML):**  
> 👉 [Abrir reporte completo en GitHub Pages](https://yizzush.github.io/Analisis-de-insumos-agricolas/)

---

## Planteamiento del Problema
En una campaña agrícola, asignar presupuesto entre distintas opciones de **semillas**, **fertilizantes** y **plaguicidas** sin evidencia controlada expone a decisiones costosas: gastar en insumos con bajo retorno marginal o atribuir el rendimiento al factor equivocado.

Este caso de estudio aborda la selección de insumos como una **decisión de inversión respaldada por estadística**, evaluando **4 opciones de semilla**, **4 opciones de fertilizante** y **4 opciones de plaguicida** bajo un **Diseño en Cuadrado Latino (DCL) $4 \times 4$**.

---

## Metodología y Análisis Estadístico en R
* **Diseño experimental:** Cuadrado Latino $4 \times 4$ ($16$ unidades experimentales) controlando simultáneamente dos fuentes de variación (fertilizantes como filas y plaguicidas como columnas) para aislar el efecto de las semillas.
* **Análisis de Varianza (ANOVA):** Evaluación de significancia estadística de los factores sobre el rendimiento.
* **Diagnóstico de supuestos del modelo:**
  * Normalidad de los residuos mediante **Shapiro-Wilk**.
  * Homocedasticidad mediante la prueba de **Bartlett**.
  * Independencia de los residuos mediante **Durbin-Watson**.
* **Comparaciones múltiples (post-hoc):** Contraste entre **LSD** y ajuste por **Bonferroni** para identificar grupos de rendimiento y equilibrar potencia estadística con prudencia ante el costo de equivocarse.

---
