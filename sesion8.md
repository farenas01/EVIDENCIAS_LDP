<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 


## Ejercicios de métodos en Java

1. Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.

### Solución.

import java.util.Scanner;

  public class MayorDosNumeros {
    public static void main(String[] args) {
    Scanner reader = new Scanner (system.in);
    int inumero1, inumero2;
    
    System.out.println("Dame el primer número");
    inumero1 = reader.nextInt();

    System.out.println("Dame el segundo número");
    inumero2 = reader.nextInt();

    if (inumero1>inumero2)
       System.out.println(inumero1 + "es mayor que " + inumero2);
    else
       System.out.println(inumero2 + "es mayor que " + inumero1);

    reader.close();
      
      }
    }

2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.

### Solución.

    import java.util.Scanner;

    public class ContadorDeVocales {
       public static void main(String[] args) {

       const contarVocales = palabra => {
       const vocales = "aáeéiíoóuú";
       let cantidadVocales = 0;
       for (const letra of palabra) {
       //Usamos la función includes de la lista de vocales para saber si la letra es una vocal. Y convertimos la vocal a minúscula usando toLowerCase.

       if (vocales.includes(letra.toLowerCase())) {
            cantidadVocales++;
       }
       }
       return cantidadVocales;
       };

       }
    }

3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.

### Solución.

    import java.util.Scanner;

    public class MayuYMinuInter{
      public static void main(String[] args){
      Scanner sc = new Scanner(System.in);

      System.out.print(«Escribe algo: «);
      String text = sc.nextLine();
      System.out.print(«\n»+text+»\n\n»);
      for(int i=0; i < text.length(); i++){
      if(i % 2 == 0){
      String txt2 = Character.toString(text.charAt(i));
      System.out.print(txt2.toUpperCase());
      }

      else{
      System.out.print(txt.charAt(i));
      }
      }
      System.out.println("\n");
      
      }

      }


4. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.

### Solución.

El programa lee un texto por teclado y lo guarda en un String. A continuación mostrará el número de palabras que contiene.
La forma más sencilla de resolverlo es utilizando la clase StringTokenizer. Esta clase sirve para dividir un String en partes, según unos delimitadores. Uno de estos delimitadores es el espacio en blanco, por lo tanto podemos aplicar StringTokenizer al texto ya que las palabras en un texto están separadas por espacios en blanco. El método countTokens() nos dirá cuantos elementos se han obtenido o lo que es lo mismo, cuantas palabras contiene el texto.


    import java.util.Scanner;
    import java.util.StringTokenizer;
      public class ContarPalabras {
        public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String frase;
        System.out.print("Introduce una frase: ");
        frase = sc.nextLine();
        StringTokenizer st = new StringTokenizer(frase);
        System.out.println("Número de palabras: " + st.countTokens());                                             
        }
      }







