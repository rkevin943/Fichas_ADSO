# Estructura 5: Collections, JSON y Manejo de Datos en Java

## ¿Qué son las Collections y cómo se usan en Java?

En Java, las **Collections** son estructuras de datos que permiten almacenar y manipular grupos de objetos de manera eficiente. Existen varios tipos de colecciones que ofrecen diferentes características y usos, como listas, conjuntos y mapas.

### Tipos comunes de colecciones en Java:

- **Listas (List)**: Permiten almacenar elementos en un orden determinado, con posibilidad de duplicados. Ejemplo: `ArrayList`.
- **Conjuntos (Set)**: Almacenan elementos de manera única, sin permitir duplicados. Ejemplo: `HashSet`.
- **Mapas (Map)**: Almacenan pares de clave-valor, permitiendo acceder a un valor mediante una clave única. Ejemplo: `HashMap`.

## ¿Qué es JSON y cómo se maneja en Java?

El **JSON (JavaScript Object Notation)** es un formato de intercambio de datos basado en texto, utilizado para almacenar y transferir datos estructurados. En Java, se puede trabajar con JSON utilizando bibliotecas como **Jackson** o **Gson**.

### Manejo de JSON con Jackson en Java:

Jackson es una biblioteca popular para convertir objetos Java a JSON y viceversa. Se usa ampliamente para manejar datos JSON de forma eficiente.

## Ejemplo de Código en Java:


```java
import com.fasterxml.jackson.databind.ObjectMapper; // Importar Jackson

import java.util.*; // Importar colecciones

public class Main { // Inicio de la clase Main
    public static void main(String[] args) throws Exception { // Método main, punto de entrada del programa
        
        // Uso de Collections en Java:
        
        // Creación de una lista (ArrayList)
        List<String> fruits = new ArrayList<>();
        fruits.add("Manzana");
        fruits.add("Banana");
        fruits.add("Cereza");
        
        // Imprimir los elementos de la lista
        System.out.println("Frutas: " + fruits);
        
        // Creación de un conjunto (HashSet)
        Set<String> uniqueFruits = new HashSet<>();
        uniqueFruits.add("Manzana");
        uniqueFruits.add("Banana");
        uniqueFruits.add("Banana"); // Duplicado que no será agregado
        
        // Imprimir el conjunto (no permite duplicados)
        System.out.println("Frutas únicas: " + uniqueFruits);
        
        // Creación de un mapa (HashMap)
        Map<String, Integer> fruitPrices = new HashMap<>();
        fruitPrices.put("Manzana", 2);
        fruitPrices.put("Banana", 1);
        fruitPrices.put("Cereza", 3);
        
        // Imprimir los precios de las frutas
        System.out.println("Precios de frutas: " + fruitPrices);

        // Manejo de JSON con Jackson:

        // Crear un objeto para convertir a JSON
        Map<String, String> person = new HashMap<>();
        person.put("nombre", "Juan");
        person.put("apellido", "Pérez");
        person.put("edad", "30");
        
        // Crear un ObjectMapper para convertir a JSON
        ObjectMapper objectMapper = new ObjectMapper(); 
        
        // Convertir el objeto en JSON
        String jsonString = objectMapper.writeValueAsString(person);
        System.out.println("Objeto convertido a JSON: " + jsonString);
        
        // Convertir de JSON a un objeto
        String jsonInput = "{\"nombre\":\"Ana\",\"apellido\":\"Gómez\",\"edad\":\"25\"}";
        Map<String, String> personFromJson = objectMapper.readValue(jsonInput, Map.class);
        System.out.println("Objeto deserializado desde JSON: " + personFromJson);

    } // Fin del método main
} // Fin de la clase Main 
```
# Explicación paso a paso del código:

## Declaración de variables:

- **List<String> fruits**: Es una variable de tipo `List`, específicamente un `ArrayList` que almacena una lista de frutas. Es utilizada para almacenar elementos en un orden determinado y permite duplicados.

- **Set<String> uniqueFruits**: Es una variable de tipo `Set`, específicamente un `HashSet`, que almacena frutas únicas, es decir, no permite duplicados.

- **Map<String, Integer> fruitPrices**: Es una variable de tipo `Map`, específicamente un `HashMap`, que almacena los precios de frutas utilizando un par clave-valor.

## Uso de Collections en Java:

- **Lista (ArrayList)**: Permite almacenar elementos de tipo `String` en un orden específico. En este ejemplo, se agregan frutas a la lista, y se imprime la lista completa.

- **Conjunto (HashSet)**: Permite almacenar elementos únicos. Aunque se intente agregar un duplicado (la banana), no se agrega debido a la propiedad del conjunto.

- **Mapa (HashMap)**: Almacena pares de clave-valor, donde la clave es el nombre de la fruta y el valor es su precio. Los elementos del mapa se imprimen de acuerdo con sus claves.

## Manejo de JSON con Jackson:

- **Conversión de objeto a JSON**: Se utiliza el `ObjectMapper` de Jackson para convertir un mapa (`person`) a un `String` en formato JSON. Esto es útil para enviar datos entre sistemas o almacenar datos en un archivo JSON.

- **Conversión de JSON a objeto**: A continuación, se toma un `String` en formato JSON y se deserializa de nuevo a un `Map<String, String>`. Esto permite reconstruir un objeto Java a partir de un formato JSON recibido.

## Impresión de resultados:

Se utiliza `System.out.println()` para imprimir los resultados de las colecciones y la conversión entre objetos Java y JSON.

## ¿Por qué y para qué se utilizan estas estructuras y técnicas?

- **Collections**: Las colecciones son esenciales cuando se necesita almacenar y manipular datos de manera flexible. Las listas son ideales para mantener el orden, los conjuntos son útiles cuando no se deben permitir duplicados, y los mapas permiten asociar claves con valores, lo que es muy útil para representar datos relacionados.

- **JSON**: El formato JSON es ampliamente utilizado para el intercambio de datos entre aplicaciones. Convertir objetos Java a JSON y viceversa permite interactuar con APIs, bases de datos, o archivos de configuración de manera eficiente.

## Notas:

- **Collections**: Las colecciones como `List`, `Set` y `Map` tienen métodos específicos para agregar, eliminar y buscar elementos. El uso de las colecciones depende de las necesidades del programa, como si es necesario mantener el orden de los elementos o evitar duplicados.

- **JSON y Jackson**: Jackson es una biblioteca poderosa para trabajar con JSON. Permite convertir fácilmente entre objetos Java y JSON, lo que es útil en la mayoría de las aplicaciones modernas que interactúan con servicios web o almacenan configuraciones en formato JSON.

## Cómo funciona la estructura:

En este ejemplo, las colecciones se utilizan para almacenar y manipular datos de forma eficiente. El uso de un `ArrayList`, un `HashSet`, y un `HashMap` demuestra cómo se pueden organizar datos y realizar operaciones sobre ellos.

La conversión entre objetos Java y JSON facilita la interacción con otros sistemas y servicios, asegurando que los datos se puedan transferir de manera fácil y estandarizada. La ejecución de este código muestra cómo trabajar con estructuras de datos fundamentales en Java y cómo utilizar Jackson para manejar JSON.
