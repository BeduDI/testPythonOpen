# Ejemplo

Existen diversas formas de abrir un fichero, la más común es utilizando la función open del **módulo io.**  
Abrimos nuestra terminal con Python, primero agregaremos el **módulo io** seguida por una variable texto que contenga dos líneas de texto.  
****

```coffeescript
from io import open

texto = "Una línea con texto\nOtra línea con texto"
```

![](https://lh4.googleusercontent.com/kfG-Q0EYd_aBSNquqBzkhZ7z2-GhSgahYI8OCgD-zdoYGkcMTzAZlNX5znwHMoRJ51PQR_V1wV06g_O00OOu_xR5B416yJVrgLFYJdvSAsA8j2Xe_NQAiu-YZ8MhmU8wVhwZwCAq)

A continuación debemos crear el fichero: ****

```coffeescript
fichero = open('fichero.txt','w')  
```

![](https://lh3.googleusercontent.com/oYnTssAt8tDLCwsgbcbzIR4mETl5F_wufoT3hLIPBC4dwCZlkRL0NRcwlscUMEm3C3Mh-rfP40Vql3RLISBNcPtvX_f_MCR0p7Lwp69ZanFwvemmV7fcR6mjKkFDAnnyRxJT_GA7)

> \*\*\*\*💡 **Nota:**
>
> La **w** indica escritura \(puntero al principio\)

Si revisamos la ruta en nuestra computadora donde estamos trabajando, observaremos que el **archivo fichero.text** fue creado con éxito

![](https://lh5.googleusercontent.com/Njupm_LCAF0t-7bSmzqX-iXs8tRL4gPMgICUHA8n02uHDPcPcsadajdzS_cxEC6EKmQotPvmtcHgfQGzSfvImaHJ1edk6O8iA2vSn8-cf1PXbWcIPUizUGkXc8RZCnqoRerm2R_K)

Procedemos a cerrar el fichero con **fichero.close\(\),** para realizar la lectura de nuestro archivo utilizaremos la siguiente línea:  

```coffeescript
fichero = open('fichero.txt','r')  
```

\*\*\*\*

> \*\*\*\*💡 **Nota:**
>
> La letra **r** indica que se trata de una acción de lectura, cargaremos el archivo con **.read\(\),** cerramos el archivo y después podremos imprimir el contenido del archivo.La letra **r** indica que se trata de una acción de lectura, cargaremos el archivo con **.read\(\),** cerramos el archivo y después podremos imprimir el contenido del archivo.  
> ****

```coffeescript
from io import open

fichero = open('fichero.txt','r')  
texto = fichero.read() 
fichero.close()  

print(texto)
```

![](https://lh6.googleusercontent.com/GSIOknu2XP7AvAfE324BZrEUJNwFgemLofGPnBEYrHpkiCKL2gPeqpdY33qDlH5fNwVka6gDM15YOp99lpwdqNhQmnyqzy0jHdtnyP0e-uGiysU12Ohx13zPaLfSr7YBD77nphOl)

Por medio del método **readlines\(\)** podemos generar una lista con las líneas:

```coffeescript
from io import open
fichero = open('fichero.txt','r')

#Creando una lista de líneas
texto = fichero.readlines()

fichero.close()
print(texto)
```

![](https://lh3.googleusercontent.com/naDeOx42W0r8s4x636MV7bJyzQ3vv6ivDUfxW0aJo0t2-xP0SupnE3aDc8CScmjLI2NeNsj4-PyUANC3F21_4AGXf155E2S9X-lGRaEE2ncudn5UcRNgAbU692Uljd0wcsCsa2OS)

También se puede leer un fichero utilizando la instrucción estándar **with** de la siguiente forma:

```coffeescript
with open("fichero.txt", "r") as fichero:
    for linea in fichero:
        print(linea)
```

![](https://lh6.googleusercontent.com/4L6SziDEDJxsEW4vFwUHIPVLQ04DZUNIG3yDLJyouewqWOhXXX5rUnkwXlKUUqhIBibLPUWjR9tJ-YET2oaQkBSunVOcDn9hJ1nJNv2yNSG2E5F5ge5BZNvuKnFq5e9dz1-ROOcc)

Es posible añadir datos a un fichero por medio de extensión, la cual indicaremos por medio de la **letra a**

```coffeescript
fichero = open('fichero.txt','a')  

fichero.write('\nOtra línea más abajo del todo')

fichero.close()
```

![](https://lh4.googleusercontent.com/ubCWCjuQNGlOQ1Erf0WR_Pfh14sHOWiKVhiQ7hikZJ6EC8PKuyQonR0L90u2BYLPI5iFtM-U_2wxeinDUH1ZiY6-eMCxZY1K8avIg4mIElMsAJUCnXtcMPcpzrW5iCh96OMb7VfZ)

En caso que el fichero no exista lo podemos crear por medio de la variante **a+**  


```coffeescript
fichero.close()
```

![](https://lh4.googleusercontent.com/RN5XoIZO6AJbO2lzEcWCSjTkcr9hq66w9Y3GE4ttuQXL1uTFA1pV6yBJlaC_vt1snUPxHlnltXBjWbwrfiZNn7o4Q9qMUcuSrfBU30o6jtr7NGZvMFFAVqKyLbSsLrntmhWIQ0qV)

![](https://lh6.googleusercontent.com/8NXSm8rxW4TvkldGJAvFU_H5cVDIysp6En3T9BVeJjg4acJOo5amBMDoy9zmdXT-u-lKJQYJeShQnCcXB9ZW8oc6FA9DM2eEUpeyAu_-j8kz9T_W77CZo64B36T9Neha3AOHX5bp)

Es posible posicionar el puntero en el fichero manualmente usando el método **seek** e indicando un número de caracteres para luego **leer** una cantidad de caracteres con el método **read:**

```coffeescript
fichero = open('fichero.txt','r')
fichero.seek(0)   # Puntero al principio
fichero.read(10)  # Leemos 10 caracteres
```

![](https://lh3.googleusercontent.com/Jvg8AwdhoAImMOihxREPCxJeeOEN1gFmizzNt1cmu9DbvaS21oulMz8DLSKMqVCmNi5pmb7FPL8mILyExcgwyQwpo95eDz2TgjaMUF8r0vhRjDu3HqnF9fvcuYj7m97kaw8cO6AF)

Para posicionar el puntero justo al inicio de la segunda línea, podríamos ponerlo justo en la longitud de la primera:  
****

```coffeescript
fichero = open('fichero.txt','r')
fichero.seek(0)

#Leemos la primera línea y situamos el puntero al principio de la segunda

fichero.seek( len(fichero.readline()) )

#Leemos todo lo que queda del puntero hasta el final

fichero.read()
```

![](https://lh4.googleusercontent.com/z8L6EPP9NgDFvBNsLBdd2CE1Wodt4uzLfzjqInqs334VKn2Lj8YvNHIS8lZgR1f6aCjJF9QSRybF1vGcd6-XTzszaPdQCKwsNbfsnf9XSZOYPqXy7TzcJ83hUcXRSFf8jqRy8OLx)

Se puede abrir un fichero en modo **lectura con escritura,** pero éste debe existir previamente.

Además por defecto el puntero estará al principio y si escribimos algo sobre escribiremos el contenido actual, así que debemos **tener cuidado.**  


```coffeescript
#Creamos un fichero de prueba con 4 líneas

fichero = open('fichero2.txt','w')
texto = "Línea 1\nLínea 2\nLínea 3\nLínea 4"
fichero.write(texto)
fichero.close()

#Lo abrimos en lectura con escritura y escribimos algo

fichero = open('fichero2.txt','r+')
fichero.write("0123456")

#Volvemos el puntero al inicio y leemos hasta el final

fichero.seek(0)
fichero.read()
fichero.close()
```

![](https://lh4.googleusercontent.com/FgrLexqTElNtlCqGMlA5H4a0Q-roz6kZ8dltrdxHEy9tK6xGwUCOncA8IddjtLORQkbt2pJmrN5N9VyD1gNNfWggPiCujWCLgisBnh7Xc-RYPDA-kBMuvFoF_ZiAZeARGtoxdUHt)

Es posible modificar una línea en específico, para lograr este fin lo mejor es leer todas las líneas en una lista, modificar la línea en la lista, posicionar el puntero al principio y reescribir de nuevo todas las líneas:

```coffeescript
fichero = open('fichero2.txt','r+')
texto = fichero.readlines()

#Modificamos la línea que queramos a partir del índice

texto[2] = "Esta es la línea 3 modificada\n"

#Volvemos el puntero al inicio y reescribimos

fichero.seek(0)
fichero.writelines(texto)
fichero.close()

#Leemos el fichero de nuevo

with open("fichero2.txt", "r") as fichero:
    print(fichero.read())


```

![](https://lh3.googleusercontent.com/iPwfCaME6g88NQ_DZ-3h3Nk-UZlRyXWwpbhy0r2WSDMggdNTNf_q73a1h7NDNjHf4Yf1wyIhVjXfxJXYwkeemp19le2gNKzPMWQqIBbux-mzECtsUSpl6ct4uxUKSYIs7XWa36k8)

En el archivo **ejemplosArchivos.py** encontraras el código completo de este ejemplo y podrás ejecutarlo copiandolo por partes o completo desde la terminal de python.  
****

**Ejercicios:**  


1. Realiza el código necesario para crear un fichero vacío llamado numeros.txt y después agregue una secuencia del 0 al 100.
2. Crear un programa que abra un fichero en modo lectura y escritura, si no existe lo creará, y añadir la frase ‘Este es el ejercicio 2’.

La solución a estos dos retos lo puedes encontrar en el archivo **solucionArchivos.py**   


