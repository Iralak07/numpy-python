# numpy-python
  NumPy es uno de los paquetes que debes poder usar y saber si quieres hacer ciencia de datos con Python. 
# Que es numpy?

  NumPy es el paquete fundamental para la computación científica en Python. Es una biblioteca de Python que proporciona un objeto de matriz multidimensional, varios objetos derivados (como matrices y matrices enmascaradas). Para trabajar los ejemplos, necesitamos instalar además de NumPy, la libreria matplotlib

  El objeto principal de NumPy es la matriz multidimensional homogénea.

      matriz = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
  
  Es multidimensional por que cuenta con varias dimensiones a diferencias de las listas comunes en python que solo cuentan con una dimension, con numpy se pueden crear matrices de una, dos, tres, cuatros hasta N dimensiones. En el ejemplo anterior la variable "matriz", es un array con dos dimensiones:

      print(matriz) 
      ''' Resultado:
      [[1 2 3]
       [4 5 6]
       [7 8 9]]
      '''
  Es de dos dimensiones porque cuenta con filas y columnas, en el ejemplo vemos que es un array con tres filas y tres columnas.

  Tambien, vemos que la matriz de numpy es homogenea, esto en razon que todos sus elementos necesariamente son del mismo tipo, es decir no puede existir en un array elementos como numeros enteros, con elementos con numeros flotantes, por lo tanto tienen que ser unicamente del mismo tipo, esto ayuda a poder trabajar facilmente con los mismos y de una forma mas eficiente. En numPy las dimensiones se llaman ejes.

La clase de matriz de NumPy se llama ndarray. También es conocido por el alias array. Los atributos más importantes de un ndarrayobjeto son:



              import numpy as np
              
              a = np.arange(15).reshape(3, 5)
              # con np.arange(15) generamos 15 numeros aleatorios, desl 0 al 14 exluyento al 15
              # luego, con esos numeros creamos un array de tres filas y 5 columnas
              print(a)
                '''
                    [[ 0,  1,  2,  3,  4],
                     [ 5,  6,  7,  8,  9],
                     [10, 11, 12, 13, 14]]
                '''
              print(a.shape) # Resultado:   (3, 5)  
              '''
                Esta es una tupla de enteros que indica el tamaño de la matriz en cada dimensión. Para una matriz con n filas y m columnas,                   shapeserá (n,m).
              '''
              print(a.ndim) # Resultado: 2
              '''
               El número de ejes (dimensiones) de la matriz, en este caso vemos que tiene dos ejes, por lo tanto dos dimensiones, filas y                   columnas
              '''
    
              print(a.dtype.name) # Resultado 'int64' > un objeto que describe el tipo de los elementos en la matriz, en este caso vemos que               son numeros enteros.
              
              print(a.itemsize) # Resultado 8 > el tamaño en bytes de cada elemento de la matriz.
              
              print(a.size) # Resultado 15 > el número total de elementos de la matriz.
              

# Creacion de arrays

  Puede crear una matriz a partir de una lista [1,2,3,4] o tupla (1,2,3,4) normal de Python.

          import numpy as np

          a = np.array([2, 3, 4])
          
          print(a)
          print(type(a))

          '''
          [1 2 3 4]
          <type 'numpy.ndarray'>
          '''

          b = np.array([(1,2,3,4)])
          print(a)
          print(a.shape)
          '''
            [[1 2 3 4]]
            (1, 4)
          '''


Para crear secuencias de números, NumPy proporciona la función 'arange' que es análogo a range incorporado en Python, pero devuelve un formación. 

# Diferencia entre matrices unidimensionales y bidimensionales en NumPy;

# Cómo aplicar algunas operaciones de álgebra lineal a n-dimensionales matrices sin usar bucles for;

# Las propiedades de ejes y formas para matrices n-dimensionales.
