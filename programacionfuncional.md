# Estructura 5: Programación Funcional y Expresiones Lambda en Java

## ¿Qué es la Programación Funcional?

La **programación funcional** es un paradigma de programación donde las funciones son tratadas como ciudadanos de primera clase. Esto significa que las funciones pueden ser asignadas a variables, pasadas como argumentos, o devueltas como resultados. En Java, la programación funcional se puede lograr mediante el uso de **expresiones lambda**, **interfaces funcionales** y otras características de la API de Java 8, como los flujos (`streams`).

## Expresiones Lambda

Una **expresión lambda** es una función sin nombre que puede ser tratada como una expresión. La sintaxis de las expresiones lambda en Java permite escribir código de manera más concisa y legible, especialmente cuando se trabaja con interfaces funcionales (interfaces que tienen un solo método).

### Sintaxis de una Expresión Lambda:

```java
(parameters) -> expression
```
- **parameters**: Parámetros que recibe la lambda (pueden ser varios o ninguno).

- **->**: Separador que indica que la expresión que sigue es el cuerpo de la función lambda.

- **expression**: El bloque de código que se ejecutará cuando se invoque la lambda.
import java.util.Arrays;
import java.util.List;
```java
public class Main { // Inicio de la clase Main
    public static void main(String[] args) { // Método main, punto de entrada del programa
        
        // Lista de números
        List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5);

        // Usando expresión lambda con forEach
        System.out.println("Imprimiendo los números:");
        numbers.forEach(number -> System.out.println(number));

        // Usando expresión lambda con map para duplicar los valores
        System.out.println("Números duplicados:");
        numbers.stream()
               .map(number -> number * 2)
               .forEach(number -> System.out.println(number));

        // Usando expresión lambda con filter para filtrar números mayores que 3
        System.out.println("Números mayores que 3:");
        numbers.stream()
               .filter(number -> number > 3)
               .forEach(number -> System.out.println(number));

    } // Fin del método main
} // Fin de la clase Main
```
# Declaración de la lista:

`numbers`: Es una lista de enteros que contiene los valores `{1, 2, 3, 4, 5}`.

# Uso de expresiones lambda:

## `forEach`: 

`numbers.forEach(number -> System.out.println(number));`: Esta expresión lambda toma cada elemento de la lista `numbers` y lo imprime. Es equivalente a un bucle `for` tradicional.

## `map`:

`numbers.stream().map(number -> number * 2)`: Esta expresión lambda toma cada número de la lista, lo multiplica por 2 y lo pasa al siguiente paso del flujo (`stream`). La operación `map` transforma los elementos de la lista original en una nueva lista con los números duplicados.

## `filter`:

`numbers.stream().filter(number -> number > 3)`: Esta expresión lambda filtra los elementos de la lista, devolviendo solo aquellos que son mayores que 3. En este caso, se filtran los números 4 y 5.

# Impresión de resultados:

`System.out.println()`: Se utiliza para imprimir los resultados de las transformaciones realizadas sobre la lista de números.

# ¿Por qué y para qué se utilizan las expresiones lambda?

* **Concisión**: Las expresiones lambda permiten escribir código de manera más compacta y legible, eliminando la necesidad de definir clases anónimas o implementaciones complejas para interfaces funcionales.
* **Legibilidad**: Son útiles para operaciones como iteración, filtrado, transformación, y reducción de colecciones, mejorando la claridad del código.
* **Programación Declarativa**: Permiten escribir código más declarativo y menos imperativo, especificando qué hacer en lugar de cómo hacerlo.

# Notas:

* **Interfaces Funcionales**: Son interfaces que contienen un solo método abstracto. Java 8 introdujo varias interfaces funcionales en el paquete `java.util.function`, como `Predicate`, `Function`, `Consumer`, etc. Las expresiones lambda se usan comúnmente con estas interfaces.
* **stream API**: La API de `stream` permite realizar operaciones de manera funcional sobre colecciones. Combina expresiones lambda con operaciones como `map`, `filter`, `reduce`, y `collect` para trabajar con datos de forma más eficiente y legible.

# ¿Cómo funciona la estructura?

En este ejemplo, utilizamos expresiones lambda junto con la API de `stream` de Java para realizar operaciones sobre una lista de números. La expresión lambda nos permite aplicar transformaciones a los elementos de la lista sin necesidad de escribir ciclos tradicionales. Las operaciones `forEach`, `map` y `filter` son ejemplos de cómo las expresiones lambda mejoran la legibilidad y eficiencia del código.

* `forEach` recorre cada elemento de la lista y lo imprime.
* `map` transforma los elementos, duplicándolos.
* `filter` selecciona solo los elementos que cumplen una condición (en este caso, aquellos mayores que 3).