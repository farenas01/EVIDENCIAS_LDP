<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


### Actividad 4: Ejercicios de control de flujo con expresiones compuestas.

    // Variables de tipo String
    String nombre = "Juan Pérez";
    String apellido = "González";
    String identificación = "1000000001";
    String correo = "juan.perez@ejemplo.com";
    String carrera = "Desarrollo de Software";
    String universidad = "Cesde";
    // Variable de tipo int
    int edad = 20;
    // Variable de tipo boolean
    boolean esActivo = true;
    boolean becado = false;
    // Variable de tipo char
    char género = 'M';
    // Variable de tipo double
    double promedio = 4.5;
    // Variable de tipo int
    int semestre = 2;


Con la información anterior, implementa los siguientes ejercicios:

1. Determinar si el estudiante es mayor de edad y tiene un estado activo.
2. Determinar si el estudiante tiene una beca o una carrera relacionada con el desarrollo de software.
3. Determinar si el estudiante está en el último semestre de su carrera y tiene un estado activo.
4. Determinar si el estudiante tiene una carrera relacionada con el desarrollo de software y un promedio superior a 4.0.
5. Mostrar toda la información del estudiante si está matriculado en el Cesde.
6. Asignar una beca del 50% si el estudiante está matriculado en el Cesde, tiene un promedio superior a 4.0 y está activo.
7. Determinar la cantidad de beca que recibe el estudiante según su promedio:
     * 0.0 - 3.4: El estudiante no recibe beca.
     * 3.5 - 3.9: El estudiante recibe una beca parcial del 25%.
     * 4.0 - 4.4: El estudiante recibe una beca parcial del 50%.
     * 4.5 - 5.0: El estudiante recibe una beca completa.

