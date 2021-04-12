181. Написать программу, которая запрашивает имя пользователя и здоровается с ним. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    char name[15];
    char fam[20];

    printf("Enter name -> ");
    scanf("%s%s", &name, &fam);

    printf("Hello %s %s)))\n", name, fam);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
182. Написать программу, которая запрашивает у пользователя имя и отчество, затем здоровается с ним. Для ввода используйте функцию getch(). NOT WORK IN C++
```
#include <stdio.h>

int main()
{
    char name[40];
    char ch;
    int i;

    printf("Enter ur name -> ");
    i = 0;
    while ((ch=getch()) != 13 && i < 40) {
        putch(ch);
        name[i++] = ch;
    }
    name[i] = '\0';
    printf("Hi %s!\n", name);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
183. Написать программу, которая вычисляет длину введенной с клавиатуры строки.
```
#include <stdio.h>

int main()
{
    char st[80];
    int i = 0;

    printf("Enter string -> ");
    gets(st);

    while (st[i++] != '\0');

    printf("Len: %i\n", i);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
184. Написать программу, которая выводит на экран сообщение в «телеграфном» стиле: буквы слов сообщения должны быть разделены символами тире.
```
#include <stdio.h>

int main()
{
    char msg[] = "kjfeh ewuifh ewiufh ;ewofh";
    int i;

    i = 0;
    while (msg[i]) {
        putchar(msg[i]);
        if (msg[i+1] != ' ') putchar('-');
        ++i;
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
185. Написать программу, которая выводит код введенного пользователем символа. Программа должна завершать работу в результате ввода, например, точки. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    unsigned char ch;

    do {
        ch = getchar();
        printf("Character: %c Code: %i\n", ch, ch);
    } while (ch != '.');

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
186. Написать программу, которая выводит на экран первую часть таблицы кодировки символов (символы с кодами от О до 127). Таблица должна состоять из восьми колонок и шестнадцати строк. В первой колонке должны быть символы с кодом от 0 до 15, во второй — от 16 до 31 и т. д.
```
#include <stdio.h>

#define SM 128

int main()
{
    unsigned char ch;

    int i, j;

    for (i = 0; i <= 16; ++i) {
        ch = i + SM;
        for (j = 1; j <= 8; ++j) {
            if ((ch<7 || ch >= 14) && ch != 26)
                printf("%3c - %4i", ch, ch);
            else
                printf("%3c - %4i", ch, ch);
            ch += 16;
        }
        printf("\n");
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
187. Написать программу, которая во введенной с клавиатуры строке преобразует строчные буквы русского алфавита в прописные (учтите, что стандартная функция upcase с символами русского алфавита не работает). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

#define SM 128

int main()
{
    char st[80];
    int i;

    printf("-> ");
    gets(st);
    i = 0;
    while (st[i]) {
        if ((st[i] >= 'a' && st[i] <= 'z') ||
            (st[i] >= 'a' && st[i] <= 'n'))
                st[i] -= 32;
        else if (st[i] >= 'р' && st[i] <= 'я')
            st[i] -= 80;
        ++i;
    }
    printf("%s\n", st);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
188. Написать программу, которая удаляет из введенной с клавиатуры строки начальные пробелы.
```
#include <stdio.h>

#define SM 128

int main()
{
    unsigned char sst[80];
    unsigned char dst[80];
    int i, j;

    i = 0;
    while ((sst[i] = getchar()) != 13)
        putchar(sst[i++]);
    sst[i] = '\0';

    i = 0;
    j = 0;
    while (sst[i] && sst[i] == ' ')
        ++i;

    while (sst[i])
        dst[j++] = sst[i++];
    dst[j] = '\0';

    printf("String without spaces: %s\n", dst);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
189. Написать программу, которая из введенного в одной строке полного имени выделяет имя, отчество и фамилию. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <string.h>

int main()
{
    char full[80];

    char first[80];
    char mid[80];
    char last[80];

    char *p1;
    char *p2;

    printf("Full Name -> ");
    gets(full);

    p1 = full;
    p2 = first;
    *p2 = '\0';
    while ((*p1 != ' ') && (*p1 != NULL)) {
        *p2 = *p1;
        ++p1;
        ++p2;
    }
    *p2 = '\0';
    p2 = mid;
    *p2 = '\0';
    if (*p1 == ' ') {
        ++p1;
        while ((*p1 != ' ') && (*p1 != NULL)) {
            *p2 = *p2;
            ++p1;
            ++p2;
        }
        *p2 = '\0';
    }
    p2 = last;
    *p2 = '\0';
    if (*p1 == ' ') {
        ++p1;
        while ((*p1 != ' ') && (*p1 != NULL)) {
            *p2 = *p1;
            ++p1;
            ++p2;
        }
        *p2 = '\0';
    }

    if (*last == '\0') {
        strcpy(last, mid);
        *mid = '\0';
    }

    printf("First name: %s\n", first);
    printf("Mid name: %s\n", mid);
    printf("Second name: %s\n", last);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
190. Написать программу, которая проверяет, является ли введенная с клавиатуры строка целым числом. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <string.h>

int main()
{
    char st[40];
    int i;

    printf("-> ");
    scanf("%s", &st);
    i = 0;
    while (st[i] >= '0' && st[i] <= '9')
        ++i;
    if (st[i])
        printf("Not ");
    printf("integer\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
191. Написать программу, которая проверяет, является ли введенная с клавиатуры строка двоичным числом.
```
#include <stdio.h>
#include <string.h>

int main()
{
    char st[40];
    int i;

    printf("-> ");
    scanf("%s", &st);
    i = 0;
    while (st[i] >= '0' && st[i] <= '1')
        ++i;
    if (st[i])
        printf("Not ");
    printf("binary\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
192. Написать программу, которая проверяет, является ли введенная с клавиатуры строка шестнадцатеричным числом.
```
#include <stdio.h>
#include <string.h>

int main()
{
    char st[40];
    int i;

    printf("-> ");
    scanf("%s", &st);

    strupr(st);

    i = 0;
    while ((st[i] >= '0' && st[i] <= '9') ||
           (st[i] >= 'A' && st[i] <= 'F'))
        ++i;
    if (st[i])
        printf("Not ");
    printf("Hex\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
193. Написать программу, которая проверяет, является ли введенная с клавиатуры строка вещественным числом.
```
#include <stdio.h>
#include <string.h>

int main()
{
    char st[40];
    int i;
    int ok = 0;

    printf("-> ");
    scanf("%s", &st);

    i = 0;
    while (st[i] >= '0' && st[i] <= '9')
        ++i;
    if (st[i] == '.') {
        ++i;
        if (st[i] >= '1' && st[i] <= '9') {
            while (st[i] >= '1' && st[i] <= '9')
            ++i;
        ok = 1;
        }
    }

    printf("String %s ", st);
    if (st[i] || !ok)
        printf("Not ");
    printf("float\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
194. Написать программу, которая преобразует введенное с клавиатуры восьмиразрядное двоичное число в десятичное. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <string.h>

int main()
{
    char bin[16];
    long int dec;
    int i;
    int v;

    printf("-> ");
    scanf("%s", &bin);

    dec = 0;
    v = 1;

    for (i = strlen(bin) - 1; i >= 0; --i) {
        if (bin[i] == '1')
            dec += v;
        v *= 2;
    }

    printf("Bin number %s ", bin);
    printf("is integer %d\n", dec);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
195. Написать программу, которая преобразует введенное с клавиатуры двухразрядное шестнадцатеричное число в десятичное.
```
#include <stdio.h>
#include <string.h>

int main()
{
    char st[5];
    unsigned int dec;
    int v;
    int err = 0;
    int i;

    printf("Hex num 4 len -> ");
    scanf("%s", &st);

    strupr(st);

    dec = 0;
    v = 1;

    for (i = strlen(st) - 1; i >= 0; --i) {
        if (st[i] >= '0' && st[i] <= '9')
            dec += v * (st[i]-48);
        else if (st[i] >= 'A' && st[i] <= 'F')
            dec += v * (st[i] - 55);
        else {
            err = 1;
            break;
        }
        v *= 16;
    }

    if (!err) {
        printf("Hex number %s ", st);
        printf("is int %u\n", dec);
    }
    else {
        printf("String %s not are hex\n");
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
196. Написать программу, которая преобразует введенное пользователем десятичное число в число в указанной системе счисления (от 2 до 10). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <string.h>

int main()
{
    int osn, n, cn, r;
    char st[17];
    int i;

    printf("-> ");
    scanf("%d", &n);
    printf("-> ");
    scanf("%d", &osn);

    cn = n;
    st[16] = '\0';
    i = 15;

    do {
        r = n % osn;
        n = n / osn;
        st[i--] = r + 48;
    } while (n > 0);

    ++i;
    int j = 0;
    while (st[i])
        st[j++] = st[i++];
    st[j] = '\0';
    st[i--] = ' ';
    printf("Decimal number %d ", cn);
    printf("number %s base %d\n", st, osn);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
197. Написать программу, которая преобразует введенное пользователем десятичное число в шестнадцатеричное.
```
#include <stdio.h>
#include <string.h>

int main()
{
    int n;
    int r;
    char st[5];
    int i;

    printf("-> ");
    scanf("%d", &n);

    printf("Dec num %d ", n);
    printf("is hex num ");
    st[5] = '\0';
    i = 4;
    do {
        r = n % 16;
        n = n / 16;
        if (r < 10)
            st[i--] = r + 48;
        else st[i--] = r + 55;
    } while (n > 0);

    ++i;
    int j = 0;
    while (st[i])
        st[j++] = st[i++];
    st[j] = '\0';

    printf("%s\n", st);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
198. Написать программу, которая вычисляет значение выражения NoOiNjC^-.OkNk, где N;— целое одноразрядное число, Oj — один из двух знаков простейших арифметических действий: сложения (+) или вычитания (-). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    char st[40];
    char buf[10];
    char op;
    int rez;
    int n;
    int i, j;

    printf("-> ");
    scanf("%s", &st);

    rez = 0;
    op = ' ';
    i = j = 0;
    while (st[i]) {
        j = 0;
        while (st[i] >= '0' && st[i] <= '9')
            buf[j++] = st[i++];
        buf[j] = '\0';
        n = atoi(buf);

        switch (op) {
            case '+': rez += n; break;
            case '-': rez -= n; break;
            case ' ': rez = n; break;
        }
        op = st[i++];
    }

    printf("Mean: %d\n", rez);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
199. Написать программу, реализующую игру «Угадай число». Правила игры следующие. Играют двое. Первый игрок задумывает число, второй должен угадать число, задуманное первым. На каждом шаге угадывающий делает предположение, а задумавший число — говорит, сколько цифр числа угаданы и сколько из угаданных цифр занимают правильные позиции в числе. Например, если задумано число 725 и сделано предположение, что задуманное число 523, то угаданы две цифры (5 и 2), но только одна из них (2) занимает верную позицию.
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

#define N 3
#define DEBUG

int main()
{
    char player[N];
    char pc[N] = {'6', '5', '8'};

    int a[N];
    int ugad;
    int mesto;

    int i, j;
    time_t t;

    srand((unsigned)time(&t));

    for (i = 0; i < N; ++i)
        pc[i] = rand() % 10 + 48;

#ifdef DEBUG
    printf("PC: ");
    for (i = 0; i < N; ++i)
        printf("%c", pc[i]);
    printf("\n");
#endif // DEBUG

    do {
        printf("Your value -> ");
        scanf("%s", &player);

        for (i = 0; i < N; ++i)
            a[i] = 0;

        ugad = 0;

        for (i = 0; i < N; ++i) {
            for (j = 0; j < N; ++j) {
                if ((player[i] == pc[j]) && !a[j]) {
                    ++ugad;
                    a[j] = 1;
                    break;
                }
            }
            mesto = 0;
            for (i = 0; i < N; ++i)
                if (player[i] == pc[i]) ++mesto;
            printf("Guess cnt: %i. In their places: %i\n", ugad, mesto);
        }
    } while ((mesto < N) || (ugad < N));

    printf("U are guess number conceived pc\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
200. Написать программу «Телеграф», которая принимает от пользователя сообщение и выводит его на экран в виде последовательности точек и тире. Вывод точек и тире можно сопроводить звуковым сигналом соответствующей длительности. Азбука Морзе для букв русского алфавита приведена в следующей таблице.
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

#define N 3
#define DEBUG

int main()
{
    char *morse[] = {".-  ", "-...", ".---", "--. ",
                     "-.. ", ".   ", "...-", "--..",
                     "..  ", ".---", "-.- ", ".-..",
                     "--  ", "-.  ", "--- ", ".--.",
                     ".-. ", "... ", "-   ", "..- ",
                     "..-.", "....", "-.-.", "---.",
                     "----", "--.-", "-..-", "-.--",
                     "-..-", "..-.", "..--", ".-.-"};

    char mes[80];
    char sim[4];

    char znak;
    int i, j;

    printf("-> ");
    gets(mes);

    for (i = 0; i < strlen(mes); ++i) {
        if (mes[i] >= 'А' && mes[i] <= 'Я') {
            strcpy(sim, morse[mes[i-128]);
            j = 0;
            do {
                if (sim[j] == '-' || sim[j] == '.') {
                    putchar(sim[j++]);
                }
            } while (sim[j] != ' ' && j < 4);
        }
        else if (mes[i] == ' ') {
            printf(" ");
        }
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
