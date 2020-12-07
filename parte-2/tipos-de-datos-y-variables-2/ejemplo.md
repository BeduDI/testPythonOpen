# Ejemplo

Para realizar los siguiente ejercicios es necesario que tengamos **instalado Python** en nuestr**a** computadora.

En los sistemas operativos Linux y Mac podemos ejecutarlo desde la terminal con el comando **python o python3 \(En el archivo de requerimientos encontrarás los pasos para actualizar a la versión 3 en Mac\).**

![](https://lh4.googleusercontent.com/2nUL2oWTOwf5gU6Ieo8MoEQ7OoQEg20hjR3DAKdS7I1PufCUO9S3RtT9OmjjkHCMolfLwh4f_VEDRceo1CL1-BDor6cB7yJIAAzrB7DSFSykI32MKhjqBP1F2yBfmbBf3EaXPaYr)

En Sistemas operativo Windows una vez instalado , **abriremos la terminal de Python**

![](https://lh5.googleusercontent.com/u7-xxjPqiS3LQ9TbrjzsjfmnjhQM1yg1Ok5NXOs08oXDHg5FxGkyegXM9HmF9hPfvz3ouweOUH24fTETxGWNjSb6QktfA9avrl0rIKWxCIbVsCFS6GsKZhHguC31R-XHN_6s_nxF)

Una vez tengamos ejecutada la terminal de Python vamos a declarar variables, recordando que el valor lo asignamos con el símbolo igual**.**

**Ejemplo**:

{% tabs %}
{% tab title="Python" %}
```python
numero = 5
```
{% endtab %}
{% endtabs %}

![](https://lh4.googleusercontent.com/l0IOr6b8krBYZptcEQFvN-UlUMTip_QN4CGx0-zhXbGfIbodhpzEv1B8JtZFFwr1OLyHC0Ztq_X5SLDVHY5MrGMMYkTlduT2y7CzjoJglgPerBJiUo5iixS7l2xLzmV2rMBIOZvm)

Para imprimir el valor de una variable usaremos el comando **print\( \);** 

**Ejemplo:**

{% tabs %}
{% tab title="Python" %}
```python
print(numero)
```
{% endtab %}
{% endtabs %}

![](https://lh5.googleusercontent.com/0vRZ1V8CKSUAkL7ajTlNm1tCw0osqh2N3a_YRa3o5pc6GrlgWAqXJKipSe7DRl-cdbJ0QbEfDrN9FbTe1no_WOnaZQAD_tnc7EFvk7F7SNbSAqCQvMuzdesvtNSnBXRbStYkvVg3)

Entendido el concepto básico de declaración de variable e impresión procederemos a capturar las siguientes variables:

{% tabs %}
{% tab title="Python" %}
```python
otroNumero = 10
flotante = 5.0
Complejo = 5j
booleano = True
lista = [100,50,25]
tupla = (100, 50, 25)
diccionario = {‘llave1’: ‘valor1’, ‘llave2’: ‘valor2’}
```
{% endtab %}
{% endtabs %}

![](https://lh5.googleusercontent.com/4XwBUP9o-dmnAFS2ef66EsJYocGB5VIFmG3Fmomb7Gq2Qo4EVq_k2S1mtr6ZVH7wXVPCUcu-f2xdM4FMue70YvcZhYkTzCAJKF-sN2QKj4j8YImwKsFTatcdoA69R--voBv4FAkv)

Una vez que tengamos agregados los valores a nuestra consola imprimiremos los valores de las variables con el **comando print\( \)**

{% tabs %}
{% tab title="Python" %}
```python
print(otroNumero)
print(flotante)
print(Complejo)
print(booleano)
print(lista)
print(tupla)
print(diccionario)
```
{% endtab %}
{% endtabs %}

![](https://lh4.googleusercontent.com/22HqambtpUGQVTUNSKxWRrEhqODe2aDmiX0v41coK4l0KoHTE_7DCtmjo8C_fRA96nMNk4pw4tN0hfZeruIgrFI5I-ZCApudYOEDXxr33BtYTRuk1T7DY6MRUGx36jSjpsZzkVIY)

Es posible reasignar los valores de las variables e incluso el tipo de dato de la variable, 

**Ejemplo:**

Cambiaremos el valor de la variable numero que es una variable de tipo numérica a un **string** de valor `cinco` y mandaremos a imprimir nuevamente su tipo de dato, para realizarlo tendremos que ingresar lo siguiente:

{% tabs %}
{% tab title="Python" %}
```python
numero = 'cinco'
print(type(numero))
```
{% endtab %}
{% endtabs %}

![](https://lh5.googleusercontent.com/1gY7XC5GskX6KJULM9XJAxlbVH3oh3mpT1E-CkhMKJCE7PO2XqAFUbctQ5odahohafhg-x9rQfchwzzRSt9mb_y1UzgX_sEEMe11lY2mJaV9q3BJEYtOVRY4GP4gOpYyFgBJe5tM)

Python nos permite realizar operaciones con las variables, volveremos a reasignar un valor numérico a la variable numero  y lo sumaremos con la variable `otroNumero`

{% tabs %}
{% tab title="Python" %}
```python
numero = 5
numero + otroNumero
```
{% endtab %}
{% endtabs %}

![](https://lh3.googleusercontent.com/hdNXwkybTx9pERl14Nk5-qeaggHb1ul-w4rP44qwR1JMccC_Hsf410b9W2D91zTNeqaKwqwBmnBnvSqgA4-ZgAujH2wS35I9pm7OOxNyK7dTj6yI2lPDE_sUcB2YAzWWTyD9m54U)

Debemos tener en cuenta que podemos tener errores si intentemos realizar operaciones con variables de distintos tipos ****

**Ejemplo:** 

**S**i regresamos la variable numero a un **string** `numero` e intentamos sumar nuevamente  con la variable `otroNumero` tendremos como resultado un error

{% tabs %}
{% tab title="Python" %}
```python
numero = 'cinco'
numero + otroNumero
```
{% endtab %}
{% endtabs %}

![](https://lh6.googleusercontent.com/5Tm4mImHRvaTUa6lRT5Z-b2TZVHzTxW9nlJ9xFnwsLnBOMeO5x-muKDKIyQOjlfa95x3vAhorYC5uk0ysvM5mJ63hVFV1oTmfWyu53CioHtO_hn6EGyf4zefy2UkGPNKfQ_wh9Tz)

