# Todo lo que necesitas saber sobre las funciones de Python

Primero debemos entender que las **funciones en Python** son **objetos**, por lo que podemos asignarlos a **variables**, almacenarlos en **estructuras de datos**, pasarlos como argumentos a otras funciones e incluso devolverlos como valores de otras funciones.

Comprender estos conceptos de forma intuitiva ayudará a comprender las funciones avanzadas en Python como **lambdas** y **decoradores** con mucha facilidad. Revisaremos algunos ejemplos para ayudarnos a desarrollar esta comprensión.

Declararemos una función con la palabra reservada **def** como lo vimos en el vídeo, realizaremos una función que reciba como argumento un nombre y regrese un saludo.

{% tabs %}
{% tab title="Python" %}
```python
def saludo(nombre):
    return "Hola {}!!".format(nombre)

saludo('Sergio')

# Salida

>>> def saludo(nombre):
...     return "Hola {}!!".format(nombre)
...
>>> saludo ('Sergio')
'Hola Sergio!!'
>>>
```
{% endtab %}
{% endtabs %}

### **Las funciones son objetos**

Todos los datos en un programa Python están representados por **objetos** o **relaciones** entre objetos. **Cadenas** \(String\), **listas**, **módulos** y **funciones** son objetos. No hay nada particularmente especial sobre las funciones en Python.

Como la función saludo es un objeto , podemos asignarla a otra **variable**, como cualquier otro objeto:

{% tabs %}
{% tab title="Python" %}
```python
hola = saludo
```
{% endtab %}
{% endtabs %}

La línea anterior **no llamara** a la función. Toma la referencia del objeto de función por saludo y crea un segundo nombre, **hola** , que apunta a él. 

Podemos ejecutar el **método** llamando a **hola**:

{% tabs %}
{% tab title="Python" %}
```python
hola('Sergio')
'Hola Sergio!!'

# Salida

>>> hola = saludo
>>>
>>> hola('Sergio')
'Hola Sergio!!'
>>>
```
{% endtab %}
{% endtabs %}

Los objetos de función y sus nombres son dos cosas separadas. Podemos eliminar el nombre original de las **funciones \( saludo \)** y aún llamar a la función, ya que otro **nombre \( hola \)** todavía apunta a ella.

{% tabs %}
{% tab title="Python" %}
```python
>>> del saludo
>>> 
>>> saludo('Sergio')

Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'saludo' is not defined

>>> 
>>> hola('Sergio')
'Hola Sergio!!'
>>>
```
{% endtab %}
{% endtabs %}

Por lo tanto, una variable que **apunta** a una **función** y la función en sí son **dos funciones** separadas.

### Las funciones se pueden almacenar en estructuras de datos

Dado que las **funciones** son **objetos**, podemos almacenarlas en estructuras de datos, al igual que con otros objetos.

\*\*\*\*🧙♂ **Por ejemplo, podemos agregar funciones a una lista:**

A continuación crearemos una lista con 3 funciones de python:

{% tabs %}
{% tab title="Python" %}
```python
# Salida

>>> funcs = [len, str.isdigit, str.lower]
>>> funcs

[ <built-in function len>,
 <method 'isdigit' of 'str' objects>,
 <method 'lower' of 'str' objects> ]
```
{% endtab %}
{% endtabs %}

Podemos **acceder** a los **objetos** de función almacenados dentro de la lista funciona como lo haría con cualquier otro tipo de objeto.

Realizaremos un **ciclo for** que ejecutara las tres funciones en nuestra lista sobre una cadena:

{% tabs %}
{% tab title="Python" %}
```python
for f in funcs:
print(f,f('Hola mundo!'))
```
{% endtab %}
{% endtabs %}

### **Las funciones se pueden pasar a otras funciones**

Como las funciones son objetos, podemos pasarlas como argumentos a otras funciones.

Crearemos una función llamada **accept** que obtendrá como argumento una función, en este caso enviaremos la función **hola** como argumento.

{% tabs %}
{% tab title="Python" %}
```python
def accept(func):
    msg = func('Sergio')
    print(msg)

accept(hola)
```
{% endtab %}
{% endtabs %}

Podemos influir en el mensaje resultante al pasar diferentes funciones. 

\*\*\*\*🧙 **Por ejemplo creando una función de despedida:**

{% tabs %}
{% tab title="Python" %}
```python
def adios(nombre):
    return "Bye {}!".format(nombre)

accept(adios)
```
{% endtab %}
{% endtabs %}

La capacidad de pasar objetos de función como argumentos a otras funciones es poderosa. Nos permite abstraernos y transmitir comportamientos. 

En el ejemplo anterior, la función de **accept** permanece igual, pero podemos influir en su salida al pasar diferentes comportamientos.

### **Las funciones pueden ser anidadas**

Python permite que las funciones puedan ser **definidas** dentro de otras **funciones**. A menudo se denominan **funciones anidadas** o **funciones internas** .

{% tabs %}
{% tab title="Python" %}
```python
def primeraFuncion(): 
    print ("Mensaje Primera Función")
    def segundaFuncion():
        print ("Mensaje Segunda Función")
    segundaFuncion()

primeraFuncion()
```
{% endtab %}
{% endtabs %}

Ahora, **¿qué está pasando arriba?** Cada vez que llamamos `primeraFuncion` , define una nueva función interna `segundaFuncion` y luego lo llama inmediatamente después.

Además, lo que es notable aquí es: el `segundaFuncion` no existe fuera de `primeraFuncion`:

{% tabs %}
{% tab title="Python" %}
```python
>>> def primeraFuncion():
...     print ("Mensaje Primera Función")
...     def segundaFuncion():
...        print ("Mensaje Segunda Función")
...     segundaFuncion()
...
>>> primeraFuncion()
Mensaje Primera Función 
Mensaje Segunda Función
>>>
>>> segundaFuncion()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'segundaFuncion' is not defined 
```
{% endtab %}
{% endtabs %}

### **Los objetos pueden comportarse como funciones**

Si bien todas las funciones son objetos en Python, lo contrario no es cierto. Los objetos no son funciones. Pero pueden hacerse **invocables**, lo que nos permite tratarlos como funciones en muchos casos.

Si un **objeto** es **invocable**, significa que podemos usar la sintaxis de llamada de función de paréntesis redonda e incluso pasar argumentos de llamada de función. Todo esto funciona con el método **the \_\_call\_\_ dunder**.

🧙 **Un ejemplo de clase que define un objeto invocable:**

{% tabs %}
{% tab title="Python" %}
```python
class Foo:
    def __init__(self):
        print("init")
    def __call__(self):
        print("call")

>>> obj = Foo () 
init 
>>> 
llamada obj ()
```
{% endtab %}
{% endtabs %}

### **Conclusiones:**

* Todo en Python es un objeto, incluidas las **funciones**. Podemos asignarlos a variables, almacenarlos en **estructuras de datos** y pasarlos o devolverlos desde y hacia otras funciones.
* Las funciones nos permiten **abstraer** y **transmitir** el comportamiento en nuestro programa.
* Los objetos pueden hacerse **invocables**. En muchos casos esto nos permite tratarlos como funciones.

**Después revisar el vídeo y analizado la información anterior, es momento de ponerlo en práctica:**

En el contenido adicional del vídeo anterior aprendimos lo fundamental de las funciones en Python, los **siguientes ejercicios** los puedes realizar directamente en la **terminal de Python**, pero recomendamos realizarlos desde el editor de texto y ejecutarlos mediante la terminal como se realizó en los ejercicios de **Listas** y **Tuplas** en el contenido del **vídeo 3** de este curso.

