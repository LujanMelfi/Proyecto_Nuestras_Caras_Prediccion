# Proyecto_Nuestras_Caras_Prediccion
Red Neuronal usando Backpropagation y TensorFlow para reconocer rostros

# BACKPROPAGATION

Se creó una red neuronal utilizando el algoritmo de Backpropagation a los fines de reconocer el rostro en imágenes de 23 individuos.

Datos de entrenamiento:
Para ello se realizó un análisis PCA de un data set de 230 imágenes, compuesto por 10 fotos de cada individuo. Se determinó el número óptimo de componentes a utilizar. Ese será el input de la red neuronal.

Datos de testeo final:
Se utilizaron 23 fotos (1 por cada individuo) distintas a las fotos utilizadas como datos de entrenamiento. 

## Backpropagation_una_capa_oculta.ipynb
Topología de la Red:

Capa de Entrada: un input por cada componente principal.

Capa Oculta única: se realizaron pruebas para determinar la cantidad de neuronas de esta capa. La función de transferencia será la logística.

Capa de Salida: hay un neurona por cada persona del dataset. La función de transferencia será la logística. La neurona que dispare el valor mayor, será la predicción de la red.

## Backpropagation_dos_capas_ocultas.ipynb
Topología de la Red: es igual a la anterior pero con DOS capas ocultas.
En este caso, se trabajó con el mismo número de neuronas para la primera capa determinado en el script antedicho (número de neuronas óptimo para la predicción: 15).
En este script se realizaron pruebas para determinar la cantidad de neuronas óptimas para la segunda capa oculta (para una buena predicción).

# Cómo usarlo

1. Ejecutar el script "austral_faces_train"
2. Ejecutar el script "austral_faces_test"
3. Ejecutar el script "pca"
4. Ejecutar el script "Backpropagation_una_capa_oculta"
5. Ejecutar el script "Backpropagation_dos_capas_ocultas"

A los fines de ahorrar tiempo y sólo ejecutar los scripts 4 y 5, se agregó al repositorio los archivos “x_pca_reduc.npy” y “x_pca_test_reduc.npy” (son salidas del script 3, necesarias para ejecutarlos).
Las salidas de los scripts 1 y 2 son utilizadas en el script 3.


