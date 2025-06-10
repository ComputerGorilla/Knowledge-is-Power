# Plantillas de Cadenas (String Templates)

Es fundamental saber cómo **imprimir el contenido de las variables** en la salida estándar. Para ello, se utilizan **expresiones de plantilla** que permiten acceder a los datos almacenados en variables y otros objetos, y convertirlos en cadenas de texto.

Las variables declaradas directamente en el cuerpo principal del código se consideran **de nivel superior (top level)**.

### Reglas clave para la declaración de variables:

* Declara todas las variables como **solo lectura (`val`)** por defecto.
* Declara variables **mutables (`var`)** solo si es estrictamente necesario.

Las expresiones de plantilla siempre comienzan con un **signo de dólar (`$`)**. Si necesitas evaluar un fragmento de código dentro de una expresión de plantilla, coloca el código entre llaves, después del signo de dólar, así: **`${ tuCódigoAquí }`**.

### Ejemplo:

```kotlin
val clientes = 10
println("Hay $clientes clientes")   // Salida: Hay 10 clientes
println("Hay ${clientes + 1} clientes") // Salida: Hay 11 clientes
```

# BASIC TYPES:
#### +=, -=, *=, /=, and %=, are augmented assignment operators. For more information, see Augmented assignments.

**Ejemplo:**

```kotlin
var customers = 10

// Some customers leave the queue
customers = 8

customers = customers + 3 // Example of addition: 11
customers += 7            // Example of addition: 18
customers -= 3            // Example of subtraction: 15
customers *= 2            // Example of multiplication: 30
customers /= 3            // Example of division: 10

println(customers) // 10
```
![Tabla de types](Images\Types.png)