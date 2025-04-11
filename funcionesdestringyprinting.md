# Estructura 3: Operaciones con Strings y Print en Java

## ¿Qué son los Strings?

En programación, **Strings** son secuencias de caracteres. En Java, los Strings se utilizan para almacenar texto, como nombres, frases, o cualquier otra secuencia de caracteres. Los Strings en Java son objetos de la clase `String` y se escriben entre comillas dobles (`" "`).

### Operaciones comunes con Strings:

- **Concatenación**: Unir dos o más Strings.
- **Longitud**: Obtener la cantidad de caracteres en un String.
- **Acceso a caracteres**: Obtener un carácter específico de un String en una posición determinada.
- **Conversión a mayúsculas y minúsculas**: Cambiar la caja de texto de los Strings.
- **Comparación**: Comparar dos Strings para ver si son iguales.

## Ejemplo de Código en Java:

```java
public class Main { // Inicio de la clase Main
    public static void main(String[] args) { // Método main, punto de entrada del programa
        
        // Declaración de variables tipo String
        String greeting = "Hola"; // String con valor "Hola"
        String name = "Juan"; // String con valor "Juan"
        String fullGreeting = greeting + " " + name + "!"; // Concatenación de Strings
        
        // Operaciones con Strings
        int length = fullGreeting.length(); // Longitud del String
        char firstLetter = fullGreeting.charAt(0); // Primer carácter del String
        String uppercaseGreeting = fullGreeting.toUpperCase(); // String en mayúsculas
        String lowercaseGreeting = fullGreeting.toLowerCase(); // String en minúsculas
        
        // Imprimir los resultados de las operaciones
        System.out.println("Saludo completo: " + fullGreeting); // Imprime la concatenación de Strings
        System.out.println("Longitud del saludo: " + length); // Imprime la longitud del saludo
        System.out.println("Primer letra del saludo: " + firstLetter); // Imprime la primera letra del saludo
        System.out.println("Saludo en mayúsculas: " + uppercaseGreeting); // Imprime el saludo en mayúsculas
        System.out.println("Saludo en minúsculas: " + lowercaseGreeting); // Imprime el saludo en minúsculas
    } // Fin del método main
} // Fin de la clase Main

```
# Explicación paso a paso del código:

## Declaración de Strings:

- `greeting` y `name` son variables de tipo `String` que almacenan las palabras `"Hola"` y `"Juan"`, respectivamente.
- `fullGreeting` es el resultado de concatenar los Strings `greeting` y `name` usando el operador `$+`. Esto produce el saludo completo: `"Hola Juan!"`.

## Operaciones con Strings:

- **Concatenación**: `"Hola" $+ " " $+ "Juan"` resulta en `"Hola Juan!"`.
- **Longitud**: `fullGreeting.length()` devuelve la cantidad de caracteres en la cadena (en este caso, 10).
- **Acceso a caracteres**: `fullGreeting.charAt(0)` devuelve el primer carácter de la cadena, que es `'H'`.
- **Conversión a mayúsculas**: `fullGreeting.toUpperCase()` convierte todo el texto a mayúsculas: `"HOLA JUAN!"`.
- **Conversión a minúsculas**: `fullGreeting.toLowerCase()` convierte todo el texto a minúsculas: `"hola juan!"`.

## Impresión de resultados:

- Se utiliza `System.out.println()` para imprimir en consola el resultado de cada operación.

## ¿Por qué y para qué se utilizan estas operaciones con Strings?

- **Concatenación**: Permite combinar varias cadenas de texto en una sola. Esto es útil cuando se necesita formar frases o mensajes dinámicamente.
- **Longitud**: Es útil cuando se necesita saber cuántos caracteres tiene un `String`, por ejemplo, para verificar que un texto no sea demasiado largo o corto.
- **Acceso a caracteres**: Permite acceder a un carácter específico de una cadena. Esto es útil cuando se quiere analizar o modificar un texto a nivel de sus caracteres.
- **Conversión de mayúsculas y minúsculas**: Se utiliza cuando se necesita normalizar el texto, por ejemplo, para hacer comparaciones que no distinguen entre mayúsculas y minúsculas.
- **Impresión (Printing)**: La impresión es fundamental para mostrar resultados al usuario, como mensajes, resultados de cálculos o cualquier otra información que el programa necesite comunicar.

## Notas:

- **Concatenación**: Es posible concatenar más de dos cadenas con el operador `$+`. También se puede usar el método `$concat()`, aunque el operador `$+` es más común.
- **Comparación de Strings**: Si deseas comparar dos `Strings` en Java, no debes usar el operador `==`, ya que esto compara las direcciones de memoria, no el contenido. En su lugar, debes usar el método `.equals()`.

public class Main { // La clase Main es el punto de entrada del programa en Java, donde se ejecuta el código.
    public static void main(String[] args) { // El método main es el inicio de la ejecución del programa.
        
        // En este bloque, definimos los Strings y realizamos operaciones como concatenación, longitud, acceso a caracteres, y conversiones de mayúsculas y minúsculas.
        
        // Concatenamos Strings usando el operador +, lo que nos permite construir un mensaje dinámicamente.
        
        // Posteriormente, se realizan las operaciones sobre el String y los resultados se almacenan en nuevas variables.
        
        // Finalmente, los resultados de esas operaciones son impresos en la consola para mostrar al usuario los resultados.
    } // Fin del método main
} // Fin de la clase Main