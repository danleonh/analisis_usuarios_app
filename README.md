# Proyecto 13 – Análisis de Usuarios y Métricas de Comportamiento en una App Móvil

## 📋 Descripción general
El propósito de este proyecto fue **analizar el comportamiento de los usuarios dentro de una aplicación móvil**, identificando patrones de uso, embudos de conversión y métricas que permitan optimizar la retención y experiencia del usuario.  
Mediante el análisis de eventos y pruebas estadísticas, se evaluaron las interacciones clave y se generaron recomendaciones basadas en datos para mejorar el rendimiento del producto digital.

---

## 🎯 Objetivos
- Identificar los eventos más relevantes dentro de la aplicación y sus tasas de conversión.  
- Construir y analizar un **embudo de conversión** completo, desde la instalación hasta la compra.  
- Evaluar la efectividad de diferentes versiones de la app mediante una **prueba A/A/B**.  
- Detectar anomalías o desviaciones en el comportamiento de los usuarios entre grupos experimentales.  

---

## 🧮 Datos utilizados
**Dataset principal:**  
- `logs_exp_us.csv` – Registro de eventos de usuarios (timestamp, nombre del evento, usuario, grupo experimental).  

Periodo analizado: julio a agosto de 2019.

---

## 🧰 Herramientas y librerías
- Python  
- pandas, numpy  
- matplotlib, seaborn, plotly  
- scipy (pruebas estadísticas)  
- Jupyter Notebook  

---

## 📊 Etapas del análisis
1. **Carga y preprocesamiento de datos:** limpieza de duplicados, formato de fechas y depuración de eventos.  
2. **Exploración de eventos:** análisis de frecuencia y orden cronológico de acciones dentro de la app.  
3. **Construcción del embudo de conversión:** identificación de tasas entre cada paso del flujo.  
4. **Comparación de comportamiento por grupo (A/A/B):** detección de diferencias significativas.  
5. **Pruebas estadísticas** (Mann–Whitney) para evaluar conversiones entre grupos.  
6. **Conclusiones y recomendaciones.**

---

## 🔍 Resultados principales
- El **embudo principal** incluyó cuatro etapas: instalación → inicio → visualización de producto → compra.  
- La tasa de conversión total fue de **≈ 48 %**, con la mayor caída entre “visualización” y “compra”.  
- Las versiones A1 y A2 mostraron **comportamientos similares**, confirmando la correcta división experimental (A/A).  
- El grupo **B** presentó una **mejora de ~7 % en la tasa de compra**, con diferencia estadísticamente significativa (p < 0.05).  

---

## 💡 Conclusiones
- El experimento valida la efectividad de la versión B, que optimiza el flujo de compra.  
- La distribución de usuarios fue balanceada entre grupos, garantizando confiabilidad en el experimento.  
- Se recomienda mantener las características de la versión B e implementar seguimiento de cohortes para retención.  
- Los resultados demuestran la importancia de un correcto diseño experimental y monitoreo continuo de KPIs.  
