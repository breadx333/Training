112. Написать программу, которая выводит на экран ваше имя 10 раз.
```
#include <stdio.h>

int main()
{
    char name[] = {'E', 't', 'o', '\0'};

    for (int i = 0; i < 10; ++i) {
        printf("%s\n", name);
    }

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
113. Написать программу, которая выводит таблицу значений функции у = - 2,4х2 + 5х - 3 в диапазоне от -2 до 2, с шагом 0,5. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>

#define LB -2.0
#define HB 2.0
#define DX 0.5

int main()
{
    float x, y;
    int n;

    n = (HB-LB)/DX + 1;
    x = LB;

    printf("----------------------\n");
    printf("    x     |     y     \n");
    printf("----------------------\n");

    for (int i = 1; i <= n; ++i) {
        y = -2.4*x*x+5*x-3;
        printf("%+9.2f | %+9.2f\n", x, y);
        x += DX;
    }

    printf("----------------------\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
114. Написать программу, которая выводит таблицу квадратов первых десяти целых положительных чисел. Далее приведен рекомендуемый вид экрана программы.
```

int main()
{
    int x = 1;
    int y;

    printf("Square table\n");
    printf("----------------------\n");
    printf("Number square\n");
    printf("----------------------\n");

    for (int i = 1; i <= 10; ++i) {
        y = x*x;
        printf("%3i\t%4i\n", x, y);
        x += 1;
    }

    printf("----------------------\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
115. Написать программу, которая выводит таблицу квадратов первых пяти целых положительных нечетных чисел. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>

int main()
{
    int x = 1;
    int y;

    printf("Table of squares of odd numbers\n");
    printf("----------------------\n");
    printf("Number of square\n");
    printf("----------------------\n");

    for (int i = 1; i <= 10; ++i) {
        y = x * x;
        printf("%5i\t%5i\n", x, y);
        x += 2;
    }

    printf("----------------------\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
116. Написать программу, которая выводит таблицу скорости (через каждые 0,5 с) свободно падающего тела (v = gt, где g = 9,8 м/с2 — ускорение свободного падения). Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>

#define TSTEP 0.5

int main()
{
    const float G = 9.8;
    float time = 0;
    float V;

    printf("----------------------\n");
    printf("Time, sec Speed, m/sec\n");
    printf("----------------------\n");

    for (int i = 0; i < 10; ++i) {
        V = G * time;
        printf("%6.1f\t%6.2f\n", time, V);
        time += TSTEP;
    }

    printf("----------------------\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
117. Написать программу, которая выводит таблицу ежемесячных платежей по кредиту. Исходные данные для расчета: сумма кредита, срок и процентная ставка. Предполагается, что кредит возвращается (выплачивается) ежемесячно равными долями. Проценты начисляются ежемесячно на величину долга. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
