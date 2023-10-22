<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


### Solución

```java
    import java.util.Scanner;
    import java.text.DecimalFormat;

    public class Main {
       public static void main(String[] args) {
        DecimalFormat decimalFormat = new DecimalFormat("#,###");
        Scanner scanner = new Scanner(System.in);

        System.out.println("Bienvenido al calculador de CDT!");

        // Pedir al usuario que ingrese los datos del CDT
        System.out.print("Ingrese el monto del depósito: ");
        double montoDeposito = scanner.nextDouble();

        System.out.print("Ingrese la tasa de interés anual (%): ");
        double tasaInteresAnual = scanner.nextDouble();

        System.out.print("Ingrese el plazo en meses: ");
        int plazoMeses = scanner.nextInt();

        // Calcular el interés y el monto total al vencimiento
        double tasaInteresMensual = tasaInteresAnual / 12 / 100;
        double interesMensual = montoDeposito * tasaInteresMensual;
        double montoTotalVencimiento = montoDeposito + (interesMensual * plazoMeses);

        // Mostrar el resumen del CDT
        System.out.println("Resumen del CDT:");
        System.out.println("- Monto del depósito: $" + decimalFormat.format(montoDeposito));
        System.out.println("- Tasa de interés anual: " + tasaInteresAnual + "%");
        System.out.println("- Plazo en meses: " + plazoMeses);
        System.out.println("- Interés mensual: $" + interesMensual);
        System.out.println("- Monto total al vencimiento: $" + decimalFormat.format(montoTotalVencimiento));
        }
    }


### Explicación detallada

La explicación del programa Java que escogi es sobre como poder calcular el interés de un CDT:

1. **Importación de paquetes y clases:**
   - Se importan las clases `Scanner` y `DecimalFormat` del paquete `java.util`. `Scanner` se utiliza para obtener entrada del usuario, y `DecimalFormat` se utiliza para formatear números con comas y decimales en el resultado.

2. **Método `main`:**
   - El programa comienza con la definición del método `main`, que es el punto de entrada del programa.

3. **Creación de objetos:**
   - Se crea un objeto `DecimalFormat` llamado `decimalFormat` que se utiliza para formatear los números en el resultado final.
   - Se crea un objeto `Scanner` llamado `scanner` para leer la entrada del usuario desde la consola.

4. **Mensaje de bienvenida:**
   - Se muestra un mensaje de bienvenida en la consola para dar inicio al programa.

5. **Entrada de datos:**
   - El programa solicita al usuario que ingrese tres valores:
     - El monto del depósito en una variable `montoDeposito`.
     - La tasa de interés anual en una variable `tasaInteresAnual`.
     - El plazo en meses en una variable `plazoMeses`.

6. **Cálculo de interés y monto total al vencimiento:**
   - Se calcula la tasa de interés mensual dividiendo la tasa de interés anual entre 12 (para obtener la tasa mensual) y luego dividiendo por 100 para convertirla a un valor decimal.
   - El interés mensual se calcula multiplicando el monto del depósito por la tasa de interés mensual.
   - El monto total al vencimiento se calcula sumando el monto del depósito al producto del interés mensual y el plazo en meses.

7. **Mostrar el resumen del CDT:**
   - Se muestra un resumen de los datos ingresados y los resultados del CDT en la consola. Los valores se formatean utilizando el objeto `DecimalFormat` para incluir comas en los miles y mostrar dos decimales en el interés mensual y el monto total al vencimiento.

En resumen, este programa Java es un calculador de Certificados de Depósito a Término (CDT) que toma los datos del depósito, la tasa de interés y el plazo en meses, y calcula el interés mensual y el monto total al vencimiento. Luego, muestra un resumen de estos valores en la consola.


### Solución

```java
    import java.util.Scanner;

    public class CalculoCostoEnergiaElectrica {
       public static void main(String[] args) {
      Scanner input = new Scanner(System.in);

      // Solicitar datos al usuario
      System.out.print("Ingrese la potencia del electrodoméstico (en vatios): ");
      double potencia = input.nextDouble();
      
      System.out.print("Ingrese el tiempo de uso diario (en horas): ");
      double tiempoUsoDiario = input.nextDouble();
      
      System.out.print("Ingrese el precio por kilovatio-hora (en pesos): ");
      double precioKwh = input.nextDouble();
      
      System.out.print("Ingrese el número de días del mes: ");
      int diasDelMes = input.nextInt();
      
      // Cálculo del consumo mensual en kilovatios-hora
      double consumoDiarioKwh = (potencia * tiempoUsoDiario) / 1000;
      double consumoMensualKwh = consumoDiarioKwh * diasDelMes;
      
      // Cálculo del costo mensual de energía eléctrica
      double costoEnergiaElectrica = consumoMensualKwh * precioKwh / 1000; // se divide entre 1000 para convertir el precio por kilovatio-hora en pesos
      
      // Imprimir el resultado en pantalla
      System.out.printf("El costo mensual de energía eléctrica es de: $%,.2f pesos", costoEnergiaElectrica);
      }
    }


### Explicación detallada

La explicación del programa Java que escogi es sobre el costo mensual de energía eléctrica del electrodomésticos:

1. **Importación de la clase Scanner:**
   - Se importa la clase `Scanner` del paquete `java.util`, que se utiliza para obtener entrada del usuario desde la consola.

2. **Método `main`:**
   - El programa comienza con la definición del método `main`, que es el punto de entrada del programa.

3. **Creación de un objeto Scanner:**
   - Se crea un objeto `Scanner` llamado `input` para leer la entrada del usuario desde la consola.

4. **Solicitud de datos al usuario:**
   - El programa solicita al usuario que ingrese cuatro valores:
     - La potencia del electrodoméstico en vatios, que se almacena en la variable `potencia`.
     - El tiempo de uso diario del electrodoméstico en horas, que se almacena en la variable `tiempoUsoDiario`.
     - El precio por kilovatio-hora en pesos, que se almacena en la variable `precioKwh`.
     - El número de días del mes, que se almacena en la variable `diasDelMes`.

5. **Cálculo del consumo mensual en    kilovatios-hora:**
   - Se calcula el consumo diario en kilovatios-hora (`consumoDiarioKwh`) multiplicando la potencia del electrodoméstico por el tiempo de uso diario y dividiendo por 1000 (para convertir vatios en kilovatios).
   - Luego, se calcula el consumo mensual en kilovatios-hora (`consumoMensualKwh`) multiplicando el consumo diario por el número de días del mes.

6. **Cálculo del costo mensual de energía eléctrica:**
   - Se calcula el costo mensual de la energía eléctrica (`costoEnergiaElectrica`) multiplicando el consumo mensual en kilovatios-hora por el precio por kilovatio-hora en pesos. Se divide por 1000 para convertir el precio a pesos por kilovatio-hora.

7. **Imprimir el resultado en pantalla:**
   - Se muestra el resultado en la consola utilizando `System.out.printf()` para formatear el resultado con comas en los miles y dos decimales en el costo. El resultado muestra el costo mensual de energía eléctrica en pesos.

En resumen, este programa Java es un calculador de costo de energía eléctrica que toma la potencia del electrodoméstico, el tiempo de uso diario, el precio por kilovatio-hora y el número de días del mes. Luego, calcula el consumo mensual en kilovatios-hora y el costo mensual de energía eléctrica, y muestra el resultado formateado en la consola.






