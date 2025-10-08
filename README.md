# 📊 Análisis de Proyectos de Inversión Pública en Colombia

### 🧠 **Autor:** Diego  
### 💻 **Herramientas utilizadas:** Python (Pandas, Plotly, Matplotlib, Numpy)  
### 📅 **Versión:** Proyecto completo — *Proyecto_mejorado2.ipynb*

---

## 🟢 **1. Descripción general**

Este proyecto analiza los **proyectos de inversión pública en Colombia**, con el propósito de comprender cómo se distribuyen entre los diferentes **Planes Nacionales de Desarrollo (PND)**, su eficiencia en términos de **inversión y beneficiarios**, y qué porcentaje logra **finalizarse** dentro de los plazos y presupuestos esperados.

La motivación surge de una pregunta clave:  
> **¿En qué medida los proyectos públicos logran cumplir sus objetivos y transformar la inversión en resultados reales para la población?**

---

## 🧭 **2. Objetivos del análisis**

1. Analizar la **distribución de los proyectos** entre los distintos Planes Nacionales de Desarrollo.  
2. Evaluar la relación entre **inversión total**, **cantidad de proyectos** y **beneficiarios**.  
3. Calcular la **eficiencia** de los proyectos (beneficiarios por millón invertido).  
4. Enfocar el estudio en los **proyectos finalizados**, identificando:  
   - Su nivel de eficiencia (eficiente vs. con sobrecostos).  
   - Su **tiempo de ejecución** (corto, medio o largo plazo).  
   - Los **sectores con más impacto** y beneficiarios.

---

## ⚙️ **3. Proceso analítico**

### 🔹 Limpieza y preparación
- Estandarización de nombres y tipos de datos.  
- Clasificación del estado de cada proyecto en tres grupos:
  - **Planeación/Evaluación**
  - **Ejecución**
  - **Finalizado**

### 🔹 Cálculo de métricas
- **Eficiencia:** beneficiarios por millón invertido.  
- **Clasificación de eficiencia:**  
  - *Eficiente:* si el valor total ≤ valor vigente.  
  - *Sobrecosto:* si el valor total > valor vigente.  
- **Tiempo de ejecución:** calculado a partir de columnas `Inicio` y `Fin`, y clasificado en:
  - Corto (1–3 años)  
  - Medio (4–10 años)  
  - Largo (>10 años)

---

## 📈 **4. Visualizaciones clave**

### 🟩 **Distribución de proyectos por PND**
Tres gráficos tipo dona comparan la proporción de proyectos en planeación, ejecución y finalización durante los periodos:
- 2014–2018  
- 2019–2022  
- 2022–2026  

📊 *Insight:* Los proyectos finalizados representan en promedio **solo el 5%** del total.

---

### 🟧 **Relación inversión – beneficiarios – cantidad de proyectos**
Gráfico burbuja (log-log) que muestra cómo los sectores se comportan frente a la inversión y el número de beneficiarios.

📊 *Insight:* Sectores con alta inversión, como *Transporte* o *Educación*, no siempre generan el mayor número de beneficiarios.

---

### 🟥 **Top 5 por inversión vs. eficiencia**
Comparativo entre:
- Los **sectores con mayor inversión total**.  
- Los **sectores más eficientes** en beneficiarios por millón invertido.

📊 *Insight:* La eficiencia no depende del monto. Sectores como *Organismos de Control* o *Rama Judicial* destacan por lograr más con menos.

---

### 🟪 **Eficiencia de proyectos finalizados**
Gráfico de pastel que muestra la proporción de proyectos:
- **Eficientes (88%)**  
- **Con sobrecosto (12%)**

📊 *Insight:* La mayoría de los proyectos que finalizan lo hacen dentro del presupuesto.

---

### 🟦 **Horizonte de ejecución**
Clasificación de los proyectos finalizados según su duración:
- Corto (1–3 años)  
- Medio (4–10 años)  
- Largo (>10 años)

📊 *Insight:* Más del 70% de los proyectos finalizados pertenecen al grupo de corto plazo.

---

### 🟨 **Relación costo – beneficiarios – cantidad (solo finalizados)**
Burbuja logarítmica similar a la anterior, pero enfocada exclusivamente en proyectos finalizados, mostrando el comportamiento real de los sectores que sí cumplieron su ejecución.

---

### 🟫 **Top 5 sectores con más proyectos, inversión y beneficiarios**
Comparación final:
1. **Top 5 por cantidad de proyectos.**  
2. **Top 5 por valor total ejecutado (en billones).**  
3. **Top 5 por beneficiarios alcanzados (en millones).**

📊 *Insight:*  
- *Transporte* lidera en inversión y cantidad de proyectos.  
- *Ciencia, Tecnología e Innovación* se destaca por número de beneficiarios.

---

## 📊 **5. Conclusiones**

- Solo una pequeña fracción de los proyectos alcanza la fase de finalización (**≈5%**).  
- Los proyectos finalizados muestran **alta eficiencia (88%)**, indicando una correcta ejecución presupuestal.  
- Los **plazos cortos** son los más exitosos en términos de finalización.  
- La relación entre **inversión y beneficiarios** demuestra que **mayor gasto no siempre significa mayor impacto.**  
- Sectores como *Transporte* y *Educación* concentran la inversión, pero otros como *Ciencia y Tecnología* generan mayor valor social relativo.

---

## 🧰 **6. Tecnologías empleadas**

- **Python:** análisis, limpieza y visualización.  
- **Pandas & Numpy:** procesamiento y agregación de datos.  
- **Plotly Express:** visualizaciones interactivas.  
- **Matplotlib:** gráficos complementarios.  
- **Jupyter Notebook (VSCode):** desarrollo y narrativa del análisis.

---

## 🚀 **7. Próximos pasos**
- Integrar datos temporales de avance físico-financiero.  
- Analizar correlación entre tipo de proyecto, ubicación y eficiencia.  
- Explorar predicciones de éxito usando Machine Learning.

---

## 🧩 **8. Licencia y créditos**
- **Fuente de datos:** Departamento Nacional de Planeación (DNP).  
- **Autor:** *Diego – Analista de Datos e Ingeniero Industrial.*  
- **Uso:** Proyecto educativo y exploratorio.
