245. Написать рекурсивную функцию вычисления факториала и программу, проверяющую ее работу.
```
#include <stdio.h>
#include <conio.h>
#include <string.h>

unsigned factor(unsigned k) {
    if (k == 1)
        return 1;
    else
        return (k*factor(k-1));
}

int main(int argc, char *argv[])
{
    unsigned n;
    unsigned f;

    printf("-> ");
    scanf("%u", &n);
    f = factor(n);
    printf("Factorial of number %u: %u\n", n, f);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
246. Написать рекурсивную функцию вычисления числа Фибоначчи и программу, проверяющую ее работу.
```
#include <stdio.h>
#include <conio.h>
#include <string.h>

int Fibonacci(int n) {
    if ((n == 0) || (n == 1))
        return 1;
    else
        return Fibonacci(n - 2) + Fibonacci(n - 1);
}

int main(int argc, char *argv[])
{
    for (int n = 0; n < 21; ++n) {
        printf("%i ", Fibonacci(n));
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
247. Программа демонстрирует применение рекурсии для решения задачи поиска — в частности, поиска пути на графе. Для представления графа используется массив.
```
НЕ РАБОЧИЙ КОД, А ВООБЩЕ МНОЖЕСТВО КОДОВ В КНИГЕ НЕ РАБОЧИЕ, ХОТЯ ОНА ВЫПУЩЕНА В 2019, ЧТО СТРАННО, ПРИХОДИТЬСЯ ИСПРАВЛЯТЬ КОД АВТОРА, А ПОКА Я УСТАЛ
```
```
#include <stdio.h>
#include <conio.h>
#include <string.h>

#define N 7

int mp[N][N] = {{0, 1, 1, 1, 0, 0, 0},
                {1, 0, 0, 0, 0, 0, 0},
                {1, 0, 0, 1, 0, 0, 1},
                {1, 0, 1, 0, 0, 1, 0},
                {0, 0, 0, 0, 0, 1, 1},
                {0, 0, 0, 1, 1, 0, 1},
                {0, 0, 1, 0, 1, 1, 0}};

int road[N] = {-1, -1, -1, -1, -1, -1, -1};

void step(int s, int f, int p) {
    if (s == f) {
        printf("\nPath:");
        for (int i = 0; i < N; ++i)
            if (road[i] != -1)
                printf("%i", road[i]);
        printf("\n");
    }
    else
    for (int c = 0; c < N; ++c) {
        if ((mp[s][c] != 0) && (inRoad[c] == 0)) {
            road[p] = c;
            inRoad[c] = 1;
            step(c, f, p+1);
            
            road[p] = -1;
            inRoad[c] = 0;
        }
    }
}

int main(int argc, char *argv[]) {
    int start = 2;
    int finish = 6;
    
    road[0] = start;
    inRoad[start] = 1;
    
    printf("From %i to %i \nSearch...\n", start, finish);
    
    step(start, finish, 1);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
