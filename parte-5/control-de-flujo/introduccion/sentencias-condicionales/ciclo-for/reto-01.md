# Reto 01

Abrimos nuestra terminal de Python y crearemos un ciclo for que nos permite iterar dentro de un rango, para la creación de rango utilizamos el método **range\(\),** en este ejemplo realizaremos un rango que vaya del número 1 al número 10, deberemos imprimir todos los números dentro del rango.

![](https://lh3.googleusercontent.com/kRtsbs_08h2dGDekRwl5ha7CBztZXCOI6GYnLGAe_sX21SvgY3RkTNT78AGZ1mjTerIc_NSj0b7xc-7nib_dCuqobWvB3o4phrqGrdykpThyuRE-FJhhc69ADH8qz7oUHrenfSmY)

Así como fue posible iterar dentro de una lista en el ejemplo del vídeo, también es posible iterar dentro de diccionarios, crearemos el siguiente diccionario**:**

```coffeescript
frutas = {'Fresa':'roja', 'Limon':'verde', 'Papaya':'naranja', 'Manzana':'amarilla', 'Guayaba':'rosa'}
```

**A continuación crearemos un programa que nos imprima la fruta y su color:**

```coffeescript
for nombre, color in frutas.items():
 print(nombre, "es de color", color)
```

![](https://lh4.googleusercontent.com/bHvxSg_WL8GSoi-D1BQw-YrCJTiAEsEoSry2hChAdoUlKnLr9HoUZ4-9HyX1JifX8y7n51DoEM1l355CbzxWlWuZY0nERNugL5g0YEnB9hiHcGAYXSygfUhq2vsUX-qycAJ_4Ph5)

> \*\*\*\*⚠ **Importante:**
>
> **Reto 1:** Realizar un programa similar a la **iteración** del diccionario, pero con la diferencia que deberá realizar la toma de valores por medio de la llave en lugar de **items\(\)**, en el archivo **ciclosSolución.py** encontraras una manera de realizarlo, sugerimos no consultar el documento hasta una vez realizado el ejercicio.
>
> **Reto2:** Utilizando el método **input\(\)**, crea un programa que solicite diversos números y los guarde en una lista, después deberá iterar sobre la lista de números y multiplicar su valor por sí mismo e imprimir el resultado de dicha multiplicación;por ejemplo **2 x 2 = 4 , 3 x 3 = 9.**
>
> En el archivo **ciclosSolución.py** encontraras una manera de realizarlo, sugerimos no consultar el documento hasta una vez realizado el ejercicio.
>
> ![](https://lh3.googleusercontent.com/-DS6K7Ok4pBueY6aIX0QV4p7EnxSz0y4kq1o9eItgh3yzh35NWxDZGTOaOLwU5CtkcQxJ7NrTLu_yYcBigXoYEWCKHuBB_ToP8z1oGiOel801zMiQwlFdphtc_lFyxolSfgsDj4q)

