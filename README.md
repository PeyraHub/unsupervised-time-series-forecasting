# Unsupervised Time Series Forecasting

Descripción general: Predicción de ventas mensuales por unique_id usando series temporales multivariantes. Mejora del benchmark mediante técnicas de feature engineering, cross-validation y modelos avanzados de forecasting.

O 

Descripción general: Proyecto de predicción de ventas mensuales por unique_id usando series temporales multivariantes. Ventana histórica fija y horizonte de 1 mes (Oct-2015).

Contexto del dataset:
- 426 series (unique_id).
- Frecuencia mensual desde 2013-01-31 hasta 2015-10-31 (34 meses por serie).
- Columnas principales:
    - date (fecha mensual),
    - unique_id (identificador de la serie),
    - monthly_sales (👈 objetivo y),
    - exógenas: city_id, shop_id, item_category_id, item_id, monthly_average_price.

Objetivo: predecir monthly_sales para Oct-2015 por cada unique_id.

Alcance/limitaciones:
- No mezclar futuro en el pasado (evitar leakage).
- Datos con faltantes en monthly_sales (~5%) y monthly_average_price (~8.4%): habrá que tratarlos.

Relevancia: practicar pandas, feature engineering temporal, cross-validation correcta en TS, entender diferencia LB público vs privado en Kaggle y por qué un modelo puede sobreajustar al público.