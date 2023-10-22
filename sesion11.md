<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 11 

### Actividad

Basándose en el algoritmo 1 de la sesión 11, aplicar la siguiente variante: Dado un conjunto de números enteros, se debe determinar si existe algún número que aparezca más de una vez. Si es así, se deben imprimir todos los números que aparezcan más de una vez.

### Solución

    
Lo que hice fue en lugar de usar una única variable `numeroRepetido`, lo que hice fue utilizar una estructura de datos como un `HashSet` para rastrear los números repetidos. 

```java
import java.util.HashSet;

public class Ejercicio1 {

    public static void main(String[] args) {
        // Declaramos un conjunto de números enteros
        int[] numeros = {1, 2, 3, 4, 5, 2, 4};

        // Creamos un conjunto para almacenar los números que ya hemos visto
        HashSet<Integer> numerosVistos = new HashSet<>();
        
        // Creamos un conjunto para almacenar los números repetidos
        HashSet<Integer> numerosRepetidos = new HashSet<>();

        // Recorremos el conjunto de números
        for (int numero : numeros) {
            // Si el número ya ha sido visto, lo almacenamos como repetido
            if (numerosVistos.contains(numero)) {
                numerosRepetidos.add(numero);
            } else {
                // Si no hemos visto el número, lo agregamos al conjunto de números vistos.
                numerosVistos.add(numero);
            }
        }

        // Si hay números repetidos, los imprimimos
        if (!numerosRepetidos.isEmpty()) {
            System.out.println("Los números repetidos son:");
            for (int numero : numerosRepetidos) {
                System.out.println(numero);
            }
        } else {
            // No hay ningún número repetido
            System.out.println("No hay ningún número repetido");
        }
    }
}
```

Este programa modificado utiliza dos conjuntos: uno para rastrear los números que ya hemos visto (`numerosVistos`) y otro para rastrear los números repetidos (`numerosRepetidos`). Cuando se encuentra un número repetido, se agrega al conjunto `numerosRepetidos`. Al final del programa, se imprimen todos los números que aparecen más de una vez en el conjunto de números.

### Solución

```java
    import java.util.Scanner;

    public class BinarioADecimal {
      public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingresa un número binario: ");
        String numeroBinario = scanner.nextLine();

        int decimal = convertirBinarioADecimal(numeroBinario);

        System.out.println("El número decimal equivalente es: " + decimal);
      }

    public static int convertirBinarioADecimal(String numeroBinario) {
        int longitud = numeroBinario.length();
        int decimal = 0;

        for (int i = 0; i < longitud; i++) {
            char digito = numeroBinario.charAt(i);

            // Verificar si el dígito es '0' o '1'
            if (digito == '0') {
                // Si es '0', no se agrega nada al decimal en esta posición
            } else if (digito == '1') {
                // Si es '1', se agrega 2 elevado a la posición correspondiente al decimal
                decimal += Math.pow(2, longitud - 1 - i);
            } else {
                System.err.println("Número binario inválido. Debe contener solo 0 y 1.");
                System.exit(1);
            }
        }

        return decimal;
        }
    } 
    ```


Lo que hace este programa es solicitar al usuario que ingrese un número binario como una cadena de caracteres y luego utiliza una función llamada convertirBinarioADecimal para realizar la conversión. La función recorre cada dígito del número binario, verifica si es '0' o '1', y calcula el valor decimal correspondiente. El resultado decimal se muestra en la pantalla.
