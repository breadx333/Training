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
#include <stdio.h>

int main()
{
    float amount;
    float term;
    float rate;

    float dept;
    float interest;
    float paying;
    float suminterest;

    printf("Amount -> ");
    scanf("%f", &amount);
    printf("Term -> ");
    scanf("%f", &term);
    printf("Interest rate -> ");
    scanf("%f", &rate);

    dept = amount;
    suminterest = 0;

    printf("----------------------\n");
    printf("Debt Interest Payment \n");
    printf("----------------------\n");

    for (int i = 1; i <= term; ++i) {
        interest = dept * (rate/12/100);
        suminterest += interest;
        paying = amount/term + interest;
        printf("%2i  %9.2f %9.2f %9.2f\n", i, dept, interest, paying);
        dept = dept - amount/term;
    }

    printf("----------------------\n");
    printf("Total percent: %3.2f\n", suminterest);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
118. Написать программу, которая выводит на экран таблицу соответствия температуры в градусах Цельсия и Фаренгейта (F°= 5/9-С°+32). Диапазон изменения температуры в градусах Цельсия и шаг должны вводиться во время работы программы. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float t1, t2, dt;
    float c, f;
    int n;

    printf("T1 -> ");
    scanf("%f", &t1);
    printf("T2 -> ");
    scanf("%f", &t2);
    printf("Step -> ");
    scanf("%f", &dt);

    n = (t2-t1)/dt + 1;
    c = t1;

    printf("----------------------\n");
    printf("     C          F     \n");
    printf("----------------------\n");

    for (int i = 0; i < n; ++i) {
        f = 9/5 * c + 32;
        printf("%9.2f %9.2f\n", c, f);
        c = c + dt;
    }

    printf("----------------------\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
119. Написать программу, которая выводит на экран таблицу перевода длины из дюймов в миллиметры (1 дюйм = 2,54 см). Диапазон длины в дюймах и шаг изменения должны вводиться во время работы программы.
```
#include <stdio.h>

int main()
{
    float in1, in2, dt;
    float mm;
    int n;

    printf("Inch1 -> ");
    scanf("%f", &in1);
    printf("Inch2 -> ");
    scanf("%f", &in2);
    printf("Step - > ");
    scanf("%f", &dt);

    printf("----------------------\n");
    printf("     IN        MM     \n");
    printf("----------------------\n");

    n = (in2 - in1) / dt;

    for (int i = 0; i < n; ++i) {
        mm = in1 * 2.54 * 100;
        printf("%9.2f %9.2f\n", in1, mm);
        in1 += dt;
    }

    printf("----------------------\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
120. Написать программу, которая вычисляет сумму первых п положительных целых чисел. Количество суммируемых чисел должно вводиться во время работы программы. Далее приведен рекомендуемый вид экрана (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int n;
    int summ;
    int i;

    printf("Sum of positive numbers\n");
    printf("Enter the number of numbers to add -> ");
    scanf("%i", &n);

    summ = 0;

    for (i = 1; i <= n; ++i) {
        summ = summ + i;
    }

    printf("The sum of the first %i positive numbers is %i\n", n, summ);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
121. Написать программу, которая вычисляет сумму первых п целых положительных четных чисел. Количество суммируемых чисел должно вводиться во время работы программы. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int start;
    int n;
    int sum;

    printf("Calculating the sum of even positive numbers\n");
    printf("Enter the number of numbers to add -> ");
    scanf("%i", &n);

    start = 2;
    sum = 0;

    for (int i = 0; i < n; ++i) {
        sum += start;
        start += 2;
    }

    printf("The sum of the first %i positive even numbers is %i\n", n, sum);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
122. Написать программу, которая вычисляет сумму первых « членов ряда: 1, 3, 5, 7 ... Количество суммируемых членов ряда задается во время работы программы. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int e;
    int n;
    int sum = 0;

    printf("Calculation of the partial sum of the series: 1,3,6,9, ...\n");
    printf("Enter the number of summed members of the series -> ");
    scanf("%i", &n);

    e = 1;

    for (int i = 1; i <= n; ++i) {
        sum += e;
        e += 3;
    }

    printf("The sum of the first %i members of the series is %i\n", n, sum);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
123. Написать программу, которая вычисляет сумму первых я членов ряда: 1+1/2+1/3+1/4... Количество суммируемых членов
ряда задается во время работы программы. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int n;
    float sum;
    float elem;

    printf("Calculation of the partial sumd of a series: 1 + 1/2 + 1/3 + ...\n");
    printf("Enter the number of summed members of the series -> ");
    scanf("%i", &n);

    sum = 0;

    for (int i = 1; i <= n; ++i) {
        elem = 1.0 / i;
        sum += elem;
    }

    printf("He sum of the first %i members of the series is %.4f\n", n, sum);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
124. Написать программу, которая выводит таблицу степеней двойки: от нулевой до десятой. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>

int main()
{
    int x;

    printf("Table Degrees Twos\n");
    
    x = 1;

    for (int n = 0; n <= 10; ++n) {
        printf("%3i%5i\n", n, x);
        x *= 2;
    }

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
125. Написать программу, которая вычисляет факториал введенного с клавиатуры числа. (Факториалом числа п называется произведение целых чисел от 1 до п. Например, факториал 1 равен 1, факториал 8 — 40 320).
```
#include <stdio.h>

int main()
{
    int number;
    int sum;

    printf("Calculating factorial\n");
    printf("Enter the number whose factorial you want to calculate -> ");
    scanf("%i", &number);

    sum = 1;

    for (int i = 1; i <= number; ++i) {
        sum *= i;
    }

    printf("Factorial %i is %i\n", number, sum);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
126. Написать программу, которая вводит с клавиатуры пять дробных чисел и вычисляет их среднее арифметическое. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным)
```
#include <stdio.h>

int main()
{
    int n = 5;
    float number;
    float sum = 0;
    float arithmetic_mean;

    printf("The arithmetic mean of a sequence of fractional numbers\n");
    printf("After entering each number\n");

    for (int i = 0; i < n; ++i) {
        printf("-> ");
        scanf("%f", &number);
        sum += number;
    }

    arithmetic_mean = sum / n;

    printf("The arithmetic mean of the entered sequence: %.2f\n", arithmetic_mean);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
127. Написать программу, которая вычисляет среднее арифметическое вводимой с клавиатуры последовательности дробных чисел. Количество чисел должно задаваться во время работы программы. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int n;
    float number;
    float sum = 0;
    float arithmetic_mean;

    printf("The arithmetic mean of a sequence of fractional numbers\n");
    printf("Enter the number of numbers in the sequence -> ");
    scanf("%i", &n);
    printf("After entering each number\n");

    for (int i = 0; i < n; ++i) {
        printf("-> ");
        scanf("%f", &number);
        sum += number;
    }

    arithmetic_mean = sum / n;

    printf("The arithmetic mean of the entered sequence: %.2f\n", arithmetic_mean);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
128. Написать программу, которая вводит с клавиатуры последовательность из пяти дробных чисел и после ввода каждого числа выводит среднее арифметическое введенной части последовательности. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int n = 5;
    float number;
    float sum = 0;
    float avg;

    printf("Processing a sequence of fractional numbers\n");
    printf("After entering each number press <Enter>\n");

    for (int i = 1; i <= n; ++i) {
        printf("-> ");
        scanf("%f", &number);
        sum += number;
        avg = sum / i;
        printf("Numbers entered: %i Amount: %.2f Avg. arithmetic: %.2f\n", i, sum, avg);
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
129. Написать программу, которая вычисляет среднее арифметическое последовательности дробных чисел, вводимых с клавиатуры. После ввода последнего числа программа должна вывести минимальное и максимальное числа последовательности. Количество чисел последовательности должно задаваться во время работы программы. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int i;
    int n;
    float number;
    float minimum, maximum;
    float sum;
    float avg;

    printf("Processing a sequence of fractional numbers\n");
    printf("Enter the number of numbers in the sequence -> ");
    scanf("%i", &n);
    printf("Enter the sequence. After entering each number, press <Enter>\n");

    printf("-> ");
    scanf("%f", &number);

    minimum = number;
    maximum = number;
    sum = number;

    for (i = 2; i <= n; ++i) {
        printf("-> ");
        scanf("%f", &number);
        sum += number;
        if (number < minimum) minimum = number;
        if (number > maximum) maximum = number;
    }

    avg = sum / n;

    printf("Cnt: %i\n", n);
    printf("Avg mean: %.2f\n", avg);
    printf("Min: %.2f\n", minimum);
    printf("Max: %.2f\n", maximum);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
130. Написать программу, которая генерирует последовательность из 10 случайных чисел (в диапазоне от 1 до 10), выводит эти числа на экран и вычисляет их среднее арифметическое. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    float sum = 0;
    float number;
    float avg;
    time_t t;

    srand((unsigned)time(&t));

    for (int i = 0; i < 10; ++i) {
        number = rand() % 9 + 1;
        printf("%.f\n", number);
        sum += number;
    }

    avg = sum / 10;

    printf("Avg: %.2f\n", avg);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
131. Написать программу, которая генерирует три последовательности из десяти случайных чисел (в диапазоне от 1 до 10). Для каждой последовательности программа должна рычислить среднее арифметическое. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

#define L 2
#define N 3

int main()
{
    int i, j;
    int number;
    float sum;
    float avg;

    printf("Random numbers\n");

    srand(time(NULL));

    for (i = 0; i < N; ++i) {
        sum = 0;
        for (j = 0; j < L; ++j) {
            number = rand() % 9 + 1;
            sum += number;
            printf("%i ", number);
        }
        avg = sum / L;
        printf("Avg: %.2f\n", avg);
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
132. Написать программу, которая выводит на экран таблицу стоимости, например, яблок в диапазоне от 100 г до 1 кг с шагом 100 г. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
