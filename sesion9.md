<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 9 


### Solución

```java
    import java.util.HashMap;
    import java.util.Map;

    public class CalculadoraResistencia {

    public static void main(String[] args) {
        // Definir los colores y sus valores
        Map<String, Integer> colores = new HashMap<>();
        colores.put("negro", 0);
        colores.put("marron", 1);
        colores.put("rojo", 2);
        colores.put("naranja", 3);
        colores.put("amarillo", 4);
        colores.put("verde", 5);
        colores.put("azul", 6);
        colores.put("violeta", 7);
        colores.put("gris", 8);
        colores.put("blanco", 9);

        // Solicitar al usuario los colores de las bandas
        String banda1 = "rojo"; // Cambia los valores de las bandas según tus necesidades
        String banda2 = "negro";
        String banda3 = "verde";
        String banda4 = "dorado"; // Tolerancia (cambia según el código de colores de tolerancia)

        // Calcular el valor de la resistencia
        int valor = (colores.get(banda1) * 10 + colores.get(banda2)) * (int)Math.pow(10, colores.get(banda3));
        
        // Calcular la tolerancia
        double tolerancia = 20; // Por defecto, asumimos ±20% (cambia según el código de colores de tolerancia)
        if (colores.containsKey(banda4)) {
            tolerancia = 10 * Math.pow(10, colores.get(banda4));
        }

        // Imprimir el resultado
        System.out.println("El valor de la resistencia es " + valor + " ohmios con una tolerancia del " + tolerancia + "%.");
    }
    }









