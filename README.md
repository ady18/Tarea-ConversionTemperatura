package conversiontemperatura;
import java.util.*;
/**
 *
 * @author Adirane
 */
public class ConversionTemperatura {

    public static void main(String[] args) {
        
        Scanner teclado = new Scanner(System.in);
        int c ;
        double f ;
        
        System.out.println("-------------------------------");
        System.out.println("   CONVERSIÓN DE TEMPERATURA   ");
        System.out.println("-------------------------------");
        
        do{
            
            System.out.println("\nIngrese la temperatura en grados Centigrados: °C");
            c = teclado.nextInt();

            if(c == 999){
                break;
            }
 
            System.out.println("\nLa temperatura en Fahrenheit es de " + Celsius(c) + "°F\n");
            
        }while(true);
         System.out.println("\n¡GRACIAS POR USAR EL PROGRAMA!");
    }

    public static double Celsius(double Celsius){
    
        double fahrenheit;
    
            fahrenheit = (Celsius * 9/5) + 32;
            return fahrenheit;
    }
    
}
