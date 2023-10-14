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
Insira um valor inteiro positivo para n: 2
A soma é: 1.50

2) Faça um programa que verifique e mostre os números entre 1000 e 2000 inclusive quando dividimos por 11. produzimos o resto igual a 5.
   
int main() {
    printf("Números entre 1000 e 2000 (inclusive) que têm resto 5 quando divididos por 11:\n");

    for (int num = 1000; num <= 2000; num++) {
        if (num % 11 == 5) {
            printf("%d\n", num);
        }
    }

    return 0;
}

Números entre 1000 e 2000 (inclusive) que têm resto 5 quando divididos por 11:
1006
1017
1028
1039
1050
1061
1072
1083
1094
1105
1116
1127
1138
1149
1160
1171
1182
1193
1204
1215
1226
1237
1248
1259
1270
1281
1292
1303
1314
1325
1336
1347
1358
1369
1380
1391
1402
1413
1424
1435
1446
1457
1468
1479
1490
1501
1512
1523
1534
1545
1556
1567
1578
1589
1600
1611
1622
1633
1644
1655
1666
1677
1688
1699
1710
1721
1732
1743
1754
1765
1776
1787
1798
1809
1820
1831
1842
1853
1864
1875
1886
1897
1908
1919
1930
1941
1952
1963
1974
1985
1996

3) Faça um programa que mostre as tabuadas dos números de 1 a 10.
   
#include <stdio.h>

int main() {
    int i, j;

    
    for (i = 1; i <= 10; i++) {
        printf("Tabuada do %d:\n", i);

        for (j = 1; j <= 10; j++) {
            printf("%d x %d = %d\n", i, j, i * j);
        }

        printf("\n");
    }

    return 0;
}

Tabuada do 1:
1 x 1 = 1
1 x 2 = 2
1 x 3 = 3
1 x 4 = 4
1 x 5 = 5
1 x 6 = 6
1 x 7 = 7
1 x 8 = 8
1 x 9 = 9
1 x 10 = 10

Tabuada do 2:
2 x 1 = 2
2 x 2 = 4
2 x 3 = 6
2 x 4 = 8
2 x 5 = 10
2 x 6 = 12
2 x 7 = 14
2 x 8 = 16
2 x 9 = 18
2 x 10 = 20

Tabuada do 3:
3 x 1 = 3
3 x 2 = 6
3 x 3 = 9
3 x 4 = 12
3 x 5 = 15
3 x 6 = 18
3 x 7 = 21
3 x 8 = 24
3 x 9 = 27
3 x 10 = 30

Tabuada do 4:
4 x 1 = 4
4 x 2 = 8
4 x 3 = 12
4 x 4 = 16
4 x 5 = 20
4 x 6 = 24
4 x 7 = 28
4 x 8 = 32
4 x 9 = 36
4 x 10 = 40

Tabuada do 5:
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50

Tabuada do 6:
6 x 1 = 6
6 x 2 = 12
6 x 3 = 18
6 x 4 = 24
6 x 5 = 30
6 x 6 = 36
6 x 7 = 42
6 x 8 = 48
6 x 9 = 54
6 x 10 = 60

Tabuada do 7:
7 x 1 = 7
7 x 2 = 14
7 x 3 = 21
7 x 4 = 28
7 x 5 = 35
7 x 6 = 42
7 x 7 = 49
7 x 8 = 56
7 x 9 = 63
7 x 10 = 70

Tabuada do 8:
8 x 1 = 8
8 x 2 = 16
8 x 3 = 24
8 x 4 = 32
8 x 5 = 40
8 x 6 = 48
8 x 7 = 56
8 x 8 = 64
8 x 9 = 72
8 x 10 = 80

Tabuada do 9:
9 x 1 = 9
9 x 2 = 18
9 x 3 = 27
9 x 4 = 36
9 x 5 = 45
9 x 6 = 54
9 x 7 = 63
9 x 8 = 72
9 x 9 = 81
9 x 10 = 90

Tabuada do 10:
10 x 1 = 10
10 x 2 = 20
10 x 3 = 30
10 x 4 = 40
10 x 5 = 50
10 x 6 = 60
10 x 7 = 70
10 x 8 = 80
10 x 9 = 90
10 x 10 = 100

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

Digite a idade da pessoa 1: 12
Digite a idade da pessoa 2: 29
Digite a idade da pessoa 3: 19
Digite a idade da pessoa 4: 18
Digite a idade da pessoa 5: 10
Digite a idade da pessoa 6: 17
Digite a idade da pessoa 7: 40
Digite a idade da pessoa 8: 22
Digite a idade da pessoa 9: 31
Digite a idade da pessoa 10: 25
Quantidade de pessoas com 18 anos ou mais: 7

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

Insira um número para calcular a tabuada: 5
Tabuada do 5:
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
