# ciclosSolución.py

{% tabs %}
{% tab title="Python" %}
```python
#Ejemplo 1 While
numero = 0
while numero < 10:
    numero = numero + 1
    print(numero)


#Ejemplo 2 While
nombre = ''

while not nombre:
    nombre = input('Escribe tu nombre: ')

#Realiza un programa que imprima del 10 al 1 usando un ciclo while
#Solucion al Reto 1 While
numero = 11
while numero > 1:
    numero = numero - 1
    print(numero)

'''
Haciendo uso de los ciclos while y el método input(), 
realiza un programa que cuente la longitud de una secuencia de números; 
por ejemplo si la secuencia es 342 el resultado deberá ser 3
'''
#Solucion al Reto 2 While
print('Ingresa una secuencia de números: por ejemplo 342')
n = int(input())
length = 0
while n > 0:
    n //= 10  # esto es equivalente a n = n // 10
    length += 1

print(length) 

'''
Ejemplos y Retos: Ciclos For
'''

#Ejemplo 1 Ciclos For - Iterando sobre un rango
for contador in range(1,10):
    print(contador)

#Ejemplo 2 Ciclos For - Iteración de un diccionario por items
frutas = {'Fresa':'roja', 'Limon':'verde', 'Papaya':'naranja', 'Manzana':'amarilla', 'Guayaba':'rosa'}

for nombre, color in frutas.items():
    print(nombre, "es de color", color)

'''
Realizar un programa similar a la iteración del diccionario,
 pero con la diferencia que deberá realizar la toma de valores por medio de la llave en lugar de items()
'''

#Reto 1 - Ciclos For - Iteración de un diccionario por la llave
#Nos es necesario crear de nuevo el diccionario ya que al estar en el mismo archivo tomara el valor de la linea 34

for llave in frutas:
    print(llave, 'es de color', frutas[llave])


'''
Utilizando el método input(), crea un programa que solicite diversos números y los guarde en una lista, 
después deberá iterar sobre la lista de números y multiplicar su valor por sí mismo e imprimir el resultado de dicha multiplicación;
por ejemplo 2 x 2 = 4 , 3 x 3 = 9.
'''

#Reto 2 - Ciclos For - Multiplicación de valores obtenidos

# Creacion de la lista 
lista = [] 
  
# Solicita los números a multiplicar
elementos = int(input("Cuantos números vas a multiplicar : ")) 
  
# itera sobre el número solicitado de números a ingresar
for i in range(0, elementos): 
    nuevoNumero = int(input()) 
  
    lista.append(nuevoNumero)
#Realiza la multiplicación de números     
for mult in  lista:
    print(f"{mult} * {mult} = {mult ** 2}")
```
{% endtab %}
{% endtabs %}

