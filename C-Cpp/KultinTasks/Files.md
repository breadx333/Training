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
#include <stdio.h>
#include <string.h>

#define MAXLEN 80

int main()
{
    char fname[40];
    FILE *f;

    char st[MAXLEN+2];
    int n = 0;
    char key;

    printf("-> ");
    scanf("%s", &fname);

    if ((f = fopen(fname, "rt")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    while (!feof(f)) {
        fgets(st, MAXLEN, f);
        printf("%s", st);
        if (++n > 21) {
            printf("\nEnter to continue");
            key = getchar();
            n = 0;
        }
    }
    fclose(f);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
240. Написать программу, которая дописывает в находящийся на диске компьютера файл contacts.txt имя, фамилию и номер телефона, например, вашего товарища. Если файла на диске нет, то программа должна создать его. В файле каждый элемент данных (имя, фамилия, телефон) должен находиться в отдельной строке. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <string.h>

#define FNAME "numbers.txt"

int main()
{
    char fname[20] = FNAME;
    FILE *f;

    char fam[15];
    char name[15];
    char tel[9];

    if ((f = fopen(fname, "at")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    printf("Fam -> ");
    scanf("%s", &fam);
    printf("Name -> ");
    scanf("%s", &name);
    printf("Tel -> ");
    scanf("%s", &tel);

    fprintf(f, "%s %s %s", fam, name, tel);
    fclose(f);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
241. Усовершенствуйте программу работы с телефонным справочником (см. задачу 240) так, чтобы за один сеанс работы в файл contacts.txt можно было добавить информацию о нескольких людях. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <string.h>

#define FNAME "numbers.txt"

int main()
{
    char fname[20] = FNAME;
    FILE *f;

    char fam[15];
    char name[15];
    char tel[9];

    if ((f = fopen(fname, "at")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    for (int i = 0; i < 3; ++i) {
        printf("Fam -> ");
        scanf("%s", &fam);
        printf("Name -> ");
        scanf("%s", &name);
        printf("Tel -> ");
        scanf("%s", &tel);

        fprintf(f, "%s %s %s\n", fam, name, tel);
        printf("Data has been added\n");
    }
    fclose(f);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
242. Написать программу, которая позволяет найти в телефонном справочнике (в файле contacts.txt) нужную информацию. Программа должна запрашивать у пользователя фамилию человека и выводить информацию о нем. Если в справочнике есть люди с одинаковыми фамилиями, то программа должна вывести список всех этих людей. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <string.h>

#define FNAME "numbers.txt"

int main()
{
    char fname[20] = FNAME;
    FILE *f;

    char obr[15];

    char fam[15];
    char name[15];
    char tel[9];

    int n = 0;

    if ((f = fopen(fname, "rt")) == NULL) {
        printf("Error");
        getchar();
        return -1;
    }

    printf("Fam -> ");
    scanf("%s", &obr);

    while (!feof(f)) {
        fscanf(f, "%s %s %s", &fam, &name, &tel);
        if (strcmp(fam, obr) == 0) {
            printf("%s %s %s", fam, name, tel);
            ++n;
        }
    }

    if (n)
        printf("Records found: %i", n);
    else
        printf("Data not found %s", obr);

    fclose(f);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
243. Написать программу, которая объединяет возможности программ «Добавление информации в телефонный справочник» (см. задачу 24 Г) и «Поиск в телефонном справочнике» (см. задачу 242). При запуске программы на экране должно отображаться меню следующего вида:
```
#include <stdio.h>
#include <string.h>

#define FNAME "numbers.txt"

int main()
{
    char fname[20] = FNAME;
    FILE *f;

    char obr[15];

    char fam[15];
    char name[15];
    char tel[9];

    int n = 0;

    int choose = 0;

    do {
        printf("Choose -> ");
        scanf("%i", &choose);
        switch (choose) {
            case 1:
                if ((f = fopen(fname, "at")) == NULL) {
                    printf("Error\n");
                    getchar();
                    return -1;
                }

                printf("Fam -> ");
                scanf("%s", &fam);
                printf("Name -> ");
                scanf("%s", &name);
                printf("Tel -> ");
                scanf("%s", &tel);

                fprintf(f, "%s %s %s\n", fam, name, tel);
                printf("Data has been added\n");
                fclose(f);
                break;
            case 2:
                if ((f = fopen(fname, "rt")) == NULL) {
                    printf("Error\n");
                    getchar();
                    return -1;
                }

                printf("Fam -> ");
                scanf("%s", &obr);

                while (!feof(f)) {
                    fscanf(f, "%s %s %s", fam, name, tel);
                    if (strcmp(fam, obr) == 0) {
                        printf("%s %s %s\n", fam, name, tel);
                        ++n;
                    }
                }

                if (n) {
                    printf("Records found: %i\n", n);
                    n = 0;
                }
                else
                    printf("Data not found %s\n", obr);

                fclose(f);
                break;
            default: break;
        }
    } while (choose != 0);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
244. Написать программу, при помощи которой можно автоматизировать процесс проверки знаний. Сам тест, содержащий последовательность вопросов и вариантов ответа, должен находиться в текстовом файле. Имя файла теста программа должна получать из командной строки ее запуска. Количество вопросов теста не ограничено. Вместе с тем, предлагается ввести следующее ограничение: текст вопроса и альтернативных ответов не должен занимать более одной строки.
Программа должна выставлять оценку по следующему правилу: отлично — за правильные ответы на все вопросы, хорошо — если испытуемый правильно ответил не менее чем на 80% вопросов, удовлетворительно — если правильных ответов более 60%, и неудовлетворительно — если правильных ответов меньше 60%.
Далее приведены структура файла теста (N;— количество вариантов ответа к i-му вопросу, К; — номер правильного ответа) и пример файла теста.
```
#include <stdio.h>
#include <conio.h>
#include <string.h>

int main(int argc, char *argv[])
{
    char fname[40];
    FILE *f;

    int VsegoVopr = 0;
    int PravOtv = 0;

    int nOtv;
    int Prav;
    int Otv;

    int p;

    char st[80];

    int i;

    if (!argc) {
        puts("\Error file");
        return -1;
    }

    strcpy(fname, argv[1]);

    if ((f = fopen(fname, "rt")) == NULL) {
        printf("Open Error\n");
        getchar();
        return -1;
    }

    while (!feof(f)) {
        VsegoVopr++;
        fgets(st, 80, f);
        printf("\n%s\n", st);

        fscanf(f, "%i %i", &nOtv, &Prav);

        fgets(st, 80, f);

        for (i = 1; i <= nOtv; ++i) {
            fgets(st, 80, f);
            printf("%i. %s", i, st);
        }
        printf("\nChoose -> ");
        scanf("%i", &Otv);
        if (Otv == Prav) ++PravOtv;
    }

    p = PravOtv*100/VsegoVopr;
    printf("\nMark - %i%% ", p);
    if (p == 100) puts("Awesome\n");
    if (p >= 99 && p <= 80) puts("Good\n");
    if (p >= 60 && p <= 79) puts("Not bad\n");
    if (p < 60) puts("Bad\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
