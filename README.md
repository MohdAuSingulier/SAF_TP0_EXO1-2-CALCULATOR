# SAF_TP0_JAVA_EXO1-2-CALCULATOR

## EXO 1
/**
 * SAF Mohamed
 * BDML 1 - EFREI Paris
 * Programmation en Java - Exo 1
 * Proposée par Madame Georgina ABI SEJAAN
 * Le 22 Septembre 2026
 */
public class Exo1 {

    public static void main(String[] args) {
        String prenom;
        Scanner sc;
        sc = new Scanner(System.in);
        System.out.println("Bonjour, quel est votre prenom ?");
        prenom = sc.nextLine();
        //Ajout :
        System.out.println("Enchanté, " + prenom + " !");
        System.out.println("Au revoir !");

    }
}

## EXO 2
/**
 *
 * @author Mohamed_SF
 */
public class Exo2 {

 /**
 * SAF Mohamed
 * BDML 1 - EFREI Paris
 * Programmation en Java - Exo 2
 * Proposée par Madame Georgina ABI SEJAAN
 * Le 22 Septembre 2026
 */
    public static void main(String[] args) {
        //Declaration des variables
        int nb; // nombre d'entiers à additionner
        int result; // resultat
        int ind; // indice
        Scanner sc = new Scanner(System.in);
        System.out.println("\n Entrer le nombre :");
        nb=sc.nextInt(); // On demande a sc de donner le prochain entier
        result=0;
        
        // Addition des nb premiers entiers
        ind=1;
        while (ind <= nb) {
            result=result+ind;
            //Ajout pour la correction : 
            ind++; //Pareil que ind = ind + 1 comme vu en cours
        }
        
        // Affichage du résultat
        System.out.println();
        System.out.println("La somme des "+ nb + "entiers est: "+result);
    }
}

## CALCULATOR

/*
 * Projet : Calculator
 * Auteur : SAF Mohamed
 * Classe : BDML 1 - EFREI Paris
 * Cours : Programmation en Java - Exo 1
 * Enseignante : Madame Georgina ABI SEJAAN
 * Date : 22 Septembre 2026
 */
package calculator;

import java.util.Scanner;

/**
 *
 * @author Mohamed_SF
 */

public class Calculator {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        // --- MENU & OPERATEUR ---
        System.out.println("Please enter the operator:");
        System.out.println("1) add");
        System.out.println("2) substract");
        System.out.println("3) multiply");
        System.out.println("4) divide");
        System.out.println("5) modulo");
        int operateur = sc.nextInt();
        
        // AJOUT du TEST DE L'OPERATEUR ERRONÉ
        // Si le nombre n'est pas entre 1 et 5, on met une erreur et on arrête tout.
        if (operateur < 1 || operateur > 5) {
            System.out.println("Error: Invalid operator! Please run the program again.");
            return; // Cette ligne arrête le programme immédiatement
        }
        // OPERANDE 1 
        System.out.println("Please enter the first number:");
        double operande1 = sc.nextDouble();
        
        //OPERANDE 2 ---
        System.out.println("Please enter the second number:");
        double operande2 = sc.nextDouble();
        
        //  CALCULS AVEC IF / ELSE ---
        double result = 0;
        
        if (operateur == 1) {
            result = operande1 + operande2;
        } else if (operateur == 2) {
            result = operande1 - operande2;
        } else if (operateur == 3) {
            result = operande1 * operande2;
        } else if (operateur == 4) {
            // Attention la division par zéro dans la vraie vie, mais restons simple ici
            result = operande1 / operande2;
        } else if (operateur == 5) {
            result = operande1 % operande2;
        } else {
            System.out.println("Invalid operator!");
            return; // Arrête le programme si le choix n'est pas entre 1 et 5
        }
        
        // Affichage final
        System.out.println("The result is : " + result);
    }
}