### Solución:

     import java.util. Scanner;
     
     public class Sesion4Logica {

        public static void main(String[] args) {
        String nombre = "Fernando";
        String apellido = "Sánchez";
        String documento = "128773612";
        String correo = "Fernando.sánchez@programaciondesof.com";
        String carrera = "Desarrollo de Software";
        String universidad = "Cesde";
        // Variable de tipo int: Se utiliza para asignar un valor a una variable de tipo entero.
        int edad = 26;
        // Variable de tipo boolean: Comprueba si dos valores son iguales.
        boolean esActivo = true;
        boolean becado = false;
        // Variable de tipo char: se usa para almacenar el valor entero de un miembro del juego de caracteres que se puede representar.
        char genero = 'M';
        // Variable de tipo double: es similar a float, pero se utiliza cuando la precisión de una variable de coma flotante no es suficiente
        double promedio = 4.5;
        // Variable de tipo int: Se utiliza para asignar un valor a una variable de tipo entero.
        int semestre = 3;

        System.out.println ("-----------------------------------------------------------------------------------");
        System.out.println("Ejercicio1: Determinar si el estudiante es mayor de edad y se encuentra activo.");
        System.out.println("-----------------------------------------------------------------------------------");

        if (edad >= 18) {
            System.out.println("El estudiante es mayor de edad");
            if (esActivo) {
                System.out.println("el estudiante esta activo");

            } else {
                System.out.println("El estudiante es menor de edad");
            }
        } else {
            System.out.println("el estudiante no se encuentra activo");
        }

        System.out.println("---------------------------------------------------------------------------------------------------------------");
        System.out.println("ejercicio 2: Determinar si el estudiante tiene una beca o una carrera relacionada con el desarrollo de software.");
        System.out.println("---------------------------------------------------------------------------------------------------------------");
        if (carrera.equals("Desarrollo de Software") || becado) {
            System.out.println("El estudiante cumple con alguna o con todas las condicciones");

        }

        System.out.println("---------------------------------------------------------------------------------------------------------");
        System.out.println("ejercicio 3: Determinar si el estudiante está en el último semestre de su carrera y tiene un estado activo.");
        System.out.println("----------------------------------------------------------------------------------------------------------");

        if (semestre == 3) {
            System.out.println("El estudiante cumple con las condicciones");
        } else if (esActivo) {
            System.out.println("El estudiante no cumple con una de las condiciones, pero si con una ");
        } else {
            System.out.println("El estudiante no cumple con ninguna de las condiciones.");
        }

        System.out.println("------------------------------------------------------------------------------------------------------------------");
        System.out.println("Ejercicio4: Determinar si el estudiante tiene una carrera relacionada con el desarrollo de software y un promedio superior a 4.0.");
        System.out.println("-----------------------------------------------------------------------------------------------------------------------");

        if (carrera.equals("Desarrollo de Software") && promedio >= 4.0) {
            System.out.println("el estudiante cumple con los requisitos");
        }

        System.out.println("-------------------------------------------------------------------------------------------------------");
        System.out.println("Ejercicio5: Mostrar toda la información del estudiante si está matriculado.");
        System.out.println("-------------------------------------------------------------------------------------------------------");

        if (universidad.equals("Cesde")) {
            System.out.println("Nombre del estudiante: " + nombre + "\napellido del  estudiante: " + apellido
                    + "\nNumero de documento: " + documento + "\nCorreo: " + correo + "\nNombre de carrera: " + carrera
                    + "\nUniversidad: " + universidad + "\nEdad: " + edad + "\nEstado del estudiante: " + esActivo + "\nTiene beca: " + becado
                    + "\nGenero: " + genero + "\nPromedio del estudiante: " + promedio + "\nSemestre: " + semestre);
        } else {
            System.out.println("El estudiante no esta matriculado.");
        }

        System.out.println("---------------------------------------------------------------------------------------------------------");
        System.out.println("Ejercicio6: Asignar una beca del 50% si el estudiante está matriculado en el Cesde, si tiene un promedio superior a 4.0 y si está activo.");
        System.out.println("--------------------------------------------------------------------------------------------------------------");

        if (universidad.equals("Cesde") && promedio >= 4.0 && esActivo) {
            System.out.println("El estudiante tiene una beca del 50% por cumplir con los requisitos. ");

        } else {
            System.out.println("El estudiante no cumple con los requisitos, por tal motivo no tiene beca");
        }

        System.out.println("------------------------------------------------------------------------------------");
        System.out.println(" Ejercicio7: Determinar la cantidad en % de beca que recibe el estudiante según su promedio estudiantil.:\n"
                + "0.0 - 3.4: El estudiante no es becado.\n"
                + "3.5 - 3.9: El estudiante recibe una beca parcial del 25%.\n"
                + "4.0 - 4.4: El estudiante recibe una beca parcial del 50%.\n"
                + "4.5 - 5.0: El estudiante es becado completamente.");
        System.out.println("--------------------------------------------------------------------------------------");

        if (promedio >= 0.0 && promedio <= 3.4) {
            System.out.println("El estudiante no es becado. ");

        } else if (promedio >= 3.4 && promedio <= 3.9) {
            System.out.println("El estudiante recibe una beca parcial del 25%. ");

        } else if (promedio >= 4.0 && promedio <= 4.4) {
            System.out.println("El estudiante recibe una beca parcial del 50%.");
        } else if (promedio >= 4.5 && promedio <= 5.0) {
            System.out.println("El estudiante es becado completamente.");
        }

        System.out.println("-----------------------------------------------------------------------------------------");
        System.out.println("Ejercicio8: Determinar si la estudiante es mujer, puede jugar en el equipo de volleyball");
        System.out.println("------------------------------------------------------------------------------------------");

        if (genero == 'M') {
            System.out.println("La estudiante puede jugar en el equipo de volleyball");
        } else {
            System.out.println("La estudiante no puede jugar en el equipo de volleyball.");
        }

        System.out.println("--------------------------------------------------------------------------------------------------------------------");
        System.out.println("Ejercicio9: Determinar si el estudiante tiene una edad mayor o igual a 18 para poder ingresar a la U");
        System.out.println("-------------------------------------------------------------------------------------------------------------------");

        if (edad >= 18) {
            System.out.println("El estudiante puede ingresar a la U");

        } else {
            System.out.println("El estudiante no puede ingresar a la U");
        }

        System.out.println("--------------------------------------------------------------------------------------------------");
        System.out.println("Ejercicio10: Determinar si el estudiante esta en el segundo semestre para habilitar el curso catedra de emprendedor. ");
        System.out.println("---------------------------------------------------------------------------------------------------------------");

        if (semestre == 2) {
            System.out.println("Tienes activo el curso catedra de emprendedor.");

        } else {
            System.out.println("No tienes activo el curso catedra de emprendedor.");
        }

    }
}





