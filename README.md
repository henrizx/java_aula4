package exercicio01;

import java.util.Scanner;

public class Exercicio01 {

    public static void main(String[] args) {
        String nome = "Alan";

        int valor1, valor2, soma, sub, mult, div, qtamgs;

        Scanner entrada = new Scanner(System.in);

        System.out.println("Digite um número: ");
        valor1 = entrada.nextInt();
        entrada.nextLine(); // Consumir a nova linha

        System.out.println("Digite outro número: ");
        valor2 = entrada.nextInt();
        entrada.nextLine(); // Consumir a nova linha

        soma = valor1 + valor2;
        sub = valor1 - valor2;
        mult = valor1 * valor2;
        div = valor1 / valor2;

        System.out.println(nome);
        System.out.println("A soma é: " + soma);
        System.out.println("A subtração é: " + sub);
        System.out.println("A multiplicação é: " + mult);

        if (div <= 0) {
            System.out.println("Divisão menor ou igual a ZERO");
        } else {
            System.out.println("A divisão é: " + div);
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

        // Array de nomes
        String[] nomes = {"Barbara", "Amanda", "Rafael", "Romario"};

        System.out.println("Nomes no array:");
        for (String nomeArray : nomes) {
            System.out.println(nomeArray);
        }

        // Captura a quantidade de amigos
        System.out.print("Quantos amigos você possui? ");
        qtamgs = entrada.nextInt();

        entrada.close();
    }
}
