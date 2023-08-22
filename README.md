# java_aula4

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package aula.pkg03;

import java.util.Scanner;

/**
 *
 * @Alan manager
 */
public class Aula03 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        String nome = "Alan";
        int valor1, valor2, soma, sub, mult, div;

        Scanner entrada = new Scanner(System.in);
        
        System.out.println("Digite um numero : ");
        valor1 = entrada.nextInt();
        System.out.println("Digite outro numero : ");
        valor2 = entrada.nextInt();       
        
        soma = valor1 + valor2;
        sub = valor1 - valor2;
        mult = valor1 * valor2;
        div = valor1 / valor2;

        System.out.println(nome);
        System.out.println("A soma é : " + soma);
        System.out.println("A subtração é : " + sub);
        System.out.println("A multiplicação é : " + mult);

        if (div <= 0) {
            System.out.println("Divisão menor que ZERO");
        } else {
            System.out.println("A divisão é : " + div);
        }

        System.out.println("Laço de repetição FOR");

        for (int i = 0; i <= valor1; i++) {
            System.out.println("nº " + i);
        }

        System.out.println("Laço de repetição WHILE");

        while (valor1 > valor2) {
            System.out.println("nº " + valor1);
            valor1--;
        }

        System.out.println("Laço de repetição DO WHILE");

        do {
            System.out.println("nº " + valor1);
            valor1++;
        } while (valor1 < valor2);
        
        
        
    }
}
