# ListasSolucion.py

{% tabs %}
{% tab title="Python" %}
```python
#En las siguientes lineas encontrara el ejemplo que viste en el video 

#Creación de una Lista con 4 Elementos
a = [1, 2, 3, 4]

#Imprimir el primer elemento de una lista
print( a[0] )

#El metodo append nos permite agregar un elemento más a la lista
a.append(5)

#Imprimir la lista (a) completa
print(a)

#Cambiaremos el primer valor de la lista por el string 'Hola'
a[0] = 'Hola'

#Imprimir la lista (a) completa
print(a)

#Con el metodo remove podemos remover un valor en la lista
a.remove(3)

#Imprimir la lista (a) completa
print(a)

#Si intentamos remover un valor inexistente en la lista nos va generar un error
#a.remove(6)

#Con pop podemos eliminar un elemento en alguna posición en la lista, en este caso eliminaremos el primer elemento
a.pop(0)

'''
A continuación debes agregar 5 elementos más en la lista con el metodo append
Una vez agregados los nuevos elementos realizaremos las siguientes tareas:

1. Eliminar el Ultimo elemento de la lista
2. Cambiar el valor del cuarto elemento en la lista
3. Remover el número 2 de la lista
4. Imprimir el sexto valor de la lista
5. Imprimir la lista completa
'''

a.append(6)
a.append(7)
a.append(8)
a.append(9)
a.append(10)

#Solucion Punto 3
a.pop(-1)
#Solucion Punto 2
a[3] = 'Hola'
#Solucion Punto 3
a.remove(2)
#Solucion Punto 4
print(a[5])
#Solucion Punto 5
print(a)
```
{% endtab %}
{% endtabs %}

