# Ejemplo 01

👨💻 **Ejemplo**

Abrimos nuestra terminal de Python para **crear** el ejemplo del vídeo**.**

![](https://lh6.googleusercontent.com/FKimIYNw_AdG564OEr_PM7ubXdktBvBZJgNYoc7kRIZDzr-W_k8j7YPqkXLZLE38h_vnUfiyP5gMOvNHmOhI6rBlxWU_XK-__-LJ-U5RL-w-9zMOwl1Z99vZLHP4_5-vYZm-13Ms)

Procederemos a crear un diccionario que contenga el nombre y apellido de nuestro instructor.

{% tabs %}
{% tab title="Python" %}
```python
a = {
    'nombre': 'Sergio',
    'apellido': 'Urbina'
}
```
{% endtab %}
{% endtabs %}

Ahora podemos imprimir valores de nuestro diccionario por medio de sus llaves, por ejemplo su **nombre**

{% tabs %}
{% tab title="Python" %}
```python
print(a['nombre'])
```
{% endtab %}
{% endtabs %}

![](https://lh4.googleusercontent.com/l_UneNoUVMdUs0M7R4IKvXi2xmvIcHjrZdf8QOIApaEJ8Y5s8Bzuzyl2fFyLR4bSRThQBBBA31YUj8frawbcjuHZTgGtTyL_8ZDAvo8FvrhPuccFBPpNmtLkB_uX_k4Wr8F2juyv)

Para agregar nuevos valores únicamente debemos asignar una nueva llave con el valor a asignar a nuestro diccionario; por ejemplo para agregar **edad**:

{% tabs %}
{% tab title="Python" %}
```python
a['edad'] = 27
print(a)
```
{% endtab %}
{% endtabs %}

![](https://lh4.googleusercontent.com/YV92V9dUOlFrglCSGmNHEmVPcFO33KkDRZr4PKpzWHIFSJA11em045fXwP-_qoZSGBMETITKzi8e2Z9ap-blmKNE0Zc7knnFrOlW26i7kOaHj7k4noaPnxGnoTiSoBbHrzhaLdI5)

Para borrar un elemento lo podemos realizar de igual manera por medio de la llave con el comando **`del`**

{% tabs %}
{% tab title="Python" %}
```python
del a['nombre']
```
{% endtab %}
{% endtabs %}

![](https://lh5.googleusercontent.com/lfYDRvejjYI8Yd2GQKNQu7wYS-GRr6uR0eZ7tmg0bDWrEkvuRx5omfhnn3TjPA5B1J7t0yOJ5Vypgka95djHuMm6459XwJXT5-CW5YaEtjt7eefiNfEmZmEplgzf1hxxCfQJW8ok)

De igual manera que las **lista** y ****las **tuplas** contamos con diversos métodos que nos pueden ayudar a trabajar con este tipo de dato; a continuación veremos algunos métodos comunes:

El método **`len( )`** nos devuelve la longitud de cualquier estructura, por ejemplo podemos ver cuántos elementos contiene nuestro diccionario.

{% tabs %}
{% tab title="Python" %}
```python
len(a)
```
{% endtab %}
{% endtabs %}

![](https://lh6.googleusercontent.com/NCkDmabFYq-E8wqR02Ccp_2nUDBCC1xHovrjI-2KxRWu5dX_WjvLUoz1rnV7qGq7myhjfmIC38KteRgQz7-Wq5hOmeJCZx9b3DhLDLhSgpyuazlg-tPWxH05uXk_40Ed4rNZy8UH)

El método **`items( )`** nos permite recuperar las claves con su valor, cuando conozcas las estructuras de control este método será de utilidad para recorrer los diccionarios.

{% tabs %}
{% tab title="Python" %}
```python
a.items()
```
{% endtab %}
{% endtabs %}

![](https://lh4.googleusercontent.com/wLbcgH7riZlUw3a1ocjX5Lig6cylWoi-SCvbm4gQUk2-V_W6HOkBPiMtDJSk37v7k1vZ1ykFUoAilmz7P3vjUAFoS68AnOIP4WZ5kBopc4llsjS-5Hez164B7ywDY0j1VH_dlNqU)

Podemos utilizar el método **`keys()`** para obtener las claves del diccionario

{% tabs %}
{% tab title="Python" %}
```python
a.keys()
```
{% endtab %}
{% endtabs %}

![](https://lh4.googleusercontent.com/5p06ugHWrfpCAuAtQu-hZ_YsXG_ecjaVTDXiy50gZi4vn4GhS3A1C8l9_zxgIi91o-VqoIknIwoFg9qxBf1mUYy-U69ZhaujDwyKMkt5JZusNPgAKZa5lcJJe3_u661zGUGIYIzu)

De igual manera podemos utilizar el método **`values( )`** para obtener unicamente los valores

{% tabs %}
{% tab title="Python" %}
```python
a.values()
```
{% endtab %}
{% endtabs %}

![](https://lh5.googleusercontent.com/_OeKBWoWtqUOzsLFfkCyaQ1qshl_oaDgOVX-piI-euqleL_u0UxkXfO0cjL7fnfe3qjrmr3XjvcfSXXh4buiVLZyikWhYrRrV_UGi2r7AISoanOpKAzGpfkFtRGZX0xFhYbjMBre)

También es posible verificar si una clave existe en un diccionario por medio de in o si no existe con **`not in`**

Verificaremos si existe el valor nombre en nuestro diccionario \(El cual nos debería regresar un valor falso\)

{% tabs %}
{% tab title="Python" %}
```python
print('nombre' in a)
```
{% endtab %}
{% endtabs %}

![](https://lh4.googleusercontent.com/vAkdjeO256d9vRcUUOjyBPgv8WP017tjbccVLZLG2cTC9dg-E9wq_33wi_dIr_u_x7xgeaRufS38oIrbkcfJqvs52rOgT_XPeesPAefRmDlG1CCJEQkTousM7HIpRXX_sf0EYQLI)

Realizaremos la pregunta inversa, preguntando si nombre no existe en nuestro diccionario

{% tabs %}
{% tab title="Python" %}
```python
print('nombre' not in a)
```
{% endtab %}
{% endtabs %}

![](https://lh4.googleusercontent.com/dLot_U8jXJK9YgQ_o6O8maJGiZMEa-S8lLtj6ySjtcFddyqMQDaZE-dt538Tm7t5p39VC-Q384fq6Lw_oEjKGy8uMZ0u2hBYy2aMbIh9yk4-9KyFh0cZD22Hg_FqS1LBkK5hUBfV)

