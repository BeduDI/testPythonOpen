# SolucionTuplas.py

```python
#Crearemos la tupla que vivmos en el video
tupla = (5, "Hola mundo!@", True, -1.5, True)
print(tupla)

#Recordemos que las tuplas no son modificables, por lo que si tratamos agregar un elemento con .append() tendemor un error TypeError
#tupla.append(6)

#Como vimos en el video es posible recorrer las tuplas por índices negativos 
print(tupla[-1])

#A continuación aprenderas nuevos metodos que puedes utilizar con tuplas

#El método count() nos permite contar cuantas veces se repite un elemento en la tupla
#En este ejemplo revisaremos cuantas veces se repite el valor True en tupla
tupla.count(True)

#El método index() recibe un argumento y devuelve el indice de su primera aparición en la tupla
#Por ejemplo si buscamos en que posición se encuentra el valor -1.5
tupla.index(-1.5)

'''
A continuación Realiza las siguientes actividades:

1. Crea una tupla con 7 elementos, que incluya por lo menos una lista
2. Imprime el elemento número 5, tanto por su índice como por su índice negativo
3. Utiliza el método count con dos valores distintos de la tupla
4. Utiliza el método index con dos valores distintos de la tupla
5. Imprime el valor de la lista dentro de la tupla


'''

#Solucion punto 1
lista = [1,2,3]
solucion = (1, True, tupla , "Otro mensaje", 5j, False, lista)

#Solucion punto 2
print(solucion[4])
print(solucion[-3])

#Solucion punto 3
solucion.count(5)
solucion.count(lista)

#Solucion punto 4
solucion.index(tupla)
solucion.index(5j)

#Solucion punto 5
print(solucion[-1])



```

