# Tipos de datos y variables

###  **Variables y Tipos de datos en Python** <a id="variables-y-tipos-de-datos-en-python"></a>

Todos los valores en Python son objetos y cada objeto tiene **un tipo.**‌

Cada tipo de objeto determina qué operaciones es posible realizar con dicho objeto y por lo tanto que operaciones soporta, sus atributos y si puede ser o no mutable.‌

### **Datos Primitivos** <a id="datos-primitivos"></a>

‌**Tipo de datos Numéricos**

Python soporta datos con **valores enteros, números de punto flotante \(con decimales\) y números complejos.**‌

Todos los números en Python son objetos inmutables, esto quiere decir que siempre que se realice una operación con un número el resultado será otro objeto de tipo **número.**‌

**Los tipos numéricos de python soportados son los siguientes:**

| **Nombre del Tipo de Dato** | **Tipo de Dato** | Ejemplo |
| :--- | :--- | :--- |
| Decimales | **int** | **5** |
| Flotantes | **Float** | **5.0** |
| Complejos | **int** | **5j** |

### **Tipo de datos Strings** <a id="tipo-de-datos-strings"></a>

Un **objeto string \(simple o Unicode\)** es una secuencia de caracteres utilizado para guardar y representar textos. Los **strings** en **Python** son **inmutables.**‌

**Ejemplo de un String:** **`'Hola Mundo'`**‌

**Tipo de datos booleanos** El tipo **booleano** sólo puede tener **dos valores: True \(verdadero\) y False \(falso\).** Estos valores son especialmente importantes para las expresiones condicionales y los bucles, como verá más adelante.

| ​Definición | Tipo de Datos |
| :--- | :---: |
| Valor booleano falso | **False** |
| Valor booleano verdadero | **True** |

‌**Datos Complejos Tipo de datos Listas**

* Una lista es una secuencia ordenada de elementos mutable. **\(Lo que significa que puede cambiar de tipo\)**
* Los elementos de una lista pueden ser objetos de **distintos tipos.**
* Los elementos de una lista se indican **separados por comas en el interior de corchetes.**
* Se puede crear una lista vacía utilizando **dos corchetes vacíos**‌

**A continuación podrás encontrar algunos ejemplos de listas:**

| ​Tipo de lista | ​Definición |
| :--- | :--- |
| **\[42, 3.14, 'hola mundo'\]** | Lista con tres elementos |
| **\[100\]** | Lista con un elemento |
| **\[ \]** | Lista vacía |

**Tipo de datos Tuplas**‌

* Una **tupla** es una secuencia de elementos ordenada e inmutable**.**
* Los **elementos de una tupla** pueden ser objetos de cualquier tipo**.**
* Para **especificar una tupla,** lo hacemos con los elementos separados por comas dentro de paréntesis.
* Se puede **crear una tupla vacía** utilizando dos paréntesis vacíos.

| ​**Tipo de datos Tuplas**‌ | ​Definición |
| :--- | :--- |
| **\(100, 200, 300\)** | Tupla con tres elementos |
| **\(100,\)** | Tupla con un elemento |
| **\( \)** | Tupla vacía |

‌**Tipo de datos Diccionarios**

Los diccionarios de Python son una **lista** de los cuales se proporcionan valores asociados y se definen por corchetes.‌

En Python, un diccionario es una **colección no-ordenada de valores q**ue son accedidos a través de una llave. Es decir, en lugar de acceder a la información mediante el índice numérico, como es el caso de las listas y tuplas, es posible acceder a los valores a través de sus llaves, que pueden ser de diversos tipo.‌

Las **llaves** son únicas dentro de un diccionario, es decir que no puede haber un diccionario que tenga dos veces la misma llave, si se asigna un valor a una llave ya existente, se reemplaza el valor anterior.‌

No hay una forma directa de acceder a una llave a través de su valor, y nada impide que un mismo valor se encuentre asignado a distintas llaves. **Para separar la llave de su valor se utilizan dos puntos.**‌

**A continuación podrá visualizar un ejemplo de un diccionario:**‌

**`{"two": "dos", "one": "uno"}`**

| **Llave** | **Valor** |
| :--- | :--- |
| **two** | dos |
| **one** | uno |

### **Tipo de datos Conjuntos** <a id="tipo-de-datos-conjuntos"></a>

**Un conjunto,** es una colección no ordenada y sin elementos repetidos. Los usos básicos de éstos incluyen verificación de pertenencia y eliminación de entradas duplicadas.

| **Clase** | **Tipo de dato** | **Descripción** | **Ejemplo** |
| :--- | :--- | :--- | :--- |
| **set** | Conjuntos | Mutable, sin orden, no contiene duplicados | set\(\[4.0, 'Auto', True\]\) |
| **frozenset** | Conjuntos | Inmutable, sin orden, no contiene duplicados. | frozenset\(\[4.0, 'Auto', True\] |

‌**Variables en Python**‌

**Una variable** es un espacio de memoria donde guardamos una determinada información. En Python las variables tendrán distintas funciones de acuerdo al tipo de dato que asignemos a ellas.‌

Cada variable tiene que tener un nombre con el que referirnos a ella. Python tiene en cuenta si escribimos en **mayúsculas** o **minúsculas la variable** \(lo que se conoce como case **sensitive**\). No es lo mismo una variable que se llame **V1** que una que se llame **v1**.‌

Como es lógico y, para evitar confusiones, el nombre de la variable **no puede coincidir con los nombres de los** **comandos de python** \(**if, for**, etc.\). Tampoco podremos usar nombres de variables con **tildes o con ñ**.‌

Para asignar un valor a una variable usaremos el signo de **igual**.‌

**A continuación se listan algunos ejemplos de variables de distintos tipos de datos.**

| **​Variable** | ​Tipo |
| :--- | :--- |
| **x = 5** | Decimal |
| **x = 5.0** | Flotante |
| **x = 5j** | Complejo |
| **x = False** | Booleano |
| **x = True** | Booleano |
| **x = \[42, 3.14, 'hola mundo'\]** | Lista |
| **x = \(100, 200, 300\)** | Tupla |
| **x = {"two": "dos", "one": "uno"}** | Diccionario |
| **x = set\(\[4.0, 'Auto', True\]\)** | Conjunto |

‌Después haber visto el vídeo y analizado la información anterior, **es momento de ponerlo en práctica.**

