package dados.para.rpg;

import java.util.Random;
import java.util.Scanner;

/**
 *
 * @author Gabriel Marques
 */
public class DadosParaRPG {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
    int faces,result; Random sorte = new Random(); 
    Scanner scan = new Scanner(System.in);

    System.out.println(" **** BEM-VINDO(A) **** \n QUANTAS FACES TEM O SEU DADO? "); 
    faces = scan.nextInt(); 
    faces = faces + 1;

    result = sorte.nextInt(faces); System.out.println("DADO DE " + (faces - 1) + " FACES.\n" + "RESULTADO DA ROLAGEM: " + result + ".");

    }
}
