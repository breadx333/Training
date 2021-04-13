201. Написать функцию пересчета температуры из градусов Фаренгейта в градусы Цельсия (С° = 5/9 (F°-32)) и программу, использующую эту функцию, которая выводит на экран таблицу соответствия температур в шкалах Фаренгейта и Цельсия.
```
#include <stdio.h>

float F2C(float f) {
    float c;
    c = (float)5/9*(f-32);
    return c;
}

int main()
{
    float f;
    float c;

    float f1, f2;
    float df;

    f1 = 0;
    f2 = 5;
    df = 0.5;

    f = f1;
    do {
        c = F2C(f);
        printf("%5.2f  %5.2f\n", f, c);
        f = f + df;
    } while (f <= f2);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
202. Написать функцию пересчета длины из дюймов в миллиметры (1 дюйм = 2,54 см).
```
#include <stdio.h>

float inc2mm(float inc) {
    float mm;
    mm = inc*2.54*10;
    return mm;
}

int main()
{
    float inc;
    float mm;

    float inc1, inc2;
    float df;

    inc1 = 0;
    inc2 = 5;
    df = 0.5;

    inc = inc1;
    do {
        mm = inc2mm(inc);
        printf("%5.2f inc %5.2f mm\n", inc, mm);
        inc = inc + df;
    } while (inc <= inc2);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
203. Написать функцию пересчета расстояния из миль в километры (1 миля = 1,60094 км).
```
#include <stdio.h>

float mile2km(float mile) {
    float km;
    km = mile*1.60934;
    return km;
}

int main()
{
    float mile;
    float km;

    float mile1, mile2;
    float df;

    mile1 = 0;
    mile2 = 5;
    df = 0.5;

    mile = mile1;
    do {
        km = mile2km(mile);
        printf("%5.2f miles %5.2f km\n", mile, km);
        mile = mile + df;
    } while (mile <= mile2);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
204. Написать функцию пересчета цены нефти за баррель в цену за тонну (1 нефтяной баррель марки Urals равен 136,4 кг). Для проверки работоспособности функции написать программу, использующую эту функцию для пересчета цены за баррель в цену за тонну.
```
#include <stdio.h>

float B2T(float b) {
    float t;
    t = b*(1000/136.4);
    return t;
}

int main()
{
    float barrel;
    float ton;

    printf("-> ");
    scanf("%f", &barrel);

    ton = B2T(barrel);

    printf("Price ton: %6.2f\n", ton);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
205. Написать функцию, которая вычисляет объем цилиндра. 
```
#define _USE_MATH_DEFINES

#include <stdio.h>
#include <math.h>

float vcil(float h, float r) {
    return (M_PI*r*r*h);
}

int main()
{
    float r, h;
    float v;

    printf("-> ");
    scanf("%f%f", &h, &r);
    v = vcil(h, r);
    printf("Value: %3.2f\n", v);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
206. Написать функцию, которая возвращает максимальное из двух целых чисел, полученных в качестве аргумента.
```
#define _USE_MATH_DEFINES

#include <stdio.h>
#include <math.h>

int mx(int a, int b) {
    if (a > b)
        return a;
    else
        return b;
}

int main()
{
    printf("%i", mx(1, 2));

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
207. Написать функцию, которая сравнивает два целых числа и возвращает результат сравнения в виде одного из знаков: >, < или =.
```
#include <stdio.h>

char compare(int a, int b) {
    char res;
    if (a > b) res = '>';
    else if (a < b) res = '<';
    else res = '=';
    return res;
}

int main()
{
    printf("%i %c %i", 1, compare(1, 2), 2);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
208. Написать функцию, которая вычисляет сопротивление цепи, состоящей из двух резисторов, которые могут быть соединены последовательно или параллельно. Функция должна проверять корректность параметров: если неверно указан тип соединения, то функция должна возвращать -1.
```
#include <stdio.h>

float sopr(float r1, float r2, int t) {
    float r;
    if (t == 1) r = r1 + r2;
    else if (t == 2) r = r1*r2/(r1+r2);
    else r = -1;
    return r;
}

int main()
{
    printf("%f", sopr(1, 2, 2));

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
209. Написать функцию percent, которая возвращает процент от числа, полученного в качестве аргумента.
```
#include <stdio.h>

float percent(float num, float per) {
    return ((num*per)/100);
}

int main()
{
    printf("%.2f%%", percent(100, 10));

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
210. Написать функцию factorial и программу, использующую эту функцию для вывода таблицы факториалов.
```
#include <stdio.h>

unsigned factorial(int x) {
    unsigned f = 1;
    for (int i = 2; i <= x; ++i)
        f *= i;
    return f;
}

int main()
{
    printf("%u", factorial(10));

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
211. Написать функцию profit, которая вычисляет доход по вкладу. Исходные данные для функции: величина вклада, процентная ставка (годовых) и срок вклада (количество дней).
```
#include <stdio.h>

float profit(float sum, float stavka, float srok) {
    return (sum*(stavka/100/365)*srok);
}

int main()
{
    printf("%f", profit(10000, 2, 36));

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
212. Написать функцию glasn, которая возвращает 1, если символ, полученный функцией в качестве аргумента, является гласной буквой русского алфавита, и ноль в противном случае.
```
#include <stdio.h>

int glasn(char ch) {
    static char gl[] = "АаЕеИиОоУуЫыЭэЮюЯя";
    int i = 0;

    while (gl[i] && gl[i] != ch)
        ++i;
    if (gl[i])
        return 1;
    else return 0;
}

int main()
{
    printf("%i", glasn('а'));

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
213. Написать функцию sogl, которая возвращает 1, если символ, полученный функцией в качестве аргумента, является согласной буквой русского алфавита, и ноль в противном случае.
```
#include <stdio.h>

int glasn(char ch) {
    static char gl[] = " БВГДЖЗЙКЛМНПРСТФХЦЧШЩ";
    int i = 0;

    while (gl[i] && gl[i] != ch)
        ++i;
    if (gl[i])
        return 1;
    else return 0;
}

int main()
{
    printf("%i", glasn('Б'));

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
214. Написать функцию upcase, которая возвращает преобразованную к верхнему регистру строку, полученную в качестве аргумента.
```
#include <stdio.h>

char *upcase(char *st) {
    int i = 0;
    while (st[i]) {
        if (st[i] >= 'a' && st[i] <= 'z' || st[i] >= 'а' && st[i] <= 'п')
            st[i] -= 32;
        else if (st[i] >= 'р' && st[i] <= 'я')
            st[i] -= 80;
        ++i;
    }
    return st;
}

int main()
{
    char st[80];

    printf("-> ");
    gets(st);
    puts(upcase(st));

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
215. Написать функцию, обеспечивающую решение квадратного уравнения. Параметрами функции должны быть коэффициенты и корни уравнения. Значением функции должна быть информация о корнях уравнения: 2 — два разных корня, 1 — корни одинаковые, 0— уравнение не имеет решения. Кроме того, функция должна проверять корректность исходных данных. Если исходные данные неверные, то функция должна возвращать -1.
```
#include <stdio.h>
#include <math.h>

int sq(float a, float b, float c, float *x1, float *x2) {
    float d;
    if (a == 0) return -1;
    d = b*b-4*a*c;
    if (d < 0) return 0;
    *x1 = (-b+sqrt(d))/(2*a);
    *x2 = (-b-sqrt(d))/(2*a);
    if (*x1 != *x2) return 2;
    else return 1;
}

int main()
{
    float a, b, c;
    float x1, x2;
    int n;

    printf("-> ");
    scanf("%f%f%f", &a, &b, &c);
    switch (sq(a, b, c, &x1, &x2)) {
        case -1: printf("Error\n"); break;
        case 0: printf("No resolve\n"); break;
        case 1: printf("Same: x=%3.2f\n", x1); break;
        case 2: printf("%3.2f  %3.2f\n", x1, x2); break;
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
216. Написать функцию, которая выводит на экран строку, состоящую из звездочек. Длина строки (количество звездочек) является параметром функции.
```
#include <stdio.h>

void starline(int len) {
    for (int i = i; i < len; ++i)
        printf("*");
    printf("\n");
}

int main()
{
    starline(10);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
217. Написать функцию, которая возвращает длину строки
```
#include <stdio.h>

int lenght(char *st) {
    int l = 0;
    char *p = st;
    while (*p++) {
        ++l;
    }
    return l;
}
int main()
{
    char st[80];
    int len;

    printf("-> ");
    gets(st);
    len = lenght(st);

    printf("Length: %i\n", len);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
218. Написать функцию, которая выводит на экран строку символов. Длина строки и символ являются параметрами функции.
```
#include <stdio.h>

void line(char ch, int n) {
    for (int i = 0; i < n; ++i)
        putchar(ch);
    printf("\n");
}

int lenght(char *st) {
    int l = 0;
    char *p = st;
    while (*p++) {
        ++l;
    }
    return l;
}

int main()
{
    char mes[] = "Hello, World!";
    int len;
    len = lenght(mes);
    line('*', len);
    printf("Hello, World!\n");
    line('*', len);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
219. Написать функцию, обеспечивающую ввод с клавиатуры целого положительного числа. При нажатии на клавишу соответствующий символ должен появляться на экране только в том случае, если это цифра. Функция должна позволять редактировать введенное число при помощи клавиши <Backspace>. При нажатии клавиши <Enter> функция должна завершать работу и возвращать введенное число.
```
#include <stdio.h>
#include <conio.h>
#include <stdlib.h>

#define K_BACK 8
#define K_ENTER 13
#define HB 4

int getint() {
    char ch;
    char buf[HB];
    int n = 0;
    buf[0] = '\0';
    while ((ch = getchar()) != K_ENTER)
        if (ch >= '0' && ch <= '9' && n < HB) {
            putchar(ch);
            buf[n++] = ch;
        }
        else if (ch == K_BACK && n) {
            printf("\b\b");
            --n;
        }
    if (n != 0) {
        buf[n] = '\0';
        return atoi(buf);
    }
    else return -1;
}
int main()
{
    int a;
    printf("-> ");
    if (a = getint())
        printf("Entered num %d\n", a);
    else printf("Error");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
220. Написать функцию, обеспечивающую ввод с клавиатуры дробного числа. При нажатии на клавишу соответствующий символ должен появляться на экране только в том случае, если этот символ допустим в данной позиции. Например, функция не должна допускать ввод знака минус не в первой позиции и более чем одной точки в составе числа. Функция должна позволять редактировать введенное число при помощи клавиши <Backspace>. При нажатии клавиши <Enter> функция должна завершать работу и возвращать введенное число.
```
#include <stdio.h>
#include <conio.h>
#include <stdlib.h>

int pos(char *st, char c) {
    int i = 0;
    while (st[i] != c && st[i])
        ++i;
    if (st[i])
        return (i+1);
    else return 0;
}

float getfloat() {
    #define N 10
    char ch;
    char buf[N+1];
    int i;
    for (i = 0; i < N+1; ++i)
        buf[i++] = '\0';
    i = 0;
    do {
        ch = getchar();
        if (ch >= '0' && ch <= '9' && i < 8) {
            putch(ch);
            buf[i++] = ch;
        }
        else
        switch (ch) {
            case '-': if (!i) {
                putch(ch);
                buf[i++] = ch;
            } break;
            case '.': if (!(pos(buf, '.'))) {
                putch(ch);
                buf[i++] = ch;
            } break;
            case 8: if (i) {
                printf("\b \b");
                buf[--i] = '\0';
            }
        }
    } while (ch != 13);
    return atof(buf);
}

int main()
{
    float f;
    printf("-> ");
    f = getfloat();
    printf("Entered %e\n", f);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
