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












