<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


Actividad: Diseñar un formulario de pedido de un producto
Objetivo:

Aplicar los conocimientos sobre los tipos de etiquetas HTML para diseñar un formulario de pedido de un producto.

Instrucciones:

Crear un nuevo documento HTML.
Crear un formulario con los siguientes campos:
Nombre del producto
Cantidad
Precio unitario
Precio total
Dirección de envío
Información de contacto (nombre, correo electrónico, número de teléfono)
Agregar los siguientes campos relacionados al formulario:
Método de pago
Fecha de entrega
Comentarios
Utilizar las etiquetas HTML apropiados para cada campo.



### Solución

```java
     import java.util.Scanner;

     public class SESION5 {
    
         public static void main (String [] args){
            int Multiplicando ;
     
            System.out.println("¿Que tabla desea Realizar?");
            Scanner valor1 = new Scanner(System.in);
            Multiplicando = valor1.nextInt();

            int multiplicador = 1;
            while(multiplicador <=5){
            System.out.println(Multiplicando + " X " + multiplicador + " = " + Multiplicando * multiplicador );
            multiplicador++;
    
            }
        } 
    }

2. Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

### Solución 

     import java.util.Scanner;

     public class ContarNumeros {
         public static void main(String[] args) {
         Scanner sc = new Scanner(System.in);
         System.out.print("Ingrese una cadena de caracteres: ");
         String cadena = sc.nextLine();

         int i = 0;
         int contadorNumeros = 0;

         while (i < cadena.length()) {
         char caracter = cadena.charAt(i);
         if (caracter == '1' || caracter == '2' || caracter == '3' || caracter == '4' || caracter == '5' ||
         caracter == 'a' || caracter == 'c' || caracter == 'f' || caracter == 'x' || caracter == 'r') {
         contadorNumeros++;
         }
            i++;
         }

         System.out.println("La cadena ingresada contiene " + contadorNumeros + " Numeros.");
         }
     }

### Ejercicios - do while

1. Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.

### Solución 

     import java.util.Scanner;

     public class Main {
         public static void main(String[] args) {
         Scanner entradaDatos = new Scanner(System.in);
         int i = 1;     
         System.out.println("Ingresa un numero:");
         int numero =entradaDatos.nextInt();
         do {System.out.println(i);
         i++;         
         } while(i<=100 && numero >=0 ); 
         }
     }

3. Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

### Solución

     import java.util.Scanner;

     public class SESION5 {
    
         public static void main (String [] args){
         int Multiplicando ;
     
         System.out.println("¿Que tabla desea Realizar?");
         Scanner valor1 = new Scanner(System.in);
         Multiplicando = valor1.nextInt();

         int multiplicador = 1;
         do {
         System.out.println(num + " X " + multiplicador + " = " + num * multiplicador );
         multiplicador++;
    
         }
         while (i<25 && num!=0);
         } 
     }

### Ejercicios - for

1. Imprimir los números impares del 1 al 50.

       import java.util.Scanner;
       public class Main {
         public static void main(String[] args) {
         for (int i=1; i<50; i+=2) {
         System.out.println(i);
         }
         }
     }

2. Imprimir los números primos del 1 al 100.

     import java.util.Scanner;

     public class SESION5 
    
         public static void main (String [] args){
         for (int i=1 ;i<=100);{
         if (i % 2==0);{
         System.out.println("i");
         }
         i ++;
         }
         }    
       


