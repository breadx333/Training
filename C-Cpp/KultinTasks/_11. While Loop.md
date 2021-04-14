154. Написать программу, которая выводит на экран таблицу значения функции у - 2х2 - 5т - 8 в диапазоне от -4 до 4. Шаг изменения аргумента равен 0,5.
```
#include <stdio.h>

int main()
{
    float x, dx;
    float x1, x2;
    float y;

    x1 = -4;
    x2 = 4;
    dx = 0.5;
    x = x1;
    printf("-----------------------\n");
    printf("     x     |     y     \n");
    printf("-----------------------\n");
    while (x < x2) {
        y = x*x + 2;
        printf("%9.2f  | %9.2f\n", x, y);
        x += dx;
    }
    printf("-----------------------\n");

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
155. Написать программу, которая вычисляет число «Пи» с заданной пользователем точностью. Для вычисления числа л воспользуйтесь тем, что значение частичной суммы ряда 1 - 1/3 + 1/5 - 1/7 + 1/9 ..., при суммировании достаточно большого количества членов, приближается к я/4. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float p;
    float t;
    int n;
    float el;

    p = 0;
    n = 1;
    el = 1;
    printf("Enter accuracy for calculating PI -> ");
    scanf("%f", &t);
    while (el >= t) {
        el = (float) 1 / (2*n - 1);
        if ((n%2) == 0)
            p -= el;
        else p += el;
        ++n;
    }
    p = p*4;
    printf("Value PI with Acc. %f eval %f\n", t, p);
    printf("Summ Cnt %i\n", n);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
156. Написать программу, которая вычисляет наибольший общий делитель двух целых чисел.
```
#include <stdio.h>

int main()
{
    int n1, n2;
    int nod;
    int r;

    printf("Calculating max divine\n");
    printf("For two numbers\n");
    printf("Enter two nums in one line\n-> ");
    scanf("%i%i", &n1, &n2);
    printf("MDN of numbers %i and %i - is ", n1, n2);
    while (n1 % n2) {
        r = n1 % n2;
        n1 = n2;
        n2 = r;
    }
    nod = n2;
    printf("%i\n", nod);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
