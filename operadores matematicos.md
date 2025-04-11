# Estructura 2: Operadores Matemáticos en Java

## ¿Qué son los operadores matemáticos?
En programación, los **operadores matemáticos** se utilizan para realizar operaciones aritméticas sobre los valores de las variables. Los operadores matemáticos más comunes en Java incluyen:

- **+**: Suma. Realiza la adición de dos valores.
- **-**: Resta. Realiza la sustracción entre dos valores.
- **\***: Multiplicación. Realiza la multiplicación de dos valores.
- **/**: División. Realiza la división entre dos valores.
- **%**: Módulo. Devuelve el residuo de la división entre dos valores.)

## Ejemplo de Código en Java:

```java
public class Main { // Inicio de la clase Main
    public static void main(String[] args) { // Método main, punto de entrada del programa
        
        // Declaración de variables
        int num1 = 25; // Primer número entero
        int num2 = 5;  // Segundo número entero
        
        // Realización de operaciones matemáticas
        int suma = num1 + num2; // Suma de num1 y num2
        int resta = num1 - num2; // Resta de num1 y num2
        int multiplicacion = num1 * num2; // Multiplicación de num1 y num2
        int division = num1 / num2; // División de num1 entre num2
        int modulo = num1 % num2; // Módulo de num1 entre num2
        
        // Imprimir los resultados de las operaciones
        System.out.println("Suma: " + suma); // Imprime el resultado de la suma
        System.out.println("Resta: " + resta); // Imprime el resultado de la resta
        System.out.println("Multiplicación: " + multiplicacion); // Imprime el resultado de la multiplicación
        System.out.println("División: " + division); // Imprime el resultado de la división
        System.out.println("Módulo: " + modulo); // Imprime el residuo de la división
    } // Fin del método main
} // Fin de la clase Main
```
# Explicación paso a paso del código:

## Declaración de variables:

- `num1` y `num2` son variables de tipo `int` que almacenan los valores 25 y 5, respectivamente.

## Operaciones matemáticas:

- **Suma**: `int suma = num1 + num2;` realiza la suma de `num1` y `num2` (25 + 5 = 30).
- **Resta**: `int resta = num1 - num2;` realiza la resta entre `num1` y `num2` (25 - 5 = 20).
- **Multiplicación**: `int multiplicacion = num1 * num2;` realiza la multiplicación entre `num1` y `num2` (25 * 5 = 125).
- **División**: `int division = num1 / num2;` realiza la división entre `num1` y `num2` (25 / 5 = 5).
- **Módulo**: `int modulo = num1 % num2;` calcula el residuo de dividir `num1` entre `num2` (25 % 5 = 0).

## Impresión de resultados:

- Se utiliza `System.out.println()` para mostrar los resultados de las operaciones en la consola.

## ¿Por qué y para qué se utilizan estos operadores?

- Los operadores matemáticos permiten realizar cálculos dentro de un programa, lo que es fundamental para resolver problemas que requieran manipular valores numéricos.
- Los operadores de suma, resta, multiplicación y división son utilizados en la mayoría de las aplicaciones para realizar cálculos básicos.
- El operador módulo es útil cuando se necesita saber el residuo de una división, por ejemplo, para determinar si un número es divisible por otro o para realizar operaciones de ciclos o iteraciones.

## Notas:

- **División de enteros**: Si ambos números involucrados en la división son enteros, el resultado también será un entero. Si se desea obtener un resultado decimal, al menos uno de los números debe ser de tipo `float` o `double`.
- **Módulo**: El operador módulo (`%`) devuelve el residuo de la división. Esto es útil, por ejemplo, para determinar si un número es par (si el módulo de la división de un número por 2 es 0).




//Cómo funciona la estructura:

public class Main { // Definimos la clase Main, que contiene el código que se ejecutará en el programa.
    public static void main(String[] args) { // El método main es donde comienza la ejecución del programa.
        
        // Las variables num1 y num2 son declaradas con valores numéricos. Estas variables se usan luego en las operaciones matemáticas.
        
        // Las operaciones matemáticas son llevadas a cabo en las siguientes líneas, usando operadores matemáticos (+, -, *, /, %).
        
        // Los resultados de las operaciones se almacenan en nuevas variables (como suma, resta, multiplicación, etc.).
        
        // Finalmente, los resultados son mostrados en la consola utilizando System.out.println(), que imprime los valores de las variables.
    } // Fin del método main
} // Fin de la clase Main