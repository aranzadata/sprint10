Este es un modelo predictivo de aprendizaje supervisado para detectar clientes de Beta Bank en riesgo de cancelar sus cuentas.

Se examina una base de datos de clientes actuales o pasados que contiene identificador de cliente, apellido, edad, género, país, balance, número de productos, 
score crediticio, salario estimado, si tiene una tarjeta de crédito, si es cliente activo y si ha cancelado su cuenta. 
Esta base de datos se segmenta para entrenamiento, validación y prueba. 
Se consideran tres modelos: Regresión Logística, Árbol de Decisión y Bosque Aleatorio. 
Para cada modelo se realizan codificación, estandarización y escalado de datos. 
Posteriormente se hace una exploración para optimizar los hiperparámetrs sin considerar el desequilibrio de clases. 
Se mejoran los modelos utilizando diferentes enfoques para corregir el desequilibrio. 
Se calculan y comparan el valor F1 y la métrica AUC-ROC para cada modelo y se elige el modelo final en base a las mejores métricas.

Para el modelo final se optó por el modelo de Bosque Aleatorio, con 100 estimadores y profundidad máxima de 8. Se utiliza codificación de etiquetas y corrección con sobremuestreo con 3 repeticiones. El puntaje final f1 es de 0.614 y el AUC ROC de 0.853.
