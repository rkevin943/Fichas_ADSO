# Estructura 1: Manejo de Variables en Java

## ¿Qué son las variables?

// En programación, las variables son fundamentales para almacenar datos que se pueden utilizar durante la ejecución de un programa. Las variables pueden almacenar distintos tipos de información como texto, números enteros, decimales, caracteres individuales, etc. En Java, los tipos de datos más comunes son:

- **String**: Almacena cadenas de texto (como nombres, frases, etc.). Los valores se escriben entre comillas dobles (`" "`).
- **int**: Almacena números enteros (sin decimales), como 123 o -123.
- **float**: Almacena números decimales, pero con precisión limitada (por ejemplo, 19.99 o -19.99). Es importante recordar que se debe agregar la `f` al final del valor decimal para especificar que es un número de tipo `float`.
- **double**: Similar a `float`, pero con mayor precisión. Ideal para cálculos más complejos que requieran decimales.
- **char**: Almacena un solo carácter. Los valores de tipo `char` se escriben entre comillas simples (`' '`).
- **boolean**: Almacena valores de **verdadero** o **falso**.

## Ejemplo de Código en Java:

```java
public class Main {
    public static void main(String[] args) {
        // Declaración de variables de distintos tipos
        String studentName = "John Doe"; // Variable de tipo String
        int studentID = 15;              // Variable de tipo int
        int studentAge = 23;             // Variable de tipo int
        float studentFee = 75.25f;       // Variable de tipo float (nota: f al final)
        double studentDouble = 75.24;    // Variable de tipo double
        char studentGrade = 'B';         // Variable de tipo char
        
        // Imprimir los valores de las variables
        System.out.println("Student name: " + studentName);
        System.out.println("Student id: " + studentID);
        System.out.println("Student age: " + studentAge);
        System.out.println("Student fee: " + studentFee);
        System.out.println("Student double: " + studentDouble);
        System.out.println("Student grade: " + studentGrade);
    }
}

```
# Explicación paso a paso del código

## Definición de variables:

- **String**: `studentName` almacena el nombre del estudiante. `"John Doe"` es un valor de tipo cadena.
- **int**: `studentID` y `studentAge` almacenan el ID y la edad del estudiante, respectivamente, ambos valores enteros.
- **float**: `studentFee` almacena el costo de la matrícula o tarifa, con decimales. Se coloca una `f` al final del valor para indicar que es un `float`.
- **double**: `studentDouble` es una variable para almacenar un valor decimal de doble precisión, ideal para cálculos más detallados.
- **char**: `studentGrade` almacena el carácter que representa la calificación del estudiante (en este caso, `'B'`).

## Impresión de los valores:

Se usan las instrucciones `System.out.println()` para mostrar en pantalla el valor de cada variable.

## ¿Por qué y para qué se utilizan estas variables?

- Las **variables** son esenciales para guardar y manipular datos en un programa. Permiten que el programa trabaje con valores que cambian durante la ejecución.
- Dependiendo del tipo de dato, las variables permiten realizar operaciones matemáticas, manipular texto, o guardar estados lógicos (como `true` o `false` en el caso de un booleano).
- **String** es útil para mostrar mensajes o nombres.
- **int** y **float** se usan para cálculos con números enteros o decimales.
- **char** se usa cuando se necesita almacenar un solo carácter, como una letra o un símbolo.
- **boolean** es útil cuando se necesita representar condiciones binarias, como si una condición es verdadera o falsa.

## Notas:

- El tipo **float** debe tener una `f` al final para diferenciarlo de un **double**, que es el tipo por defecto para números decimales en Java.
- Se puede usar **double** para obtener mayor precisión en cálculos que involucran decimales.

## Cómo funciona la estructura:

En este código de ejemplo, cada línea de declaración de variable está asignando un valor a una variable en particular. Estas variables son luego utilizadas en las instrucciones de salida, que son las que muestran el valor en consola. Los tipos de datos aseguran que las variables manejen correctamente los valores que se les asignan, ya sean cadenas de texto, números enteros o decimales.

Este proceso permite que el programa sea flexible y que los valores de las variables puedan cambiar dinámicamente, haciendo que el código sea reutilizable y adaptable a distintos escenarios.
```java
public class Main { // Inicio de la clase Main
    public static void main(String[] args) { // Método main, punto de entrada del programa
        
        // Declaración de variables de distintos tipos
        String studentName = "John Doe"; // Variable de tipo String
        int studentID = 15;              // Variable de tipo int
        int studentAge = 23;             // Variable de tipo int
        float studentFee = 75.25f;       // Variable de tipo float (nota: f al final)
        double studentDouble = 75.24;    // Variable de tipo double
        char studentGrade = 'B';         // Variable de tipo char
        
        // Imprimir los valores de las variables
        System.out.println("Student name: " + studentName); // Imprime el nombre del estudiante
        System.out.println("Student id: " + studentID); // Imprime el ID del estudiante
        System.out.println("Student age: " + studentAge); // Imprime la edad del estudiante
        System.out.println("Student fee: " + studentFee); // Imprime la tarifa del estudiante
        System.out.println("Student double: " + studentDouble); // Imprime el valor decimal
        System.out.println("Student grade: " + studentGrade); // Imprime la calificación del estudiante
    } // Fin del método main
} // Fin de la clase Main