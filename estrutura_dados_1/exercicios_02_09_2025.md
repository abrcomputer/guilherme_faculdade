1) Crie um programa em Java que declare e inicialize um vetor de inteiros com 5 posições. Atribua valores a cada uma das posições e, em seguida, imprima no console o valor armazenado na terceira posição do vetor (índice 2).
2) Crie um programa em Java que declare um **vetor de booleanos** chamado `status` com 3 posições. Atribua os valores `true`, `false` e `true` a cada uma das posições, respectivamente.

Em seguida, use uma estrutura de controle **`if-else`** para verificar o valor da **primeira posição** do vetor (`status[0]`) e imprima a seguinte mensagem:

* Se o valor for `true`, exiba: "O primeiro status está ativo."
* Se o valor for `false`, exiba: "O primeiro status está inativo."
3) Crie um programa em Java que declare e inicialize um **vetor de inteiros** chamado `notas` com os seguintes valores: `85, 92, 78, 95, 88`.

Em seguida, utilize um **laço de repetição `for`** para percorrer todos os elementos do vetor. Dentro do laço, imprima cada nota no console, acompanhada de sua respectiva posição (por exemplo: "Nota 1: 85", "Nota 2: 92", e assim por diante).

4) Crie um programa em Java que declare e inicialize um **vetor de números decimais** (`double`) chamado `precos`, com os seguintes valores: `1.50, 2.75, 5.00, 3.25`.

Em seguida, use um **laço de repetição `for`** para percorrer todos os elementos do vetor, calculando a soma total dos valores. Ao final do programa, imprima o resultado da soma no console.

5) Crie um programa em Java que declare e inicialize um **vetor de `Strings`** chamado `frutas` com os valores "Maçã", "Banana", "Laranja" e "Uva".

Em seguida, o programa deve realizar as seguintes ações:

1.  Imprimir o valor da **primeira posição** do vetor.
2.  **Alterar** o valor da segunda posição para "Morango".
3.  Imprimir o **novo valor** da segunda posição no console.

/*
 
 * ===============================================
 *          ATIVIDADES - DIA 02/09/2025
 * Autor: Guilherme Abreu
 * Descrição: Exercícios com vetores (arrays) em Java
 * ===============================================
 */

public class ExerciciosDia02 {

    // Exercício 1 - Vetor de inteiros
    public static void exercicio1() {
        System.out.println("Exercício 1: Vetor de inteiros");
        int[] numeros = {10, 20, 30, 40, 50};
        System.out.println("O valor da terceira posição é: " + numeros[2]);
    }

    // Exercício 2 - Vetor de booleanos
    public static void exercicio2() {
        System.out.println("\nExercício 2: Vetor de booleanos");
        boolean[] status = {true, false, true};

        if (status[0]) {
            System.out.println("O primeiro status está ativo.");
        } else {
            System.out.println("O primeiro status está inativo.");
        }
    }

    // Exercício 3 - Vetor de notas
    public static void exercicio3() {
        System.out.println("\nExercício 3: Vetor de notas");
        int[] notas = {85, 92, 78, 95, 88};

        for (int i = 0; i < notas.length; i++) {
            System.out.println("Nota " + (i + 1) + ": " + notas[i]);
        }
    }

    // Exercício 4 - Vetor de preços
    public static void exercicio4() {
        System.out.println("\nExercício 4: Vetor de preços");
        double[] precos = {1.50, 2.75, 5.00, 3.25};
        double soma = 0;

        for (int i = 0; i < precos.length; i++) {
            soma += precos[i];
        }

        System.out.println("Soma total: " + soma);
    }

    // Exercício 5 - Vetor de frutas
    public static void exercicio5() {
        System.out.println("\nExercício 5: Vetor de frutas");
        String[] frutas = {"Maçã", "Banana", "Laranja", "Uva"};

        System.out.println("Primeira fruta: " + frutas[0]);

        frutas[1] = "Morango";
        System.out.println("Nova segunda fruta: " + frutas[1]);
    }

    // Main
    public static void main(String[] args) {
        exercicio1();
        exercicio2();
        exercicio3();
        exercicio4();
        exercicio5();
    }
}
