157. Написать программу, которая записывает введенные с клавиатуры данные в одномерный массив целого типа, состоящий из семи элементов. Перед вводом каждого элемента должна выводиться подсказка с номером элемента. После ввода последнего элемента программа должна вывести введенный массив и вычислить среднее арифметическое его элементов. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int a[7] = {};
    int sum;
    float m;
    int j;

    printf("Enter integer to massive\n");

    for (j = 0; j < 7; j++) {
        printf("a[%i] = ", j);
        scanf("%i", &a[j]);
    }

    for (j = 0; j < 7; ++j) {
        printf("%i ", a[j]);
    }

    sum = 0;

    for (j = 0; j < 7; ++j) {
        sum += a[j];
    }

    m = sum / 7;

    printf("Sum: %i\n", sum);
    printf("Avg. mean: %.2f\n", m);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
158. Написать программу, которая вводит с клавиатуры данные в одномерный массив дробного типа, состоящий из пяти элементов, после чего выводит количество ненулевых элементов. Перед вводом каждого элемента должна выводиться подсказка с номером элемента. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE] = {};
    int n = 0;
    int i;

    printf("Enter array of integer numbers\n");

    for (i = 0; i < SIZE; ++i) {
        printf("a[%i] = ", i);
        scanf("%i", &a[i]);
        if (a[i] != 0) ++n;
    }

    printf("In array %i non zero elements\n", n);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
159. Написать программу, которая выводит минимальный элемент введенного с клавиатуры массива целых чисел. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE];
    int minimum;
    int i;

    printf("Find minimum element of array\n");
    printf("Enter data in one line\n-> ");

    for (i = 0; i < SIZE; ++i) {
        scanf("%i", &a[i]);
    }

    minimum = 0;

    for (i = 1; i < SIZE; ++i) {
        if (a[i] < a[minimum]) minimum = i;
    }

    printf("Minimal element of array: a[%i]=%i ", minimum+1, a[minimum]);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
160. Написать программу, которая выводит минимальный элемент введенного с клавиатуры массива целых чисел. Для доступа к элементам массива используйте указатель.
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE];
    int *minimum;
    int *p;
    int i;

    printf("Find minimum element of array\n");
    printf("Enter data in one line\n-> ");

    p = a;

    for (i = 1; i <= SIZE; ++i) {
        scanf("%i", p++);
    }

    minimum = a;
    p = a + 1;

    for (i = 2; i <= SIZE; ++i) {
        if (*p < *minimum) minimum = p;
        ++p;
    }

    printf("Minimal element of array: %i\n", *minimum);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
161. Написать программу, которая вычисляет среднее арифметическое ненулевых элементов введенного с клавиатуры массива целых чисел. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

#define SIZE 10

int main()
{
    int a[SIZE] = {};
    int sum = 0;
    float avg = 0;
    int n = 0;
    int i;

    printf("Enter array of integer numbers\n");

    for (i = 0; i < SIZE; ++i) {
        printf("a[%i] = ", i);
        scanf("%i", &a[i]);
        if (a[i] != 0) {
            sum += a[i];
            ++n;
        }
    }

    avg = sum / n;

    printf("Sum: %i\n", sum);
    printf("In array %i non zero elements\n", n);
    printf("Avg. Mean: %.2f\n", avg);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
162. Написать программу, которая вычисляет среднее арифметическое элементов массива без учета минимального и максимального элементов массива. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
