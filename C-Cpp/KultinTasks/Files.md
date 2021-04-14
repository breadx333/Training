233. Написать программу, которая создает на диске файл numbers.txt и записывает в него 5 целых чисел, введенных пользователем с клавиатуры. Откройте созданный программой файл и убедитесь, что каждое число находится в отдельной строке.
```
#include <stdio.h>

#define FNAME "numbers.txt"
#define N 5

int main()
{
    char fname[40] = FNAME;
    FILE *f;
    int n;

    if ((f = fopen(fname, "wt")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    for (int i = 0; i < N; ++i) {
        printf("-> ");
        scanf("%i", &n);
        fprintf(f, "%i\n", n);
        fflush(stdin);
    }
    fclose(f);
    printf("Entered: %s\n", fname);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
234. Написать программу, которая дописывает в файл numbers.txt три целых числа, введенных пользователем. Убедитесь, открыв файл при помощи редактора текста, что в файле находятся 8 чисел.
```
#include <stdio.h>

#define FNAME "numbers.txt"
#define N 3

int main()
{
    char fname[40] = FNAME;
    FILE *f;
    int n;

    if ((f = fopen(fname, "at")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    for (int i = 0; i < N; ++i) {
        printf("-> ");
        scanf("%i", &n);
        fprintf(f, "%i\n", n);
        fflush(stdin);
    }
    fclose(f);
    printf("Entered: %s\n", fname);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
235. Написать программу, которая выводит на экран содержимое файла numbers.txt.
```
#include <stdio.h>

#define FNAME "numbers.txt"
#define N 3

int main()
{
    char fname[40] = FNAME;
    FILE *f;
    char st[80];

    if ((f = fopen(fname, "rt")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    while (!feof(f)) {
        fscanf(f, "%s", &st);
        printf("%s\n", st);
    }
    fclose(f);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
236. Написать программу, которая вычисляет среднее арифметическое чисел, находящихся в файле numbers.txt.
```
#include <stdio.h>

#define FNAME "numbers.txt"
#define N 3

int main()
{
    char fname[40] = FNAME;
    FILE *f;

    int a;
    int n = 0;
    int sum = 0;
    float sr;

    if ((f = fopen(fname, "rt")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    while (!feof(f)) {
        fscanf(f, "%i", &a);
        sum += a;
        ++n;
    }
    fclose(f);

    sr = (float)sum/n;
    printf("Entered: %i nums\n", n);
    printf("Sum: %i\n", sum);
    printf("Avg. mean: %3.2f\n", sr);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
237. Написать программу, которая записывает в файл данные, находящиеся в двумерном массиве дробного типа.
```
#include <stdio.h>
#include <string.h>

#define NR 3
#define NC 6

int main()
{
    float a[NR][NC] = {15.0, 16.5, 18.0, 19.5, 21.0, 24.0,
                       16.5, 18.0, 19.5, 21.0, 22.5, 24.0,
                       18.0, 19.5, 21.0, 22.5, 24.0, 27.0};
    FILE *f;
    int r, c;

    for (r = 0; r < NR; ++r) {
        for (c = 0; c < NC; ++c) {
            printf("%5.2f\t", a[r][c]);
        }
        printf("\n");
    }

    if ((f = fopen("nubers.txt", "wt")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    for (r = 0; r < NR; ++r) {
        for (c = 0; c < NC; ++c) {
            fprintf(f, "%5.2f ", a[r][c]);
        }
        if (r != NR-1)
            fprintf(f, "\n");
    }
    fclose(f);
    printf("Data was writed\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
238. Написать программу, которая загружает из файла данные в двумерный массив дробного типа.
```
#include <stdio.h>
#include <string.h>

#define NR 3
#define NC 6

int main()
{
    float a[NR][NC];
    FILE *f;
    int r, c;

    if ((f = fopen("nubers.dat", "rt")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    for (r = 0; r < NR; ++r) {
        for (c = 0; c < NC; ++c) {
            fscanf(f, "%f", &a[r][c]);
        }
    }
    fclose(f);

    for (r = 0; r < NR; ++r) {
        for (c = 0; c < NC; ++c) {
            printf("%7.2f ", a[r][c]);
        }
        printf("\n");
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
239. Написать программу, которая позволяет просматривать текстовые файлы (выводит на экран их содержимое)— например, файлы исходных программ C/C++. Имя просматриваемого файла должно вводиться пользователем во время работы программы. 
```
