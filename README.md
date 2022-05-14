# Predicción de la demanda de energía eléctrica con RNN LSTM
El proyecto consiste  en predecir valores para una serie temporal del consumo de energía eléctrica de la ciudad de Juliaca específicamente una barra de 10kv. El proyecto contiene los siguientes archivos:
 - juliaca_10kv.xlsx :Historial de la demanda de energia
 - juliaca_10kv_ultimo.xls : datos preprocesados
 - Preproseamiento_de_datos_Juliaca_10kv : contiene el preproceado de los datos
 - lstm : contiene los modelos realizados
 - logs : curvas de entrenamiento, función de perdida vs épocas
 - models : modelos entrenados


Utilicé varias arquitecturas RRN LSTM como simple, apilada y bidireccional de entrada múltiple y salida múltiple, se empezó comparando con que tipos de datos el modelo predice mejor, el primero fue predecir el día actual con los datos de entrada de la semana pasada, el segundo fue predecir el dáa actual con los datos de entrada del día anterior, como resultado se obtuvo que el modelo predice mejor cuando se le suministra los datos del día anterior.

Los datos de entrada son 48 valores correspondientes a la demanda de la energia eléctria y  las salidas tambien son 48 valores.

