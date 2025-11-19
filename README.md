> # Java
Basics by Chatri_amg
 ### Variables primitivas
- - -
- - - 
> Numeros:

- Byte
- short
- int
- long

> #### Decimales
- float 
- double

> #### Booleanos
- Boolean

- - -
![asd](https://i0.wp.com/rduinostar.com/wp-content/uploads/2012/10/Tipos-de-Variables-Arduino.jpg)
- - -

>#### Cadena / Cadena de texto:
- String
- Char




### Variables no primitivas
- - -
- - -
- integer = null 
    - Se pude usar un valor numerico normal
- constante: 
    - Final 
        - el valor se mantiene, nunca cambia


## Imput del usuario
- - -


``` java
Scanner entrada = new Scanner(System.in);

numero = entrada.nextInt();     

// para texto:
 entrada.next(); 
// texto con mas largo con espacios:
 entrada.nextLine();

//para un solo caracter:

entrada.next().charAt(0);
```

#### Ejemplo
``` Java 
Scanner entrada = new Scanner(System.in);

    char letra;
        System.out.println("digite una cadena: ");
        letra = entrada.next().charAt(2);

        System.out.println("la cadena es: " + letra);

```

Esto es para un char (Un solo caracter)
> ### Observaciones: 
- int normal

- float: no coma, usa punto

#### JOption Pane:
Para cadenas, strings.
```java
import javax.swing.JOptionPane;
// antes del public class
JOptionPane.showInputDialog();
 ```
#### Ejemplo
```java
import javax.swing.JOptionPane;

public class mocoso {

    public static void main(String[] args) {
        String cadena;
        int numero;
        char letra;
        double decimal;

        cadena = JOptionPane.showInputDialog("digite una cadena: ");
        System.out.println(cadena);
 ```
- - - 
- - -
 Para enteros o numeros:
 ```java 
 numero = Integer.parseInt(JOptionPane.showInputDialog(""));
 ```

 #### Ejemplo
 ```java
 import javax.swing.JOptionPane;

public class mocoso {

    public static void main(String[] args) {
        int numero;
        

        numero = Integer.parseInt(JOptionPane.showInputDialog(""));
            System.out.println(numero);  
    }
}
  ```
- - -
- - -
Para un solo caracter:

```java
JOptionPane.showInputDialog("").charAt(0);
```
#### Ejemplo
```java
import javax.swing.JOptionPane;

public class mocoso {

   public static void main(String[] args) {
       char letra;
       

       letra = JOptionPane.showInputDialog("").charAt(0);
           System.out.println(letra);  
   }
}
 ```
- - -
- - -
Para decimales:
```java
Double.parseDouble(JOptionPane.showInputDialog(""));
```
#### Ejemplo
```java 
import javax.swing.JOptionPane;

public class mocoso {

   public static void main(String[] args) {
       double decimal;
       

       decimal = Double.parseDouble(JOptionPane.showInputDialog(" "));
           System.out.println(decimal);  
   }
}
```
- - -
- - -
### Ejemplo completo
```java
import javax.swing.JOptionPane;

public class mocoso {

    public static void main(String[] args) {
        String cadena;
        int numero;
        char letra;
        double decimal;

        cadena = JOptionPane.showInputDialog("digita mi huevo: ");
        numero = Integer.parseInt(JOptionPane.showInputDialog("digita tu edad:"));
        decimal = Double.parseDouble(JOptionPane.showInputDialog("digita tu altura: "));
        letra  = JOptionPane.showInputDialog("digita una letra: ").charAt(0);


            System.out.println(cadena);
            System.out.println(numero);
            System.out.println(decimal);
            System.out.println(letra);


    }
}

 ```
