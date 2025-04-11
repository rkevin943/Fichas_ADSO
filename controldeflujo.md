# Estructura 4: Control de Flujo en Java

## ¿Qué es el Control de Flujo?

En programación, el **control de flujo** se refiere a la secuencia de ejecución de las instrucciones de un programa. El control de flujo determina cómo y cuándo se ejecutan ciertas partes del código. En Java, se utilizan estructuras de control como condicionales (`if`, `else`, `switch`) y bucles (`for`, `while`, `do-while`) para controlar el flujo de ejecución.

### Tipos comunes de estructuras de control de flujo:

- **Condicionales**: Permiten ejecutar diferentes bloques de código según ciertas condiciones.
  - `if`: Ejecuta un bloque de código si la condición es verdadera.
  - `else`: Ejecuta un bloque de código si la condición del `if` es falsa.
  - `else if`: Permite verificar múltiples condiciones.
  - `switch`: Selecciona uno de varios bloques de código dependiendo del valor de una variable.
  
- **Bucles**: Permiten repetir un bloque de código varias veces.
  - `for`: Repite un bloque de código un número específico de veces.
  - `while`: Repite un bloque de código mientras una condición sea verdadera.
  - `do-while`: Repite un bloque de código al menos una vez, y luego verifica la condición.

## Ejemplo de Código en Java:

```java
public class Main { // Inicio de la clase Main
    public static void main(String[] args) { // Método main, punto de entrada del programa
        
        // Declaración de variables
        int number = 5;

        // Uso de la estructura if-else para controlar el flujo
        if (number > 0) {
            System.out.println("El número es positivo");
        } else if (number < 0) {
            System.out.println("El número es negativo");
        } else {
            System.out.println("El número es cero");
        }

        // Uso de un bucle for para imprimir los primeros 5 números
        System.out.println("Contando hasta 5:");
        for (int i = 1; i <= 5; i++) {
            System.out.println(i);
        }

        // Uso de un bucle while para contar de 5 hacia abajo
        System.out.println("Contando hacia abajo desde 5:");
        while (number > 0) {
            System.out.println(number);
            number--;
        }

    } // Fin del método main
}``` // Fin de la clase Main

```
# Explicación paso a paso del código:

## Declaración de variables:

- **number**: Es una variable de tipo `int` que almacena el valor `5`. Es utilizada para evaluar las condiciones en los bloques `if` y en los bucles.

## Control de flujo con if-else:

- **Condicional if-else**: Verifica si `number` es mayor que 0, menor que 0 o igual a 0.
  - Si `number` es mayor que 0, imprime `"El número es positivo"`.
  - Si `number` es menor que 0, imprime `"El número es negativo"`.
  - Si `number` es igual a 0, imprime `"El número es cero"`.

## Control de flujo con bucles:

- **Bucle for**: Repite el bloque de código entre llaves 5 veces (desde `i = 1` hasta `i = 5`), imprimiendo los valores de `i` en cada iteración. Es útil cuando se sabe cuántas veces se debe repetir una acción.
- **Bucle while**: Repite el bloque de código mientras `number` sea mayor que 0. En cada iteración, se imprime el valor de `number` y se reduce en 1 (`number--`), hasta que `number` sea igual a 0.

## Impresión de resultados:

- Se utiliza `System.out.println()` para imprimir los resultados de las condiciones y los valores de las variables dentro de los bucles.

## ¿Por qué y para qué se utilizan estas estructuras de control?

- **Condicional if-else**: Se utiliza cuando se necesita tomar decisiones basadas en el valor de una condición. Es útil para ejecutar diferentes bloques de código dependiendo de si se cumplen o no ciertas condiciones.
- **Bucle for**: Es ideal cuando se conoce el número exacto de repeticiones que se deben hacer, como contar o iterar sobre un conjunto de elementos.
- **Bucle while**: Se utiliza cuando no se sabe cuántas veces se debe repetir el bloque de código, pero se tiene una condición que debe cumplirse para continuar la ejecución.

## Notas:

- **Condicionales**: El bloque `else if` se utiliza para verificar condiciones adicionales después de un `if` inicial. Si ninguna de las condiciones anteriores es verdadera, se ejecuta el bloque de código del `else`.
- **Bucles for y while**: Ambos tipos de bucles tienen su uso específico. El `for` es más adecuado cuando se tiene un rango conocido de valores, mientras que el `while` se usa cuando no se sabe cuántas veces se repetirá el ciclo, pero se necesita comprobar una condición en cada iteración.

## Cómo funciona la estructura:

En este ejemplo, se usan estructuras de control para evaluar condiciones y repetir bloques de código. La ejecución comienza con la evaluación de la condición `if-else`, y dependiendo de si la condición se cumple, se ejecuta el bloque correspondiente.

Los bucles repiten sus bloques de código un número de veces o mientras se cumpla una condición. Los bucles `for` se utilizan para repetir el código un número conocido de veces, mientras que el bucle `while` sigue ejecutándose mientras una condición sea verdadera.
