# ¿Qué son los paquetes y cómo los uso?

Los paquetes son colecciones de módulos que puedes **crear** y **usar**.

Es posible importar módulos directamente en el directorio donde ejecuta el programa por medio del comando **import**, pero si desea importar módulos de otros directorios, debe informar a Python que el directorio desde el que está importando es un paquete de Python. Para hacer eso, coloca un archivo llamado **\_\_init\_\_.py** en ese directorio.   
 🧙♂ **Por ejemplo**, en un programa de música donde queremos usar distintos módulos:

{% tabs %}
{% tab title="Python" %}
```python
sound/                          Top-level package
      __init__.py               Initialize the sound package
      formats/                  Subpackage for file format conversions
              __init__.py
              wavread.py
              wavwrite.py
              aiffread.py
              aiffwrite.py
              auread.py
              auwrite.py
              ...
      effects/                  Subpackage for sound effects
              __init__.py
              echo.py
              surround.py
              reverse.py
              ...
      filters/                  Subpackage for filters
              __init__.py
              equalizer.py
              vocoder.py
              karaoke.py
              ...

```
{% endtab %}
{% endtabs %}

Supongamos que desea utilizar el módulo **equalizer** en su programa separado \(es decir, uno que no está en este directorio\). tendría que realizar lo siguiente:

{% tabs %}
{% tab title="Python" %}
```python
import sound.filters.equalizer as equalizer
```
{% endtab %}
{% endtabs %}

Como **sound** es el paquete raíz, esa sería la primera sección de la declaración de importación. **filters** es el paquete que contiene el módulo **ecualizador**, así que esa es la siguiente sección. **equalizer** es lo que realmente estamos tratando de importar, así que esa es la última sección. Las declaraciones de importación se usan como una forma de mostrar el árbol de directorios. 

La declaración **as** no es necesariamente necesaria, pero si no la cambia, ¡tendría que escribir **sound.filters.equalizer** cada vez que quiera usar un método **equalizer.py** Usando as, solo tenemos que escribir **equalizer**. Como alternativa se puede escribir el siguiente código:

{% tabs %}
{% tab title="Python" %}
```python
from sound.filters import equalizer
```
{% endtab %}
{% endtabs %}

Ahora, Python solo importará esa única variable desde **equalizer**.

Tampoco tiene que importar un solo artículo. Si el módulo está en el mismo paquete \(o si la **variable / función** está en el mismo módulo, dependiendo de cómo esté importando\), puede encadenarse usando comas.

{% tabs %}
{% tab title="Python" %}
```python
from sound.filters import equalizer, vocoder
```
{% endtab %}
{% endtabs %}

> \*\*\*\*💡 **Nota:**
>
> Si desea importar **\* todo \*** desde un módulo, puede usar un asterisco.

{% tabs %}
{% tab title="Python" %}
```python
from sound.filters.equalizer import *
```
{% endtab %}
{% endtabs %}

Sin embargo, esto va en contra de la guía de estilo de python **PEP8**. Donde se recomienda que seas detallado con lo que estás importando.

Sin embargo, para importar todo desde un paquete, el autor del paquete debe hacer algo un poco más especial.

Utilizando el archivo **\_\_init\_\_.py** , debe establecer una variable llamada  **\_\_all\_\_** que contenga todos los módulos en el paquete, así:

{% tabs %}
{% tab title="Python" %}
```python
__all__ = ['equalizer', 'vocoder', 'karaoke']
```
{% endtab %}
{% endtabs %}

De esa manera, **import \***importará esos tres módulos.

### **Importancia relativa**

También puede importar módulos relativamente. Digamos que estás en el **módulo echo**  y quieres llamar a algo desde el **ecualizador.** Esa declaración de importación se vería así.

{% tabs %}
{% tab title="Python" %}
```python
from ..filters import equalizer
```
{% endtab %}
{% endtabs %}

> 💡 **Nota:**
>
> Separa las carpetas, como aprendimos anteriormente, así que eso es lo mismo que ir **effects -&gt; sound -&gt; filters**

### **Obteniendo paquetes externos**

Hay varios sitios web para obtener paquetes útiles que necesita, siendo el más grande **PyPi.** Para instalar paquetes desde PyPi, ejecute el comando **pip i**ncluido en su instalación de Python. Como ejemplo, supongamos que desea instalar la biblioteca **requests.** 

Es posible encontrar la biblioteca en el siguiente recurso

{% embed url="https://pypi.org/project/requests/" %}

Pera para **instalarlo** usaremos el siguiente comando:

```coffeescript
pip install requests
```

Si estás en **Linux o Mac** y no en un entorno virtual, tendrás que ejecutar sudo\(aunque se recomienda el uso de un entorno virtual **como virtualenv\)**

\*\*\*\*

