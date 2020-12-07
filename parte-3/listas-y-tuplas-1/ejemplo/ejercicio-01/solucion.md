# Solucion

\*\*\*\*🧙 **¡Mira lo que se nos ocurrió, para solucionar el problema!**

A continuación debes agregar 5 elementos más en la lista con el **metodo append**

Una vez agregados los nuevos elementos realizaremos las siguientes tareas:

1. Eliminar el Ultimo elemento de la lista

2. Cambiar el valor del cuarto elemento en la lista

3. Remover el número 2 de la lista

4. Imprimir el sexto valor de la lista

5. Imprimir la lista completa

{% tabs %}
{% tab title="Python" %}
{% code title="listasSolución.py" %}
```python
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
{% endcode %}
{% endtab %}
{% endtabs %}

