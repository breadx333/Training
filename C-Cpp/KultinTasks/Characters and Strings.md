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
