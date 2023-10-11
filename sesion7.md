<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 


# Actividad: Ejecicios Array - ArrayList

1. En parejas, probar, analizar y explicar el funcionamiento de los siguientes ejemplos de Array y ArrayList.

### Ejemplo Array

    import java.util.Arrays;

    public class EjercicioArray {

        public static void main(String[] args) {
            // Crear un array de números enteros
            int[] numeros = {5, 2, 10, 7, 1};

            // Imprimir el array original
            System.out.println("Array original: " + Arrays.toString(numeros));

            // Calcular la suma de los elementos del array
            int suma = 0;
            for (int i = 0; i < numeros.length; i++) {
            suma += numeros[i];
            }
            System.out.println("La suma de los elementos es: " + suma);

            // Encontrar el número más grande en el array
            int maximo = numeros[0];
            for (int i = 1; i < numeros.length; i++) {
            if (numeros[i] > maximo) {
                maximo = numeros[i];
            }
            }
            System.out.println("El número más grande es: " + maximo);

            // Ordenar el array en orden ascendente
            Arrays.sort(numeros);
            System.out.println("Array ordenado: " + Arrays.toString(numeros));
        }
    }

### Ejemplo Array list

    import java.util.ArrayList; 
    import java.util.Scanner;

    public class AppNotas {

       public static void main(String[] args) {

         ArrayList<String> notas = new ArrayList<>();
    
         Scanner scan = new Scanner(System.in);

         while(true) {

          System.out.println("1. Agregar nota");  
          System.out.println("2. Mostrar notas");
          System.out.println("3. Salir");

          int opcion = scan.nextInt();

          if (opcion == 1) {
            agregarNota(notas, scan);  
          } else if (opcion == 2) {
            mostrarNotas(notas);
          } else {
            break;
          }

         }

       }   

       public static void agregarNota(ArrayList<String> notas, Scanner scan) {
    
          System.out.println("Ingrese el titulo de la nota:");
          String titulo = scan.nextLine();
    
          System.out.println("Ingrese el contenido de la nota:");
          String contenido = scan.nextLine();
    
         notas.add(titulo + " - " + contenido);

       }

       public static void mostrarNotas(ArrayList<String> notas) {

         for(String n : notas) {
         System.out.println(n);
         }

       }

    }


2. Crear un ejemplo de Array y otro de ArrayList para visualizar sus diferencias.
Previous.

## Solución

### Que es un Array.

Un array es una variable que almacena una lista de valores del mismo tipo.
El array se almacena en posiciones continuas de memoria y el acceso a los elementos se realiza
mediante índices, es usual en los programas la necesidad de almacenar una lista de valores para después
procesarlos. Una posibilidad es asociar a cada valor una variable, pero esto sería ineficiente y engorroso.

### Ejemplo de array

    import java.util.ArrayList; 
    import java.util.Scanner;
 
    public class ArrayDeNombres {

       public static void main(String arg[ ]) {

          String[ ] nombre = new String[4];

          nombre[0] = "Luis";
          nombre[1] = "María";
          nombre[2] = "Carlos";
          nombre[3] = "Jose";
          nombre[4] = "Ismael";   //Error:No existe esta variable array de índice 4

       }

    }


### Que es un Array list.

 es una clase que permite almacenar datos en memoria de forma similar a los Arrays, con la ventaja de que el numero de elementos que almacena, lo hace de forma dinámica, es decir, que no es necesario declarar su tamaño como pasa con los Arrays. Un ArrayList puede cambiar de tamaño segun se necesite en tiempo de ejecucion, la Clase ArrayList implementa la interfaz List.

### Ejemplo de array list
    
    import java.util.ArrayList; 
    import java.util.Scanner;

    public class Elementos {

       public static void main(String[] args) {

       // Declaración el ArrayList
       ArrayList<String> nombreArrayList = new ArrayList<String>();

       // Añadimos 10 Elementos en el ArrayList
       for (int i=1; i<=10; i++){
	     nombreArrayList.add("Elemento "+i);
       }

       // Añadimos un nuevo elemento al ArrayList en la posición 2
       nombreArrayList.add(2, "Elemento 3");

       // Declaramos el Iterador e imprimimos los Elementos del ArrayList
       Iterator<String> nombreIterator = nombreArrayList.iterator();
       while(nombreIterator.hasNext()){
	     String elemento = nombreIterator.next();
	     System.out.print(elemento+" / ");
       }

       }

    }








 


