# Ejemplo 02

En las siguientes lineas **encontraras** el ejemplo que viste en el vídeo.

{% tabs %}
{% tab title="Python" %}
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
```
{% endtab %}
{% endtabs %}

