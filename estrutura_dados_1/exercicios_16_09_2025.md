Mostrar todos os programas de todos os exercícios no seu GitHub até hoje (16/09/2025);

1) Transforme a matriz do programa ArrayBidimensional.java para 5 x 5;
2) Por que não aumentar o array diretamente?

A imutabilidade do tamanho do array é uma característica de Java. Isso porque a alocação de memória para um array é contígua e fixa. Se um array pudesse "crescer", ele exigiria mais espaço do que o inicialmente alocado, o que poderia invadir o espaço de memória de outras variáveis. A solução de copiar para um novo array garante que a nova alocação de memória seja feita de forma segura.

Alternativa: Use ArrayList

Para situações em que você precisa de uma lista de elementos com tamanho dinâmico, a melhor solução é usar a classe ArrayList. Ela é muito mais prática e eficiente para lidar com coleções que precisam aumentar ou diminuir de tamanho.

Teste o programa: AumentarArray.java

3) Arrays Irregulares (ou "Jagged Arrays"). Em Java, arrays multidimensionais não precisam ter um número fixo de colunas em todas as linhas. Você pode ter arrays onde cada "linha" (sub-array) tem um tamanho diferente. Execute o programa ArrayIrregular.java e veja o resultado;
4) Adicione 10 elementos no programa ExemploPilhaSimples1.java;
5) Empilhe 10 elementos no programa ExemploPilhaSimples2.java;
6) Coloque 5 URLs reais no programa ExemploStack.java;
7) Qual a função do método Arrays.sort(nomes) no programa OrdenaArray.java?



/*
 * ===============================================
 *          ATIVIDADES - DIA 16/09/2025
 * Autor: Guilherme Abreu
 * Descrição: Exercícios com matrizes, pilhas e arrays em Java
 * ===============================================
 */

public class ExerciciosDia16 {

    // Exercício 1 - Mostrar todos os programas já feitos
    public static void exercicio1() {
        System.out.println("Exercício 1: Mostrar todos os programas já feitos até hoje.");
        System.out.println("-> Este exercício é prático: os programas já estão no repositório do GitHub.");
    }

    // Exercício 2 - Matriz 5x5
    public static void exercicio2() {
        System.out.println("\nExercício 2: Matriz 5x5");

        int[][] matriz = new int[5][5];
        int valor = 1;

        for (int i = 0; i < 5; i++) {
            for (int j = 0; j < 5; j++) {
                matriz[i][j] = valor++;
                System.out.print(matriz[i][j] + "\t");
            }
            System.out.println();
        }
    }

    // Exercício 3 - Array Irregular
    public static void exercicio3() {
        System.out.println("\nExercício 3: Array Irregular");

        int[][] arrayIrregular = new int[3][];
        arrayIrregular[0] = new int[]{1, 2};
        arrayIrregular[1] = new int[]{3, 4, 5};
        arrayIrregular[2] = new int[]{6};

        for (int i = 0; i < arrayIrregular.length; i++) {
            for (int j = 0; j < arrayIrregular[i].length; j++) {
                System.out.print(arrayIrregular[i][j] + " ");
            }
            System.out.println();
        }
    }

    // Exercício 4 - Pilha simples
    public static void exercicio4() {
        System.out.println("\nExercício 4: Pilha Simples com 10 elementos");

        java.util.Stack<Integer> pilha = new java.util.Stack<>();

        for (int i = 1; i <= 10; i++) {
            pilha.push(i);
            System.out.println("Empilhado: " + i);
        }

        System.out.println("Elementos na pilha: " + pilha);
    }

    // Exercício 5 - URLs em uma pilha
    public static void exercicio5() {
        System.out.println("\nExercício 5: URLs na pilha");

        java.util.Stack<String> urls = new java.util.Stack<>();
        urls.push("https://www.google.com");
        urls.push("https://www.github.com");
        urls.push("https://www.stackoverflow.com");
        urls.push("https://www.oracle.com");
        urls.push("https://www.youtube.com");

        while (!urls.isEmpty()) {
            System.out.println("Visitando: " + urls.pop());
        }
    }

    // Exercício 6 - Ordenar nomes
    public static void exercicio6() {
        System.out.println("\nExercício 6: Ordenação de nomes");

        String[] nomes = {"Carlos", "Ana", "Beatriz", "Daniel", "Eduardo"};

        java.util.Arrays.sort(nomes);

        for (String nome : nomes) {
            System.out.println(nome);
        }
    }

    // Main
    public static void main(String[] args) {
        exercicio1();
        exercicio2();
        exercicio3();
        exercicio4();
        exercicio5();
        exercicio6();
    }
}
