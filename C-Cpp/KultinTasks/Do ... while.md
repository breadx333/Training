145. Написать программу, которая выводит на экран таблицу значений функции у = -2,4х2+ 5х-3. Диапазон и шаг изменения аргумента должны задаваться во время работы программы. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>

int main()
{
    float x, y;
    float x1, x2, dx;

    printf("x1 -> ");
    scanf("%f", &x1);
    printf("x2 -> ");
    scanf("%f", &x2);
    printf("dx -> ");
    scanf("%f", &dx);

    x = x1;
    printf("-----------------------\n");
    printf("     x     |      y    \n");
    printf("-----------------------\n");
    do {
        y = -2.4*x*x+5*x-3;
        printf("%9.2f  | %9.2f\n", x, y);
        x += dx;
    }
    while (x <= 2);

    printf("-----------------------\n");

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
146. Написать программу, которая выводит на экран таблицу соответствия температуры в градусах Цельсия и Фаренгейта (7?°= 5/9 С°+32). Диапазон изменения температуры в градусах Цельсия и шаг должны вводиться во время работы программы. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float t1, t2, dt;
    float c, f;

    printf("t1 -> ");
    scanf("%f", &t1);
    printf("t2 -> ");
    scanf("%f", &t2);
    printf("dt -> ");
    scanf("%f", &dt);

    c = t1;
    printf("-----------------------\n");
    printf("     C     |      F    \n");
    printf("-----------------------\n");
    do {
        f = 9.0/5 * c + 32;
        printf("%9.2f  | %9.2f\n", c, f);
        c += dt;
    }
    while (c <= t2);

    printf("-----------------------\n");

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
147. Написать программу, вычисляющую сумму и среднее арифметическое последовательности положительных чисел, которые вводятся с клавиатуры. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int a;
    int n;
    int s;
    float m;

    s = 0;
    n = 0;

    printf("Calculating Avg. mean\n");
    printf("Enter numbers. To complete press <Enter>\n");

    do {
        printf("-> ");
        scanf("%i", &a);
        if (a > 0) {
            s += a;
            ++n;
        }
    }
    while (a > 0);

    printf("Numbers Entered: %i\n", n);
    printf("Sum of numbers: %i\n", s);
    m = (float) s / n;
    printf("Avg. Mean: %3.2f\n", m);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
148. Написать программу, которая определяет максимальное число из введенной с клавиатуры последовательности положительных чисел (длина последовательности не ограничена). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int a;
    int m;

    puts("Defines max number\n");
    puts("Enter numbers; To complete enter 0\n");
    m = 0;
    do {
        printf("-> ");
        scanf("%i", &a);
        if (a > m)
            m = a;
    }
    while (a > 0);
    printf("Max number: %i\n", m);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
149. Написать программу, которая определяет минимальное число во введенной с клавиатуры последовательности положительных чисел (длина последовательности не ограничена). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int a;
    int minimum;

    printf("Defines minimum number\n");
    printf("Enter numbers. To complete enter 0\n");
    printf("-> ");
    scanf("%i", &a);
    minimum = a;
    while (a > 0) {
        if (a < minimum) minimum = a;
        printf("-> ");
        scanf("%i", &a);
    }
    printf("Minimum number: %i\n", minimum);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
150. Написать программу, которая проверяет, является ли введенное пользователем целое число простым (простым называется число, которое делится только на единицу и на само себя). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int n;
    int d;
    int r;

    printf("Enter whole number and press <Enter>\n-> ");
    scanf("%i", &n);
    d = 2;
    do {
        r = n % d;
        if (r != 0) ++d;
    }
    while (r != 0);
    if (d == n)
        printf("%i - simply number\n", n);
    else printf("%i - not simply number\n", n);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
151. Написать программу приближенного вычисления интеграла методом прямоугольников. Интервал и точность вычисления должны задаваться во время работы программы, функция — в программе. После каждого цикла вычислений программа должна выводить вычисленное значение интеграла.
```
#include <stdio.h>
#include <math.h>

int main()
{
    float x1, x2;
    float e;

    float dx;
    float n;
    float x;
    float y;
    float st;
    float sp;

    int i;

    printf("Calculating integral\n");
    printf("Low edge -> ");
    scanf("%f", &x1);
    printf("Up edge -> ");
    scanf("%f", &x2);

    printf("Accuracy - > ");
    scanf("%f", &e);

    dx = 0.5;
    st = 0;

    do {
        sp = st;
        dx = dx / 2;
        n = (x2 - x1) / dx;
        x = x1;
        st = 0;
        for (i = 0; i <= n; ++i) {
            y = x + 2;
            st = st + (y * dx);
            x += dx;
        }
        printf("Value of integral: %6.3f\n", st);
    }
    while (abs(sp - st) > e);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
152. Написать программу, которая «задумывает» число в диапазоне от 1 до 10 и предлагает пользователю угадать его за пять попыток. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
#include <conio.h>

int main()
{
    int comp;
    int player;
    int n;
    time_t t;

    srand((unsigned) time(&t));
    comp = rand() % 10 + 1;

    system("cls");
    printf("Computer number 1...10\n\r");
    printf("You should guess in 5 try\n");
    printf("Enter number and press <Enter>\n");
    n = 0;
    do {
        printf("\n\r-> ");
        scanf("%i", &player);
        ++n;
    }
    while ((player != comp) && (n < 3));

    if (player == comp) {
        printf("\n\rYou Win! Congratulations!");
    }
    else {
        printf("\n\rYou Lose");
        printf("PC think number %d", comp);
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
153. Написать программу приближенного вычисления интеграла методом трапеций. Интервал и точность вычисления должны задаваться во время работы программы. После каждого цикла вычислений программа должна выводить вычисленное значение интеграла, число интервалов и шаг изменения аргумента.
```
```
