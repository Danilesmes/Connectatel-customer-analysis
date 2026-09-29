# ConnectaTel - Análisis de Clientes

## Objetivo
Analizar el comportamiento de los clientes de ConnectaTel, una empresa de 
telecomunicaciones en Latinoamérica, para identificar patrones de uso, 
detectar anomalías en los datos y construir segmentos de clientes que 
permitan diseñar estrategias de retención y mejora de planes.

## Datasets utilizados
- `plans.csv` → información de los planes disponibles (precio, minutos, 
  GB incluidos y costos por uso extra).
- `users.csv` → información de los clientes (edad, ciudad, fecha de 
  registro, plan asignado y fecha de cancelación).
- `usage.csv` → detalle del uso real de servicios por cliente 
  (llamadas y mensajes).

## Etapas del análisis
1. **Exploración inicial** → revisión de estructura, tipos de datos y 
   valores nulos de cada dataset.
2. **Limpieza de datos** → tratamiento de sentinel values, fechas fuera 
   de rango, valores inválidos y nulos estructurales.
3. **Análisis estadístico** → estadísticas descriptivas de variables 
   numéricas y categóricas.
4. **Agregación de uso** → construcción de perfil de uso por usuario 
   (mensajes, llamadas y minutos totales).
5. **Visualización** → histogramas y boxplots para analizar distribuciones 
   y detectar outliers.
6. **Detección de outliers** → método IQR para identificar límites superiores 
   en variables de uso.
7. **Segmentación** → clasificación de clientes por nivel de uso y grupo 
   de edad.
8. **Conclusiones ejecutivas** → hallazgos y recomendaciones accionables 
   para el negocio.

## Cómo ejecutar el notebook
1. Abre [Google Colab](https://colab.research.google.com/).
2. Selecciona **File → Upload notebook** y sube el archivo 
   `connectatel_customer_analysis.ipynb`.
3. Sube los archivos `plans.csv`, `users.csv` y `usage.csv` en la 
   sección de archivos de Colab.
4. Ejecuta las celdas en orden desde la primera.

## Guía de reproducción
- Python 3.x
- Librerías necesarias: `pandas`, `numpy`, `matplotlib`, `seaborn`
- Para instalar las librerías ejecuta:
```bash
pip install pandas numpy matplotlib seaborn
```
- Los datasets deben estar en la misma carpeta que el notebook para 
  que las rutas de carga funcionen correctamente.
