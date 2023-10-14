1) Faça um programa que leia um valor n, inteiro positivo, calcule e mostre a seguinte soma: s =1+ 1/2 + 1/3 + 1/4 +...+1/n.
   
#include <stdio.h>

int main() {
    int n;
    float soma = 0;

    printf("Insira um valor inteiro positivo para n: ");
    scanf("%d", &n);

    if (n > 0) {
        for (int i = 1; i <= n; i++) {
            soma += 1.0 / i;
        }
        printf("A soma é: %.2f\n", soma);
    } else {
        printf("Por favor, insira um valor inteiro positivo para n.\n");
    }

    return 0;
}

2) faça um programa que verifique e mostre os números entre 1000 e 2000 inclusive quando dividimos por 11. produzimos o resto igual a 5.

#include <stdio.h>

int main() {
    printf("Números entre 1000 e 2000 (inclusive) que têm resto 5 quando divididos por 11:\n");

    for (int num = 1000; num <= 2000; num++) {
        if (num % 11 == 5) {
            printf("%d\n", num);
        }
    }

    return 0;
}

3) Faça um programa que mostre as tabuadas dos números de 1 a 10.

   #include <stdio.h>

int main() {
    int idade, cont_maior_ou_igual_18 = 0;

    for (int i = 0; i < 10; i++) {
        printf("Digite a idade da pessoa %d: ", i + 1);
        scanf("%d", &idade);

        if (idade >= 18) {
            cont_maior_ou_igual_18++;
        }
    }

    printf("Quantidade de pessoas com 18 anos ou mais: %d\n", cont_maior_ou_igual_18);

    return 0;
}

4) Faça um programa que receba a idade de dez pessoas e que calcule e mostre a quantidade de pessoas com idade maior ou igual a 18 anos.

#include <stdio.h>

int main() {
    int idade, cont_maior_ou_igual_18 = 0;

    for (int i = 0; i < 10; i++) {
        printf("Digite a idade da pessoa %d: ", i + 1);
        scanf("%d", &idade);

        if (idade >= 18) {
            cont_maior_ou_igual_18++;
        }
    }

    printf("Quantidade de pessoas com 18 anos ou mais: %d\n", cont_maior_ou_igual_18);

    return 0;
}

5) Faça um programa que receba um número e que calcule e mostre a tabela desse número.

#include <stdio.h>

int main() {
    int numero;

    printf("Insira um número para calcular a tabuada: ");
    scanf("%d", &numero);

   
    printf("Tabuada do %d:\n", numero);

    for (int i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", numero, i, numero * i);
    }

    return 0;
}
