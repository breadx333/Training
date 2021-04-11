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
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE] = {};
    int mn;
    int mx;
    int n = 0;
    int sum = 0;
    int avg = 0;

    for (int i = 0; i < SIZE; ++i) {
        printf("a[%i] = ", i);
        scanf("%i", &a[i]);
    }

    mn = a[0];
    mx = a[0];

    for (int i = 0; i < SIZE; ++i) {
        if (a[i] > mx) mx = a[i];
        if (a[i] < mn) mn = a[i];
    }

    for (int i = 0; i < SIZE; ++i) {
        if (a[i] != mn && a[i] != mx) {
            sum += a[i];
            ++n;
        }
    }

    printf("Min: %i\n", mn);
    printf("Max: %i\n", mx);
    printf("Avg. mean %i elements: %.2f\n", n, (float)sum/n);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
163. Написать программу, которая вычисляет среднюю (за неделю) температуру воздуха. Исходные данные должны вводиться во время работы программы. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    char *day[] = {"1", "2", "3", "4", "5", "6", "7"};

    float t[7];
    float sum;
    float avg;

    for (int i = 0; i < 7; ++i) {
        printf("%s day -> ", day[i]);
        scanf("%f", &t[i]);
        sum += t[i];
    }

    avg = sum / 7;

    printf("Avg. temperature: %.2f\n", avg);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
164. Написать программу, которая проверяет, находится ли введенное с клавиатуры число в массиве. Массив должен вводиться в процессе работы программы.
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int m[SIZE];
    int exemplar;
    int found;
    int i;

    printf("-> ");
    for (i = 0; i < SIZE; ++i) {
        scanf("%i", &m[i]);
    }
    printf("-> ");
    scanf("%i", &exemplar);

    found = 0;
    i = 0;
    do {
        if (m[i] == exemplar)
            found = 1;
        else ++i;
    } while (!found && i < SIZE);

    if (found)
        printf("%i\n", i+1);
    else
        printf("Not found\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
165. Написать программу, которая проверяет, представляют ли элементы введенного с клавиатуры массива возрастающую последовательность.
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE];
    int i;
    int ok;

    printf("Enter %i numbers in one line -> ", SIZE);

    for (i = 0; i < SIZE; ++i) {
        scanf("%i", &a[i]);
    }

    i = 0;
    ok = 1;
    do {
        if (a[i] > a[i+1])
            ok = 0;
        ++i;
    } while (i < SIZE-1 && ok);

    if (!ok)
        printf("No\n");
    else printf("Yes\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
166. Написать программу, которая вычисляет, сколько раз введенное с клавиатуры число встречается в массиве.
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE];
    int sample;
    int n;
    int i;

    printf("-> ");
    for (i = 0; i < SIZE; ++i) {
        scanf("%i", &a[i]);
    }
    printf("-> ");
    scanf("%i", &sample);
    n = 0;
    for (i = 0; i < SIZE; ++i) {
        if (a[i] == sample) ++n;
    }
    if (n)
        printf("%i meets in array %i\n", sample, n);
    else printf("Not found\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
167. Написать программу, которая проверяет, есть ли во введенном с клавиатуры массиве элементы с одинаковым значением.
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE];
    bool ok = true;

    for (int i = 0; i < SIZE; ++i) {
        printf("-> ");
        scanf("%i", &a[i]);
    }

    for (int i = 0; i < SIZE - 1; ++i) {
        if (a[i] != a[i+1]) {
            ok = false;
            break;
        }
    }

    if (ok) {
        printf("Yep\n");
    }
    else printf("No\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
168. Написать программу, которая методом прямого выбора сортирует по убыванию введенный с клавиатуры одномерный массив.
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE];
    int i;

    int mn;

    int j;
    int buf;
    int k;

    for (k = 0; k < SIZE; ++k) {
        printf("-> ");
        scanf("%i", &a[k]);
    }

    for (i = 0; i < SIZE - 1; ++i) {
        mn = i;
        for (j = i+1; j < SIZE; ++j) {
            if (a[j] < a[mn]) mn = j;
        }
        buf = a[i];
        a[i] = a[mn];
        a[mn] = buf;

        for (k = 0; k < SIZE; ++k)
            printf("%i ", a[k]);
        printf("\n");
    }

    for (k = 0; k < SIZE; ++k)
        printf("%i ", a[k]);
    printf("\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
169. Написать программу, которая методом обмена («пузырька») сортирует по убыванию введенный с клавиатуры одномерный массив.
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE];
    int i;
    int k;
    int buf;

    printf("-> ");
    for (i = 0; i < SIZE; ++i)
        scanf("%i", &a[i]);

    for (i = 0; i < SIZE - 1; ++i) {
        for (k = 0; k < SIZE - 1; ++k) {
            if (a[k] > a[k+1]) {
                buf = a[k];
                a[k] = a[k+1];
                a[k+1] = buf;
            }
        }
        for (k = 0; k < SIZE; ++k)
            printf("%i ", a[k]);
        printf("\n");
    }

    for (k = 0; k < SIZE; ++k)
        printf("%i ", a[k]);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
