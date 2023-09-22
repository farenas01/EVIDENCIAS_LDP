<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


# Actividad 3: Ejercicios de operaciones básicas en Java.

1. Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

### Solución:

    import java.util. Scanner;
    
    public class EjerciciosSesion3 {
         
         public static void main (String [] args) {
             Scanner entradaDatos = new Scanner (System.in);
             
             System.out.println("ingrese el primer numero");
             int numl = entradaDatos.nextInt ();
         
             System.out.println("ingrese el segundo numero");
             int num2 = entradaDatos.nextInt ();

             int suma = numl + num2;
             int multiplicacion = numl * num2;

             System.out.println ("La suma es: " + suma);
             System.out.println ("La multiplicacion es: " + multiplicacion);
        
             }

    }

2. Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

### Solución:

    import java.util. Scanner;
    
    public class EjerciciosSesion3 {

         public static void main (String [] args) {
            Scanner entradaDatos = new Scanner (System.in);

            System.out.println("ingrese el primer numero");
            int numl = entradaDatos.nextInt ();

            System.out.println ("ingrese el segundo numero");
            int num2 = entradaDatos.nextInt ();

            int resta = numl - num2;
            int division = numl / num2;

            System.out.println ("La resta es: " + resta);
            System.out.println ("La division es: " + division);

         }

    }

3. Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

### Solución: 

    import java.util. Scanner;

    public class EjerciciosSesion3 {
         
         public static void main(String[] args) {
             Scanner entradaDatos = new Scanner (System.in);

             System.out.println ("ingrese el primer numero");
             int numl = entradaDatos.nextInt ();

             System.out.println ("ingrese el segundo numero");
             int num2 = entradaDatos.nextInt ();

             System.out.println("ingrese el tercer numero");
             int num3 = entradaDatos.nextInt ();

             int suma = numl + num2 + num3;
             int total = (numl * num2) / num3;

             System.out.println ("La suma de los tres numeros es: " + suma);
             System.out.println ("el resultado de los dos primeros numeros dividido por el tercero es: " + total);

         }

    }

4. Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

### Solución:

    import java.util. Scanner;

    public class EjerciciosSesion3 {

         public static void main (String [] args) {
             Scanner entradaDatos = new Scanner (System.in);

             System.out.println ("ingrese el primer numero decimal");
             float numl = entradaDatos.nextFloat ();

             System.out.println ("ingrese el segundo numero decimal");
             float num2 = entradaDatos.nextFloat ();

             float suma = num1 + num2;
             float resta = num1 - num2;
             float multiplicacion = num1 * num2;
             float division = num1 / num2;

             System.out.println ("La suma de los 2 numeros es: " + suma);
             System.out.println ("La resta de los 2 numeros es: " + resta);
             System.out.println ("La multiplicacion de los 2 numeros es: " + multiplicacion);
             System.out.println ("La division de los 2 numeros es: " + division);

         }

    }

5. Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

### Solución:

    import java.util. Scanner;

    public class EjerciciosSesion3 {

         public static void main (String [] args) {
             int numero = 51;

             numero + = 3;
             System.out.println ("El resultado del incremento en numero es: " + numero);

             numero - = 0x3;
             System.out.println ("El resultado del decremento en numero es: " + numero);

         }

    }

6. Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

### Solución:

    import java.util. Scanner;

    public class EjerciciosSesion3 {

         public static void main (String [] args) {

            int num= 53;
            num + =5; 

            System.out.println ("El resultado de la asignacion compuesta mas 5 es: " + num);

         }

    }

7. Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

### Solución:

    import java.util. Scanner;

    public class EjerciciosSesion3 {
         
         public static void main(String[] args) {
             Scanner entradaDatos = new Scanner (System.in);

             System.out.println ("ingreso a la montaña rusa");

             System.out.println ("su edad es mayor a 18");
             boolean edad = entradaDatos.hasNextBoolean ();

             System.out.println ("su altura es mayor a 1 metro");
             boolean altura = entradaDatos.hasNextBoolean ();

             boolean ingresomontañaR1 = edad && altura;
             boolean ingresomontañaR2 = !edad;
             boolean ingresomontañaR3 = !altura;
             boolean ingresomontañaR4 = edad || altura;

             System.out.println ("Resultado de ingreso a la montañaR1 es: " + ingresomontañaR1);
             System.out.println ("Resultado de ingreso a la montañaR2 es: " + ingresomontañaR2);
             System.out.println ("Resultado de ingreso a la montañaR3 es: " + ingresomontañaR3);
             System.out.println ("Resultado de ingreso a la montañaR4 es: " + ingresomontañaR4);

         }

    }

8. Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.

### Solución:

    import java.util. Scanner;

    public class EjerciciosSesion3 {

         public static void main(String[] args) {

         Scanner entradaDatos = new Scanner(System.in);
         System.out.println("Ingrese un número");

         int num = entradaDatos.nextInt();

         if (num == 1) {
         System.out.println("Es un número entero");
         } 
        
         else if (num <= 1) {
         System.out.println("Es un número negativo");
         } 
         else {
         System.out.println("Es un número positivo");}
    
         }
    }







             





