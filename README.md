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
En este paso hemos eliminado columnas que consideramos no relevantes y hemos hecho separación de columnas por tipo de transacción y tipo de destinatario.

### 2. Exploración de Datos

*   Existe un **desbalanceo** muy grande entre la variable objetivo, es necesario hacer un **balanceo** mas adelante para obtener un mejor modelo.

![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/distribucion_fraudes.png)
  
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/transacciones_x_destinatario.png)

*   Sólo tenemos **8103 registros** catalogados como **fraude**, de los cuales fueron de cliente a cliente.
*   De dichos registros, están muy equilibradas en un 50-50 por  **Retiro** y**Transferencia**.

Es interesenta notar que no hay transacciones fraudulentas por **Cliente a Comercio**, ni por los conceptos de: **Depósito, Débito, Pago**.

![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/transacciones_mes.png)

*   Una gran cantidad de transacciones ocurren los primeros días del mes, se puede deber a que a la mayoría de las personas perciben su salario mensualmente y deciden hacer transacciones.
*   También existe una gran concentración de transacciones entre los días 6-17 del mes, algunas perconas podrían recibir sus ingresos cada quince días o semanalmente.
*   Es muy común que para los días finales del mes, las personas hayan terminado con gran parte de su dinero, lo que explicaría las pocas transacciones entre los días 18-31.

![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/transacciones_fraude.png)
![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/transacciones_rango_horario.png)

*   Se suelen hacer más transferencias en las tardes y noches que en la mañana y madrugada. Tiene sentido ya que es cuando las personas no se encuentran en la escuela y/o trabajo.
*   El último día del mes tuvo 268 transaciones, de las cuales todas fueron fraudulentas.

### 3. Construcción de Modelos
Observamos que los dos mejores modelos con mejores métricas son **Random Forest** y **Árbol de Decisión** con un número bajo de Falsos Negativos y buenas clasificaciones.

![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/matiz_confusion.png)
![image](https://github.com/GeraDLC/Financial_Fraud_Detection/blob/main/Unknown.png)

### 4. Evaluación y Selección del Modelo
**Hemos decidido escoger el modelo Random Forest por sus buenas métricas en general.** Aunque Árbol de Decisión tambien obtuvo buenas métricas y en un tiempo menor, consideramos que Random Forest se acopla mejor al problema de negocio para grandes cantidades de datos

En este caso, Recall es una métrica clave para poder disminuir el numero de fraudes NO detectados correctamente como fraude.

![image](https://github.com/TigerXHero/Financial-Fraud-Detection/blob/main/images/evaluacion_modelos.png)

## Conclusiones:

Sería beneficioso continuar evaluando y mejorando el modelo utilizando conjuntos de datos más grandes y variados, así como explorar técnicas adicionales de preprocesamiento de datos y ajuste de hiperparámetros para mejorar aún más su desempeño en diferentes contextos bancarios y en un entorno de producción.

En conclusión, el uso del algoritmo **Random Forest** para la detección de fraudes bancarios ha demostrado ser una elección acertada, proporcionando un balance óptimo entre precisión, capacidad de generalización y eficiencia, lo que lo convierte en una herramienta valiosa para combatir el fraude en el sector bancario.

## Autores

- [@Gerardo](https://github.com/GeraDLC)
- [@Isaias](https://github.com/TigerXHero)
- [@Cristobal]()