170. Написать программу, которая объединяет два упорядоченных по возрастанию массива в один, который также должен быть упорядочен по возрастанию. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE], b[SIZE];
    int c[SIZE*2];
    int k, i, m;

    printf("-> ");
    for (k = 0; k < SIZE; ++k)
        scanf("%i", &a[k]);

    printf("-> ");
    for (k = 0; k < SIZE; ++k)
        scanf("%i", &b[k]);

    for (int d = 0; d < SIZE; ++d)
        printf("%i ", a[d]);
    printf("\n");

    for (int d = 0; d < SIZE; ++d)
        printf("%i ", b[d]);
    printf("\n");

    k = i = m = 0;

    do {
        if (a[k] < b[i])
            c[m++] = a[k++];
        else
            if (a[k] > b[i])
                c[m++] = b[i++];
            else {
                c[m++] = a[k++];
                c[m++] = b[i++];
            }
    } while (k < SIZE && i < SIZE);

    while (k < SIZE)
        c[m++] = a[k++];

    while (i < SIZE)
        c[m++] = b[i++];

    for (i = 0; i < 2 * SIZE; ++i)
        printf("%i ", c[i]);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
171. Написать программу, которая, используя метод бинарного поиска, выполняет поиск в упорядоченном по возрастанию массиве.
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int a[SIZE];
    int obr;
    int ok;

    int verh, niz;

    int sred;
    int found;
    int n;
    int i;

    printf("-> ");
    for (i = 0; i < SIZE; ++i)
        scanf("%i", &a[i]);

    ok = 1;
    i = 0;

    do {
        if (a[i] <= a[i+1])
            ++i;
        else ok = 0;
    } while (ok && i < SIZE - 1);

    if (!ok) {
        puts("ii\n");
        goto bye;
    }

    printf("-> ");
    scanf("%i", &obr);

    verh = 0;
    niz = SIZE - 1;
    found = 0;
    n = 0;
    do {
        sred = (niz-verh) / 2 + verh;
        ++n;
        if (a[sred] == obr)
            found = 1;
        else
        if (obr < a[sred])
            niz = sred-1;
        else verh = sred+1;
    } while (verh <= niz && !found);

    if (found) {
        printf("element %i ", sred);
        printf("Com %i", n);
    }
    else printf("Not found\n");

    bye:

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
172. Написать программу, которая определяет количество учеников в классе, чей рост превышает средний. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

#define SIZE 5

int main()
{
    int r;
    int rost[SIZE];
    int n = 0;

    float sred;
    int m = 0;

    int sum = 0;
    int i = 0;

    do {
        printf("-> ");
        scanf("%i", &r);
        if (r) {
            rost[i++] = r;
            sum += r;
            ++n;
        }
    } while (r && i < SIZE);

    if (n) {
        sred = (float)sum / n;
        m = 0;
        for (i = 0; i < n; ++i)
            if (rost[i] > sred) ++m;
        printf("Avg. H: %3.2f\n", sred);
        printf("%i b\n", m);
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
173. Написать программу, которая вводит по строкам с клавиатуры двумерный массив и вычисляет сумму его элементов по столбцам.
```
