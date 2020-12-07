# Sentencias condicionales

### Sentencias condicionales

**Python** al igual que otros lenguajes de programación cuenta con diversos mecanismos de control de flujo, en esta ocasión trabajaremos con las sentencia `if` y `else`:

La sentencia `IF` requiere de una condición a evaluar, esta expresión será evaluada como expresión **Boolean** teniendo como resultado true o false. Si la condición evaluada es verdadera, se ejecutará la `sentencia_1`, en caso contrario se ejecuta la `setencia_2`.

{% tabs %}
{% tab title="Python" %}
```python
if (condición)
	sentencia1
else
    sentencia_2
```
{% endtab %}
{% endtabs %}

A diferencia de lenguajes como JavaScript que hacen uso de corchetes para delimitar la sentencia en Python debemos hacer uso de la identación, la **identación** es el espacio dejado detrás de otro comando ya que limita las instrucciones; en el siguiente ejemplo podrás identificar de color rojo la indentación en Python se recomienda una indentación de 4 espacios.

{% tabs %}
{% tab title="Python" %}
```python
if edad >= 18:
>>>>print('Eres mayor de edad')
```
{% endtab %}
{% endtabs %}

**En el uso de sentencias podemos hacer uso de operadores de comparación:**

| **Operadores de Comparación** | Definición |
| :--- | :--- |
| `Equal (==)` | **Regresa verdadero si ambos valores son iguales** |
| `Not equal (!=)` | **Regresa verdadero si ambos valores son diferentes** |
| `Mayor que (>)` | **Regresa verdadero si el valor de lado izquierdo es mayor al valor de lado derecho** |
| `Mayor o igual que (>=)` | **Regresa verdadero si el valor de lado izquierdo es mayor o igual al valor de lado derecho** |
| `Menor que (<)` | **Regresa verdadero si el valor de lado izquierdo es menor al valor de lado derecho** |
| Menor o igual que \(&lt;=\) | **Regresa verdadero si el valor de lado izquierdo es menor o igual al valor de lado derecho** |

