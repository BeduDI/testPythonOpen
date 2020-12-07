# Ejemplo



Crear un módulo en Python es tan sencillo como crear un script, sólo tenemos que añadir alguna función a un fichero con la extensión **.py**, por ejemplo creamos un archivo **saludos.py** con la siguiente función:

{% tabs %}
{% tab title="Python" %}
```python
def saludar():
    print("Hola, te estoy saludando desde la función saludar() " \
            "del módulo saludos")
```
{% endtab %}
{% endtabs %}

Luego ya podremos utilizarlo desde otro **script**,por ejemplo **script.py**, 

{% tabs %}
{% tab title="Python" %}
```python
import saludos
saludos.saludar()

class Saludo():
    def __init__(self):
        print("Hola, te estoy saludando desde el __init__ " \
                "de la clase Saludo")

```
{% endtab %}
{% endtabs %}

![](https://lh6.googleusercontent.com/335WvrBTK1E7McgyQ-QR_wkM7NKi1qYiZ7GueNYeOUnzlUP5M4l9n55fd5-344zmEuVlBec8OZr5Giu8gz6mZja2QD9a0GOeVG4pdqpwe9PJRgIAmWxMAzz8q0j-altqmGNqADI5)

> \*\*\*\*👨💻 **Nota:**
>
> Puedes descargar los archivos del ejemplo: **saludos.py** y **ejemplo1.py**

### **¡Felicidades!** 🎉 

**Has concluido con éxito, el curso de Introducción a Python desde cero, no te olvides de contarnos que tal te ha parecido nuestro contenido respondiendo el siguiente formulario.** 

{% embed url="https://bedu-formularios.typeform.com/to/aBbHND" %}

**¡Hasta la próxima!** 👋 ****

