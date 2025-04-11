# Estructura 4: Loops y Bucles en Java

## ¿Qué son los Loops y Bucles?

En programación, un **bucle** o **loop** es una estructura que permite repetir un bloque de código varias veces de acuerdo con una condición. Los bucles son fundamentales para realizar tareas repetitivas sin tener que escribir el mismo código una y otra vez. En Java, existen diferentes tipos de bucles, como `for`, `while`, y `do-while`, que se utilizan dependiendo del tipo de tarea y la condición de repetición.

### Tipos comunes de bucles en Java:

- **Bucle `for`**: Se utiliza cuando se conoce de antemano el número de veces que se debe ejecutar un bloque de código.
  - Sintaxis: 
    ```java
    for (inicialización; condición; actualización) {
        // Bloque de código
    }
    ```
- **Bucle `while`**: Se ejecuta mientras se cumpla una condición determinada. Si la condición es falsa desde el inicio, el bucle no se ejecuta ni una sola vez.
  - Sintaxis:
    ```java
    while (condición) {
        // Bloque de código
    }
    ```
- **Bucle `do-while`**: Similar al `while`, pero la diferencia es que siempre ejecuta al menos una vez el bloque de código, ya que verifica la condición al final de la ejecución.
  - Sintaxis:
    ```java
    do {
        // Bloque de código
    } while (condición);
    ```

## Ejemplo de Código en Java:

```java
public class Main { // Inicio de la clase Main
    public static void main(String[] args) { // Método main, punto de entrada del programa
        
        // Uso de un bucle for para imprimir los primeros 5 números
        System.out.println("Contando hasta 5:");
        for (int i = 1; i <= 5; i++) {
            System.out.println(i);
        }

        // Uso de un bucle while para contar de 5 hacia abajo
        int number = 5;
        System.out.println("Contando hacia abajo desde 5:");
        while (number > 0) {
            System.out.println(number);
            number--;
        }

        // Uso de un bucle do-while para asegurarse de que se imprime al menos una vez
        System.out.println("Ejemplo de do-while:");
        int count = 1;
        do {
            System.out.println("Número " + count);
            count++;
        } while (count <= 3);

    } // Fin del método main
} // Fin de la clase Main
```
# Explicación paso a paso del código:

## Declaración de variables:

- **number**: Es una variable de tipo `int` que almacena el valor `5`. Se utiliza en el bucle `while` para contar hacia abajo.

- **count**: Es una variable de tipo `int` que almacena el valor `1`. Se utiliza en el bucle `do-while` para asegurarse de que se imprima al menos una vez.

## Uso de los bucles:

### Bucle `for`:
- El bucle `for` repite el bloque de código 5 veces, comenzando con `i = 1` y aumentando `i` hasta 5. En cada iteración, imprime el valor de `i`.

### Bucle `while`:
- El bucle `while` sigue ejecutando el bloque de código mientras que la condición `number > 0` sea verdadera. En cada iteración, imprime el valor de `number` y luego lo decrementa en 1 (`number--`). Cuando `number` llega a 0, la condición se vuelve falsa y el bucle termina.

### Bucle `do-while`:
- El bucle `do-while` garantiza que el bloque de código se ejecute al menos una vez, independientemente de si la condición es verdadera o falsa al principio. En este caso, imprimirá el número `1`, luego aumentará el contador `count` y continuará hasta que `count` sea mayor que 3.

## Impresión de resultados:

- Se utiliza `System.out.println()` para imprimir los valores dentro de los bucles.

## ¿Por qué y para qué se utilizan los bucles?

- **Bucle `for`**: Es útil cuando sabemos cuántas veces debemos repetir un bloque de código. Por ejemplo, al contar números o recorrer un conjunto de datos de longitud conocida.

- **Bucle `while`**: Es adecuado cuando no sabemos cuántas veces se debe ejecutar el bucle, pero sí sabemos cuál es la condición que debe cumplirse para que continúe ejecutándose.

- **Bucle `do-while`**: Es útil cuando necesitamos ejecutar un bloque de código al menos una vez, independientemente de la condición, y luego continuar repitiéndolo mientras se cumpla la condición.

## Notas:

- **Bucle `for`**: En el bucle `for`, la inicialización, la condición y la actualización están todas en una sola línea, lo que lo hace ideal cuando tenemos un rango fijo de valores que recorrer.

- **Bucle `while`**: El bucle `while` se ejecuta mientras la condición sea verdadera. Asegúrate de que la condición eventualmente se vuelva falsa para evitar un bucle infinito.

- **Bucle `do-while`**: Es una opción útil cuando necesitas ejecutar el código al menos una vez antes de comprobar la condición. Ten en cuenta que la condición se evalúa después de la ejecución del bloque de código.

## Cómo funciona la estructura:

En este ejemplo, los bucles se utilizan para repetir un bloque de código en función de una condición. El `for` se usa cuando sabemos cuántas repeticiones necesitamos. El `while` es útil cuando no sabemos cuántas repeticiones se requerirán, pero tenemos una condición que debe cumplirse para continuar ejecutando el bloque de código. Finalmente, el `do-while` garantiza que el código se ejecute al menos una vez, y luego verifica la condición al final.
