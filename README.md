# FINANCIAL FRAUD DETECTION

## PROBLEMA DE NEGOCIO

La urgencia por detectar fraudes en transacciones móviles de dinero ha llevado a una empresa del segmento Fintech a buscar soluciones innovadoras. Como científicos de datos hemos sido convocados para desarrollar un modelo de machine learning que pueda distinguir de manera precisa entre transacciones legítimas y fraudulentas, estableciendo así un estándar de seguridad en el sector financiero móvil global.

## DESCRIPCION DEL PROYECTO

Este proyecto utiliza técnicas de Machine Learning para detectar transacciones fraudulentas en un conjunto de datos. El objetivo es identificar patrones que puedan distinguir entre transacciones legítimas y fraudulentas.

## Herramientas utilizadas
- Colab
- Python
- Librerías:
  - Pandas
  - Numpy
  - Time
  - Matplotlib
  - StringIO
  - Sklearn
  - Imblearn
  - Warnings

## Configuración del Ambiente
Se realizó el trabajo en google Colab con los siguientes pasos:
- Configuración del Ambiente
- Obtención y tratamiento de datos

El archivo Financial_Fraud_Detection_BigData.ipynb es el código escrito en colab el cual contiene todas las operaciones de analisis, limpieza de datos, Insights construcción de modelos y evaluación.
Los datos base fueron extraidos de fuentes oficiales, https://www.kaggle.com/datasets/sriharshaeedala/financial-fraud-detection-dataset

## Pasos Desarrollados
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/pasos.png)

### 1. Preprocesamiento de Datos


### 2. Exploración de Datos

Exploremos los datos del dataframe mediante visualizaciones

![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/distribucion_fraudes.png)
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/boxplot_monto.png)
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/transacciones_x_destinatario.png)
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/transacciones_mes.png)
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/transacciones_fraude.png)
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/transacciones_rango_horario.png)
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/mapa_calor_1.png)

### 3. Construcción de Modelos
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/matiz_confusion.png)
![image](https://github.com/GeraDLC/Financial_Fraud_Detection/blob/main/Unknown.png)

### 4. Evaluación y Selección del Modelo
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/evaluacion_modelos.png)

## Conclusiones:

Determinamos que el modelo Random Forest era la opción más apropiada debido a sus ventajas específicas en términos de métricas de desempeño y capacidad de generalización en conjuntos de datos grandes, complejos y desequilibrados.

La implementación de este modelo en un entorno bancario puede mejorar significativamente la capacidad de detectar y prevenir fraudes, reduciendo así las pérdidas económicas y aumentando la confianza de los clientes en la seguridad de las transacciones.

## Autores

- [@Gerardo](https://github.com/GeraDLC)
- [@Isaias](https://github.com/TigerXHero)
- [@Cristobal]()
