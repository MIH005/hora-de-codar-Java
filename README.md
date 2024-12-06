# hora-de-codar-Java

# Exercícios de Lógica de Programação em Java

Este repositório contém uma série de exercícios de lógica de programação desenvolvidos em **Java**. Os exercícios abordam conceitos básicos e intermediários, como manipulação de variáveis, controle de fluxo, laços de repetição e cálculos matemáticos.

## Exercícios e Soluções

### **1. Baby Steps**
Crie uma variável chamada "Planeta" e atribua a ela o valor "Plutão". Em seguida, exiba o valor para o usuário.

```java
public class BabySteps {
    public static void main(String[] args) {
        String planeta = "Plutão";
        System.out.println("Planeta: " + planeta);
    }
}


import java.util.Scanner;

public class HelloClarice {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Informe o seu nome: ");
        String nome = scanner.nextLine();
        System.out.println("Olá, " + nome);
    }
}


import java.util.Scanner;

public class BitOfInformation {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Informe o seu nome: ");
        String nome = scanner.nextLine();
        System.out.print("Informe a sua idade: ");
        int idade = scanner.nextInt();
        System.out.println("Olá, " + nome + ", sua idade é " + idade);
    }
}


import java.util.Scanner;

public class AreaTriangulo {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Informe a base do triângulo: ");
        double base = scanner.nextDouble();
        System.out.print("Informe a altura do triângulo: ");
        double altura = scanner.nextDouble();
        double area = (base * altura) / 2;
        System.out.println("Área do triângulo: " + area);
    }
}


import java.util.Scanner;

public class PositivoNegativoNeutro {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Informe um valor: ");
        int valor = scanner.nextInt();

        if (valor > 0) {
            System.out.println("O valor é positivo.");
        } else if (valor < 0) {
            System.out.println("O valor é negativo.");
        } else {
            System.out.println("O valor é neutro.");
        }
    }
}


import java.util.Scanner;

public class MaiorDeTres {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Informe o primeiro valor: ");
        int a = scanner.nextInt();
        System.out.print("Informe o segundo valor: ");
        int b = scanner.nextInt();
        System.out.print("Informe o terceiro valor: ");
        int c = scanner.nextInt();

        int maior = (a > b && a > c) ? a : (b > c) ? b : c;
        System.out.println("O maior valor é: " + maior);
    }
}


import java.util.Scanner;
import java.util.Arrays;

public class SomaDosMaiores {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int[] valores = new int[3];

        for (int i = 0; i < 3; i++) {
            System.out.print("Informe o valor " + (i + 1) + ": ");
            valores[i] = scanner.nextInt();
        }

        Arrays.sort(valores);
        int soma = valores[1] + valores[2];
        System.out.println("A soma dos dois maiores valores é: " + soma);
    }
}


import java.util.Scanner;

public class Divisao {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Informe o primeiro valor: ");
        double primeiro = scanner.nextDouble();

        double segundo;
        do {
            System.out.print("Informe o segundo valor (não pode ser neutro ou negativo): ");
            segundo = scanner.nextDouble();
        } while (segundo <= 0);

        System.out.println("Resultado da divisão: " + (primeiro / segundo));
    }
}


import java.util.Scanner;

public class MediaDezValores {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        double soma = 0;

        for (int i = 1; i <= 10; i++) {
            System.out.print("Informe o valor " + i + ": ");
            soma += scanner.nextDouble();
        }

        System.out.println("Média aritmética: " + (soma / 10));
    }
}


import java.util.Scanner;

public class MediaAprovacao {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        double soma = 0;

        for (int i = 1; i <= 4; i++) {
            System.out.print("Informe a nota da avaliação " + i + ": ");
            soma += scanner.nextDouble();
        }

        double media = soma / 4;
        if (media >= 6.0) {
            System.out.println("PARABÉNS! Você foi aprovado!");
        } else {
            System.out.println("Infelizmente, você não foi aprovado.");
        }
    }
}


public class BombaRelogio {
    public static void main(String[] args) {
        for (int i = 30; i >= 0; i--) {
            System.out.println(i);
        }
        System.out.println("EXPLOSÃO!");
    }
}


