# Dados

package dados_rpg;

import java.util.Random;
import java.util.Scanner;

/**
 * Fiz esse rápido programinha para rolar alguns dados e compor uma ficha de
 * personagem de um RPG do qual eu vou participar.
 * 
 * E-mail: gabrielmarques142@gmail.com
 * @author Gabriel Marques
 */
public class Dados_RPG {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        int faces,result;
        Random sorte = new Random();
        Scanner scan = new Scanner(System.in);

        System.out.println("     **** BEM-VINDO(A) **** \n QUANTAS FACES TERÁ O SEU DADO? ");
        faces = scan.nextInt();
        faces = faces + 1;

        result = sorte.nextInt(faces);
        System.out.println("DADO DE " + (faces - 1) + " FACES.\n" + "RESULTADO DA ROLAGEM: " + result + ".");

    }
}
