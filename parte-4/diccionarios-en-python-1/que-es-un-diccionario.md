# ¿Que es un diccionario?

Los‌ ‌diccionarios‌ ‌son‌ ‌una‌ ‌herramienta‌ ‌muy‌ ‌versátil.‌ ‌Se‌ ‌pueden‌ ‌utilizar‌ ‌un‌ ‌diccionario,‌ ‌para‌ ‌ contar‌ ‌cuántas‌ ‌apariciones‌ ‌de‌ ‌cada‌ ‌palabra‌ ‌hay‌ ‌en‌ ‌un‌ ‌texto,‌ ‌o‌ ‌cuántas‌ ‌apariciones‌ ‌de‌ ‌cada‌ ‌ letra.‌ ‌ ‌ 

Es‌ ‌posible‌ ‌utilizar‌ ‌un‌ ‌diccionario,‌ ‌parar‌ ‌**crear‌ ‌una‌ ‌agenda‌** ‌donde‌ ‌la‌ ‌clave‌ ‌es‌ ‌el‌ ‌nombre‌ ‌de‌ ‌la‌ ‌ persona,‌ ‌y‌ ‌el‌ ‌valor‌ ‌es‌ ‌una‌ ‌lista‌ ‌con‌ ‌los‌ ‌datos‌ ‌correspondientes‌ ‌a‌ ‌esa‌ ‌persona‌ ‌o‌ ‌en‌ ‌la‌ ‌ creación‌ ‌de‌ ‌listas‌ ‌de‌ ‌alumnos‌ ‌relacionados‌ ‌a‌ ‌sus‌ ‌materias.‌ ‌ ‌

Pero‌ ‌también‌ ‌los‌ ‌diccionarios‌ ‌son‌ ‌una‌ ‌de‌ ‌las‌ ‌estructuras‌ ‌de‌ ‌datos‌ ‌más‌ ‌destacadas‌ ‌de‌ ‌ Python.‌ ‌Ya‌ ‌que‌ ‌nos‌ ‌permiten‌ ‌trabajar‌ ‌aplicaciones‌ ‌como‌ ‌conjunto‌ ‌de‌ ‌datos‌ ‌para‌ ‌Machine‌ ‌ Learning‌

![](https://lh5.googleusercontent.com/uqYIdQ5YF_Fal33aYj2R2A0hfz-8CRjHt8cMVSAfZqd00_nANhb-wUmP92EZ_qkcKSBmFeDjZOYU_LDrikzitBD9P4_D3Z6o29ZVNNuRwG8t5ZJ0_K1WMXM-JNyeKVHADhXbzxhl)

Otros de los usos que se le pueden es para  crear bases de datos RDBM o NoSQL

![](https://lh6.googleusercontent.com/V2ISdXmGwUwFDZshNOKkT3lh9PLu1a_UoutBkkXglenx-HZmHW-XgGgSBdY2LTk-QKe449PfFgJfIwEkkCS3340aQqHQhT-yWljo4gLtPlpF-k5MRRJr-HSNEjatLoIHPJZ1347P)

### **Pero entonces ¿Qué es un diccionario en Python?**

La mejor manera de pensar en un diccionario es como un conjunto de datos desordenados con una clave que tienen como par un valor, uno de los requisitos principales de las claves es que deben ser únicas dentro del diccionario. 

La forma más común de trabajar diccionarios en python es con archivos JSON, pero ese será un tema a futuro.

**Ejemplo:** 

Diccionario que almacena la calificación de distintos dibujos animados.

| **Nombre de la caricatura** | **Puntuación** |
| :--- | :---: |
| Tom y Jerry | 9 |
| Scooby Doo | 9 |
| Jhonny Bravo | 8 |
| Dexter | 10 |

La representación de la tabla de arriba quedaría de la siguiente forma en un **diccionario en python** 

{% tabs %}
{% tab title="Python" %}
```python
Caricaturas = {'Tom y Jerry': 9, 'Scooby Doo': 9, 'Johnny Bravo': 8, 'Dexter': 10}
```
{% endtab %}
{% endtabs %}

\*\*\*\*

