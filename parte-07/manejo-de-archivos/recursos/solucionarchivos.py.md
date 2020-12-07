# solucionArchivos.py

{% tabs %}
{% tab title="Python" %}
```python
'''
Realiza el código necesario para crear un fichero vacío llamado numeros.txt 
y después agregue una secuencia del 0 al 100.
'''
from io import open

secuencia = open('numeros.txt','a+')

for numero in range(0, 101):
    secuencia.write(str(numero))
    secuencia.write('\n')

secuencia.close()



'''
Crear un programa que abra un fichero en modo lectura y escritura,
 si no existe lo creará, y añadir la frase ‘Este es el ejercicio 2’.
'''

archivo = open("ejercicio.txt", "w+")
content = archivo.write('Este es el ejercicio 2')
archivo.close()
```
{% endtab %}
{% endtabs %}

