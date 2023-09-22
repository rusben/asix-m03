
# Introducción a Java

Java es un lenguaje de programación de alto nivel desarrollado por Sun Microsystems (ahora propiedad de Oracle). Se destaca por su portabilidad y versatilidad, lo que significa que los programas escritos en Java pueden ejecutarse en diferentes plataformas sin cambios significativos. Java se utiliza en una amplia variedad de aplicaciones, desde desarrollo web hasta aplicaciones de escritorio y aplicaciones móviles.

Algunas características clave de Java incluyen:

- **Orientación a objetos**: Java es un lenguaje de programación orientado a objetos, lo que significa que se organiza alrededor de objetos que encapsulan datos y funcionalidad.
- **Portabilidad**: Los programas Java se compilan en un formato intermedio llamado bytecode, que se ejecuta en la Máquina Virtual de Java (JVM). Esto permite que los programas Java sean independientes de la plataforma.
- **Seguridad**: Java incluye características de seguridad incorporadas, como la verificación de tipos y la gestión automática de la memoria, lo que ayuda a prevenir errores comunes de programación.
- **Multiplataforma**: Java se utiliza en una variedad de contextos, incluyendo desarrollo web (con Java EE), desarrollo de aplicaciones de escritorio (con Java SE) y desarrollo móvil (con Android, que utiliza una versión modificada de Java).
- **Gran comunidad y bibliotecas**: Java tiene una gran comunidad de desarrolladores y una amplia variedad de bibliotecas y frameworks disponibles que facilitan el desarrollo de aplicaciones.

## Método main en Java

El método main es el punto de entrada para la ejecución de programas Java. Es el método que se llama cuando ejecutas un programa Java y es obligatorio en cualquier clase que desees ejecutar. Aquí hay una explicación más detallada del método main:

```java
public class MiPrograma {
    public static void main(String[] args) {
        // Código de tu programa
    }
}
```

- `public`: Es un modificador de acceso que significa que el método main es accesible desde cualquier parte del programa.
- `static`: Indica que el método `main` pertenece a la clase en lugar de a una instancia específica de la clase.
- `void`: Indica que el método `main` no devuelve ningún valor.
- `main`: Es el nombre del método principal que se ejecutará cuando inicies tu programa.
- `String[] args`: Es un parámetro que recibe un array de cadenas de caracteres (String) llamado `args`. Este parámetro se utiliza para pasar argumentos desde la línea de comandos cuando ejecutas el programa.

El código dentro del método `main` es donde comienza la ejecución de tu programa Java. Puedes colocar instrucciones para realizar cualquier tarea que desees que realice tu programa. Por ejemplo, imprimir mensajes en la consola, calcular resultados, interactuar con el usuario, etc.

Cuando ejecutas un programa Java, el sistema invoca automáticamente el método main y ejecuta el código que contiene. Este es el punto de partida para la ejecución de tu programa.

## Ejecutar un programa desde la línea de comandos

Para ejecutar un programa en Java desde la línea de comandos, debes seguir estos pasos:

### Compila tu programa Java
Antes de poder ejecutar un programa Java, debes compilarlo para convertir el código fuente en bytecode, que es ejecutable por la Máquina Virtual Java (JVM). Utiliza el comando javac seguido del nombre de tu archivo Java. Por ejemplo:

```bash
javac MiPrograma.java
```

Esto generará un archivo `.class` en el mismo directorio que contiene el bytecode compilado.

### Ejecuta el programa Java
Una vez que hayas compilado tu programa, puedes ejecutarlo utilizando el comando java seguido del nombre de la clase principal (la clase que contiene el método main). Por ejemplo:

```bash
java MiPrograma
```

Si tu programa acepta argumentos de línea de comandos, puedes proporcionarlos después del nombre de la clase principal, separados por espacios. Por ejemplo:

```bash
java MiPrograma arg1 arg2
```

Donde `arg1` y `arg2` son argumentos que tu programa puede procesar en el método main.

### Ver la salida
Si tu programa produce alguna salida en la consola (por ejemplo, usando System.out.println()), verás los resultados en la ventana de la línea de comandos.

Un ejemplo completo podría ser:

Supongamos que tienes un archivo Java llamado "HelloWorld.java" con el siguiente contenido:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("¡Hello world!");
    }
}
```

Para compilar y ejecutar este programa, seguirías estos pasos:

```bash
javac MiPrograma.java  # Compila el programa
java MiPrograma        # Ejecuta el programa
```

La salida en la consola debería ser:

```bash
¡Hola, mundo!
```

Es importante asegurarse de estar en el directorio correcto (el directorio que contiene el archivo Java) cuando ejecutes estos comandos o proporcionar la ruta completa al archivo si no estás en el mismo directorio.

Recuerda que Java es sensible a mayúsculas y minúsculas, así que asegúrate de que el nombre del archivo y la clase coincidan exactamente, incluyendo mayúsculas y minúsculas.

## Literales y variables en Java

En Java, los literales y variables son elementos fundamentales para la programación. Los literales son valores constantes que se utilizan directamente en el código, mientras que las variables son nombres que se utilizan para almacenar y manipular datos. Aquí tienes información sobre ambos conceptos:

### Literales en Java

Los literales son valores constantes que se utilizan directamente en el código fuente. Los tipos de literales más comunes en Java son:

1. **Literales enteros**: Representan números enteros y pueden ser expresados en notación decimal, octal o hexadecimal.
- Decimal: Por defecto, los números enteros se expresan en base 10, como 42.
- Octal: Se representan con un 0 inicial, como 052 (equivalente a 42 en decimal).
- Hexadecimal: Se representan con un 0x inicial, como 0x2A (también equivalente a 42 en decimal).

2. **Literales de punto flotante**: Representan números decimales y pueden ser expresados en notación decimal o científica.
- Decimal: Por defecto, los números de punto flotante se expresan en decimal, como 3.14.
- Científica: Se utiliza la notación científica para representar números grandes o pequeños, como 2.5e-3 (equivalente a 0.0025).

3. **Literales de caracteres**: Representan un solo carácter y se escriben entre comillas simples, como 'A'.

4. **Literales de cadenas de caracteres**: Representan una secuencia de caracteres y se escriben entre comillas dobles, como "Hola, mundo!".

5. **Literales booleanos**: Representan valores booleanos true o false.

6. **Literales nulos**: Representan una referencia nula y se escriben como null.

### Variables en Java

Las variables en Java se utilizan para almacenar y manipular datos. Debes declarar una variable antes de usarla, especificando su tipo y nombre. Aquí hay algunos ejemplos de declaración de variables en Java:

```java
int numeroEntero = 42;         // Declaración de una variable entera
double numeroDecimal = 3.14;   // Declaración de una variable de punto flotante
char caracter = 'A';           // Declaración de una variable de carácter
String cadena = "Hola";        // Declaración de una variable de cadena de caracteres
boolean esVerdadero = true;    // Declaración de una variable booleana
```

Una vez que has declarado una variable, puedes asignarle un valor y utilizarla en tu programa. Por ejemplo:

```java
int x = 5;             // Asignar el valor 5 a la variable x
double precio = 19.99;  // Asignar el precio a la variable precio
String nombre = "Juan"; // Asignar un nombre a la variable nombre
```

Luego, puedes usar estas variables en expresiones y realizar operaciones con ellas en tu programa.

En resumen, los literales son valores constantes en Java, mientras que las variables son nombres que utilizas para almacenar y manipular datos en tu programa. La elección de literales o variables depende de tus necesidades y del flujo de tu programa.
