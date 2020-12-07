# control.py

{% tabs %}
{% tab title="Python" %}
```python
#Crearemos dos variables con valores distintos.
x = 10
y = 115

#A continuación crearemos una sentencia de control if para saber si las variables son iguales o diferentes.

if (x == y):
    print('Las variables X y Y son iguales')
else:
    print('Las variables X y Y no son iguales')

#Python Nos permite realizar multipes sentencias por medio de IF..ELIF..ELSE

#Vamos a crear una tercera variable para el siguiente ejemplo:
z = 20

if (x == z):
    print("Las variables X y Z son iguales")
elif (y == z):
    print("Las variables Y y Z son iguales")
else:
    print("Las variables X y Z no son iguales") 

#Cambia el valor Z por el mismo valor que la variable Y, comprueba nuevamente el código anterior
z = 115

if (x == z):
    print("Las variables X y Z son iguales")
elif (y == z):
    print("Las variables Y y Z son iguales")
else:
    print("Las variables X y Z no son iguales") 

#Cambia el valor Z por el mismo valor que la variable X, comprueba nuevamente el código anterior
z = 10

if (x == z):
    print("Las variables X y Z son iguales")
elif (y == z):
    print("Las variables Y y Z son iguales")
else:
    print("Las variables X y Z no son iguales")     

#Realiza ejercicios utilizando todos los operadores de comparación por ejemplo =! o >=
```
{% endtab %}
{% endtabs %}

