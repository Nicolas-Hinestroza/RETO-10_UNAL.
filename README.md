# RETO-10_UNAL.
Desarrolle la mayoría de ejercicios en clase. Para cada punto cree un programa individual. Al finalizar suba todo a un repo y subalo al canal reto_10 en slack.

- **1. Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.**

![image](https://github.com/Nicolas-Hinestroza/RETO-10_UNAL./assets/124611099/0feccbe6-1455-475c-82f0-0eeb20adeca9)

    r = [1.3, 2.4, -3.0, 4.5, 7.0, 5, -5, 12] # Creamos un arreglo y le definimos como r
    a = 0 # Definimos la variable a igual a 0
    b = len(r) # Definimos la variable b como la cantidad de valores que tiene el arreglo 
    for n in range(0,len(r)): # Para n en un rango de 0 hasta la cantidad de valores del arreglo r
        a += r[0] # a es igual a a + el primer valor de arreglo
        r.pop(0) # Eliminamos el primer valor del arreglo asi se va sumando todos los numeros
    a /= b # La suma de todos los numeros la dividimos entre la cantidad de valores asi sacamos el promedio 
    print("El promedio del arreglo de reales es " + str(a)) # Imprimimos el resultado

- **2. Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.**

![image](https://github.com/Nicolas-Hinestroza/RETO-10_UNAL./assets/124611099/fa59322d-c47f-454a-b79d-27f17ad15ddc)

    a = [-3, 5, -2, 7.0, 8, 3.7] # Definimos el primer arreglo como a
    b = [2, -4, 5, 2, 7.5, -8.4] # Definimos el segundo arreglo como b
    x = 0 # Definimos la variable x igual a 0
    z = 0 # Definimos la variable z igual a 0
    for n in range(0,len(a)): # Para n en un rango de 0 hasta la cantidad de valores del arreglo a
        x = a[0] * b[0] # x es igual al primer valor del arreglo de a multiplicado el primer valor del arreglo de b
        z += x # z es igual a z + x
        a.pop(0) # Eliminamos el primer valor del arreglo a asi se van tomando todos los valores del arreglo a
        b.pop(0) # Eliminamos el primer valor del arreglo b asi se van tomando todos los valores del arreglo b
    print("El producto punto de los dos arreglos de números enteros (reales) es:", z) # Imprimimos el resultado es decir z

- **3. Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.**

![image](https://github.com/Nicolas-Hinestroza/RETO-10_UNAL./assets/124611099/19c2aea7-05bb-49c1-a844-4d5937bf53c3)

    def moverCeros(a): # Definimos la funcion moverCeros con la variable a
        b = []  # Crear una lista para almacenar los ceros
        for n in a:# Para n en un rango de a
            if n == 0: # si n == 0 haga
                b.append(n) # Agregar los ceros a b
        a = [n for n in a if n != 0] # Eliminamos los ceros del arreglo a
        a.extend(b) # Agregar b al final del arreglo es decir a a 
        return a # Nos devuelve el arreglo a
    a = [0, 43, 2, 0, 5, 3, 0, 7, 0, 50] # Definimos el primer arreglo como a
    print("El arreglo es: " + str(a) + " y al mover todos los ceros al final queda el siguiente Arreglo: " +str(moverCeros(a))) # Imprimimos el arreglo
