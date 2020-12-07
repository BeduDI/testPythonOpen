# Ejemplo 01

En las siguientes líneas encontrara el **ejemplo** que viste en el vídeo 

{% tabs %}
{% tab title="Python" %}
{% code title="listas.py" %}
```python
'''
Creación de una Lista con 4 Elementos
'''
a = [1, 2, 3, 4]

'''
Imprimir el primer elemento de una lista
'''
print( a[0] )

'''
El metodo append nos permite agregar un elemento 
más a la lista
'''
a.append(5)

'''
Imprimir la lista (a) completa
'''
print(a)

'''
Cambiaremos el primer valor de la lista
por el string 'Hola'
'''
a[0] = 'Hola'

'''
Imprimir la lista (a) completa
'''
print(a)

'''
Con el metodo remove podemos remover un valor en 
la lista
'''
a.remove(3)

'''
Imprimir la lista (a) completa
'''
print(a)

'''
Si intentamos remover un valor inexistente en la
lista nos va generar un error
'''
a.remove(6)

'''
Con pop podemos eliminar un elemento en alguna 
posición en la lista, en este caso eliminaremos 
el primer elemento
'''
a.pop(0) 
```
{% endcode %}
{% endtab %}
{% endtabs %}

