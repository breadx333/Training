
1. Объявить переменные, необходимые для вычисления площади прямоугольника.
```
#include <iostream>

int main()
{
    float a = 0, b = 0;
    std::cin >> a >> b;
    float s = (a * b) / 2;
    std::cout << s << std::endl;
    return 0;
}
```
2. Объявить переменные, необходимые для пересчета веса из фунтов в килограммы.
```
#include <iostream>

int main()
{
    float funt;
    float kg;

    std::cin >> funt;
    kg = funt / 2.442;
    std::cout << kg << std::endl;

    return 0;
}
```
3. Определить исходные данные и объявить переменные, необходимые для вычисления дохода по вкладу.
```
#include <iostream>

int main()
{
    float summa = 100000;
    int srok = 40;
    int stavka = 1;
    float dohod = summa / 100 * stavka / 365 * srok;

    std::cout << dohod << std::endl;

    return 0;
}
```
4. Объявить переменные, необходимые для вычисления площади круга.
```
#include <iostream>

int main()
{
    double r = 0;
    const double pi = 3.1416;

    std::cin >> r;
    std::cout << "Area of circe: " << pi * (r * r) << std::endl;

    return 0;
}

```
5. Объявить переменные, необходимые для вычисления площади кольца. 
```
#include <iostream>

int main()
{
    const float pi = 3.1416;
    float r1 = 0, r2 = 0;
    std::cin >> r1 >> r2;
    float s = pi * (r1 - r2);
    std::cout << s << std::endl;
    return 0;
}
```
6. Объявить переменные, необходимые для вычисления объема и площади поверхности цилиндра.
```
#include <iostream>

int main()
{
    const double pi = 3.1416;
    double r = 3;
    double h = 6;

    double v = (pi * (r * r)) * h;
    double s = 2 * pi * r * (r + h); //(2 * pi * r * h) + (2 * pi * (r * r));

    std::cout << v << ' ' << s << std::endl;

    return 0;
}
```
7. Объявить переменные, необходимые для вычисления стоимости покупки, состоящей из нескольких тетрадей, карандашей и линейки.
```
#include <iostream>

int main()
{
    float CenaTetr = 3.2;
    int KolTetr = 6;

    float CenaKar = 2.6;
    int KolKar = 2;

    float CenaLin = 4;
    int KolLin = 1;

    float Summa = (CenaTetr * KolTetr) + (CenaKar * KolKar) + (CenaLin * KolLin);

    std::cout << Summa << std::endl;

    return 0;
}
```
8. Объявить переменные, необходимые для вычисления стоимости покупки, состоящей из нескольких тетрадей и такого же количества обложек. [b]/// Задания ебанутые конечно...[/b]
```
#include <iostream>

int main()
{
    float CenaTetr = 2.8;
    int KolTetr = 3;

    float CenaObl = 0.5;
    int KolObl = 3;

    float Summa = (CenaTetr * KolTetr) + (CenaObl * KolObl);

    std::cout << Summa << std::endl;

    return 0;
}
```
9. Записать инструкцию, которая присваивает переменной x значение 1,5.
```
#include <iostream>

int main()
{
    double x = 0;
    
    x = 1.5;
    
    return 0;
}
```
10. Написать инструкцию, которая присваивает переменной summa нулевое значение.
```
#include <iostream>

int main()
{
    double summa = 912;
    
    summa = 0;
    
    return 0;
}
```
11. Записать инструкцию, которая увеличивает на единицу значение переменной п.
```
#include <iostream>

int main()
{
    int n = 1;

    ++n;

    std::cout << n << std::endl;

    return 0;
}
```
12. Записать инструкцию, которая уменьшает на два значение переменной counter.
```
#include <iostream>

int main()
{
    int counter = 7;

    counter -= 2;

    std::cout << counter << std::endl;

    return 0;
}
```
13. Написать инструкцию вычисления среднего арифметического переменных xl и х2.
```
#include <iostream>

int main()
{
    double x = 8.6, y = 2.2;

    double middleArithmetic = (x + y) / 2;

    std::cout << middleArithmetic << std::endl;

    return 0;
}
```
14. Записать в виде инструкции присваивания формулу вычисления значения функции у = -2,7х^3+ 0,23х^2- 1,4.
```
#include <iostream>

int main()
{
    double y = 0;

    int x = 3;

    y = (-2.7)*x*x*x + 0.23*x*x - 1.4;

    std::cout << y << std::endl;

    return 0;
}
```
15. Написать инструкцию, которая увеличивает значение переменной х на величину, находящуюся в переменной dx.
```
#include <iostream>

int main()
{
    int x = 3, dx = 6;

    x += dx;

    std::cout << x << std::endl;

    return 0;
}
```
16. Записать в виде инструкции присваивания формулу пересчета веса из фунтов в килограммы (один фунт = 405,9 г).
```
#include <iostream>

int main()
{
    double kg = 0, funt = 777;

    kg = funt * 0.4059;

    std::cout << kg << std::endl;

    return 0;
}
```
17. Записать в виде инструкции присваивания формулу пересчета расстояния из километров в версты (одна верста = 1066,8 м).
```
#include <iostream>

int main()
{
    double km = 1228, vrst = 0;

    vrst = (km * 1000) / 1066.8;

    std::cout << vrst << std::endl;

    return 0;
}
```
18. Записать в виде инструкции присваивания формулу вычисления площади прямоугольника.
```
#include <iostream>

int main()
{
    double a = 8, b = 6.888, c = 0;

    c = (a * b) / 2;

    std::cout << c << std::endl;

    return 0;
}
```
19. Записать в виде инструкции присваивания формулу вычисле1 ь ния площади треугольника: а л, где a— длина основания, h — высота треугольника.
```
#include <iostream>

int main()
{
    double a = 8, h = 6.888, s = 0;

    s = 0.5 * a * h;

    std::cout << s << std::endl;

    return 0;
}
```
20.  Записать в виде инструкции присваивания формулу вычислеa+b 1 к ния площади трапеции: s=——" > гДе a и Ь — длины основании, h — высота трапеции.
```
#include <iostream>

int main()
{
    double a = 8, b = 6.888, h = 7;
    double s = 0;

    s = (a + b) / 2 * h;

    std::cout << s << std::endl;

    return 0;
}
```
21. Записать в виде инструкции присваивания формулу вычисления площади круга: s=pi*(r^2)
```
#include <iostream>

int main()
{
    const double pi = 3.1416;
    double r = 9.1337;
    double s = 0;

    s = pi * (r * r);

    std::cout << s << std::endl;

    return 0;
}
```
22. Записать в виде инструкции присваивания формулы вычисления площади поверхности и объема цилиндра.
```
#include <iostream>

int main()
{
    const double pi = 3.1416;
    double r = 13.55, h = 4;
    double s = 0, v = 0;

    s = 2 * pi * r * (h + r);
    v = pi * (pi * pi) * h;

    std::cout << s << '\n' << v << std::endl;

    return 0;
}
```
23. Записать в виде инструкции присваивания формулу вычисления объема параллелепипеда.
```
#include <iostream>

int main()
{
    double a = 1, b = 5, c = 3;
    double s = 0;

    s = 2 * (a*b + b*c + a*c);

    std::cout << s << std::endl;

    return 0;
}
```
24. Объявить необходимые переменные и записать в виде инструкции присваивания формулы вычисления объема и площади поверхности шара.
```
#include <iostream>

int main()
{
    const double pi = 3.1416;
    double r = 3.1;
    double v = 0, s = 0;

    v = (3 * pi * (r * r * r)) / 4;
    s = 4 * pi * (r * r);

    std::cout << v << '\n' << s << std::endl;

    return 0;
}
```
25. Записать в виде инструкции присваивания формулу вычисления объема цилиндра.
```
#include <iostream>

int main()
{
    const double pi = 3.1416;
    double r = 2.22, h = 7.777;
    double v = 0;

    v = pi * (r*r) * h;

    std::cout << v << std::endl;

    return 0;
}
```
26. Записать в виде инструкции присваивания формулу вычисления объема полого цилиндра.
```
#include <iostream>

int main()
{
    const double pi = 3.1416;
    double r1 = 2.22, r2 = 1.22, h = 7.777;
    double v = 0;

    v = pi * h * (r1*r1 - r2*r2);

    std::cout << v << std::endl;

    return 0;
}
```
27. Записать в виде инструкции присваивания формулу вычисления объема конуса.
```
#include <iostream>

int main()
{
    const double pi = 3.1416;
    double r = 2.22, h = 7.777;
    double s = 0;

    s = (pi * (r*r) * h) / 3;

    std::cout << s << std::endl;

    return 0;
}
```
28.  Записать в виде инструкции присваивания формулу пересчета температуры из градусов Фаренгейта в градусы Цельсия: C=5/9(F-32).
```
#include <iostream>

int main()
{
    double C = 0, F = 133;

    C = (5 * (F - 32)) / 9;

    std::cout << C << std::endl;

    return 0;
}
```
29. Записать в виде инструкции присваивания формулу для вычисления тока по известным значениям напряжения и сопротивления электрической цепи.
```
#include <iostream>

int main()
{
    double U = 220, R = 2;
    double I = 0;

    I = U / R;

    std::cout << I << std::endl;

    return 0;
}
```
30. Записать в виде инструкции присваивания формулу вычисления сопротивления электрической цепи по известным значениям напряжения и силы тока. 
```
#include <iostream>

int main()
{
    double U = 220, I = 110;
    double R = 0;

    R = U / I;

    std::cout << R << std::endl;

    return 0;
}
```
31. Записать в виде инструкции присваивания формулу вычисления сопротивления электрической цепи, состоящей из трех последовательно соединенных резисторов.
```
#include <iostream>

int main()
{
    double R1 = 220, R2 = 110, R3 = 110;
    double R = 0;

    R = R1 + R2 + R3;

    std::cout << R << std::endl;

    return 0;
}
```
32. Записать в виде инструкции присваивания формулу вычисления сопротивления электрической цепи, состоящей из двух параллельно соединенных резисторов: г= (r1 * r2) / r1 + r2;
```
#include <iostream>

int main()
{
    double R1 = 220, R2 = 110;
    double R = 0;

    R = R1 * R2 / (R1 + R2);

    std::cout << R << std::endl;

    return 0;
}
```
33. Записать в виде инструкции присваивания формулу пересчета сопротивления электрической цепи из омов в килоомы.
```
#include <iostream>

int main()
{
    double R = 12698;
    double ROm = 0;

    ROm = R/1000;

    std::cout << ROm << std::endl;

    return 0;
}
```
34. Объявить необходимые переменные и записать в виде инструкции присваивания формулу вычисления стоимости покупки, состоящей из нескольких тетрадей, обложек к ним и карандашей.
```
#include <iostream>

int main()
{
    float ctetr = 2.3, cobl = 1.1, ckar = 6.4;
    int ntetr, nkar = 2;
    float summ = 0;

    summ = ntetr*(ctetr+cobl) + nkar*ckar;

    std::cout << summ << std::endl;

    return 0;
}
```
35. Написать программу, которая выводит на экран имя сына Гомера Симпсона.
```
#include <stdio.h>

int main()
{
    printf("Bart Simpson\n");
    getchar();

    return 0;
}
```
36. Написать программу, которая выводит на экран имена детей Гомера и Мардж Симпсонов (имя каждого — с новой строки).
```
#include <stdio.h>

int main()
{
    printf("Bart Simpson\nLisa Simpson\nMaggi Simpson\n");
    printf("To exit press <Enter>");
    getchar();

    return 0;
}
```
37. Написать программу, которая выводит на экран имена детей Гомера и Мардж Симпсонов (имя каждого — с новой строки).
```
#include <stdio.h>
#include <string.h>

char* rus(char st[])
{
    char* st2 = new char[strlen(st) + 2];

    int i = 0;

    while (st[i] != 0) {
        unsigned char ch = st[i];
        if ((ch >= 192) && (ch <= 255)) {
            if (ch < 240)
                st2[i] = st[i] - 64;
            else
                st2[i] = st[i] - 16;
        }
        else
            st2[i] = st[i];
        ++i;
    }
    st2[i] = 0;
    return st2;
}

int main()
{
    printf(rus("Барт Симпсон\n"));

    return 0;
}
```
38. Написать инструкцию вывода значений переменных а, b и с (типа float) с пятью цифрами в целой части и тремя — в дробной. Значения должны быть выведены в виде: a = значение b = значение с = значение.
```
#include <stdio.h>

int main()
{
    float a = 1.222, b = 2.123123, c = 12345678.2333333;

    printf("a=%5.3f\tb=%5.3f\tc=%5.3f", a, b, c);

    return 0;
}
```
39. Написать инструкцию вывода значений переменных h и w (типа float), которые содержат значения высоты и длины прямоугольника. Перед значением переменной должен идти пояснительный текст (Height = Width =), а после — единица измерения (sm).
```
#include <stdio.h>

int main()
{
    float h = 4.12312, w = 123.1412;
    printf("Height = %f,     Width = %f", h, w);
    return 0;
}
```
40. Написать инструкцию, которая выводит в одной строке значения переменных тип целого типа (int).
```
#include <stdio.h>

int main()
{
    int m = 12, n = 13;
    printf("m=%i\tn=%i\n", m, n);
    return 0;
}
```
41. Написать инструкцию вывода значений целых переменных а, b и с. Значение каждой переменной должно быть выведено в отдельной строке.
```
#include <stdio.h>

int main()
{
    int a = 1, b = 2, c = 3;
    printf("a=%i\nb=%i\nc=%i\n", a, b, c);
    return 0;
}
```
42. Написать инструкции вывода значений дробных переменных х! и х2. На экране перед значением переменной должен быть выведен поясняющий текст, представляющий собой имя переменной, за которым следует знак «равно».
```
#include <stdio.h>

int main()
{
    double x1 = 123.321, x2 = 345.543;
    printf("double x1 = %d\ndouble x2 = %d\n", x1, x2);
    return 0;
}
```
43. Написать программу, которая выводит палитру — фразу Hello, World! всеми возможными для консольного приложения цветами. Перед каждой фразой необходимо указать код цвета, которым она выведена.
```
#include <stdio.h>
#include <iostream>
#include <windows.h>

int main()
{
    HANDLE hConsole = GetStdHandle(STD_OUTPUT_HANDLE);

    for (int i = 0; i < 16; ++i) {
        SetConsoleTextAttribute(hConsole, i);
        std::cout << i << " - Hello, World!\n";
    }
    return 0;
}
```
44. Написать программу, которая выводит на экран в трех строках слово RUSSIA. Первая строка должна быть выведена белым, вторая — синим, третья — красным цветом.
```
#include <stdio.h>
#include <iostream>
#include <windows.h>

#define WHITE       7
#define GRAY        8
#define BLUE        9
#define GREEN       10
#define BLUE_LIGHT  11
#define RED         12
#define MAGNETA     13
#define YELLOW      14
#define WHITE_LIGHT 15

int main()
{
    HANDLE hConsole = GetStdHandle(STD_OUTPUT_HANDLE);

    SetConsoleTextAttribute(hConsole, WHITE_LIGHT);
    std::cout << "RUSSIA" << std::endl;

    SetConsoleTextAttribute(hConsole, BLUE);
    std::cout << "RUSSIA" << std::endl;

    SetConsoleTextAttribute(hConsole, RED);
    std::cout << "RUSSIA" << std::endl;

    return 0;
}
```
45. Написать инструкцию, которая обеспечивает ввод с клавиатуры переменной koi целого типа.
```
#include <stdio.h>

int main()
{
    int kol = 0;

    scanf("%i", &kol);
    printf("kol: %i", kol);

    return 0;
}
```
46. Написать инструкцию, обеспечивающую ввод с клавиатуры значения переменной radius типа float.
```
#include <stdio.h>

int main()
{
    float radius = 0;

    scanf("%f", &radius);
    printf("radius: %f", radius);

    return 0;
}
```
47. Написать инструкции, которые обеспечивают ввод значений вещественных переменных и и г (тип float). Предполагается, что пользователь после набора каждого числа будет нажимать клавишу <Enter> (каждое число вводить в отдельной строке).
```
#include <stdio.h>

int main()
{
    float u = 0, r = 0;

    scanf("%f", &u);
    scanf("%f", &r);
    printf("%f ::: %f", u, r);

    return 0;
}
```
48. Написать инструкцию, которая обеспечивает ввод значений переменных и и г (тип float). Предполагается, что пользователь будет набирать числа в одной строке.
```
#include <stdio.h>

int main()
{
    float u = 0, r = 0;
    
    scanf("%f %f", &u, &r);
    printf("%f ::: %f", u, r);
    
    return 0;
}

```
49. Объявить необходимые переменные и написать фрагмент программы вычисления объема цилиндра, обеспечивающий ввод исходных данных.
```
#include <stdio.h>

int main()
{
    const float pi = 3.1416;
    float r = 0, h = 0;
    float v = 0;

    printf("Enter data:\n");
    printf("Enter Radius -> ");
    scanf("%f", &r);
    printf("Enter Height -> ");
    scanf("%f", &h);

    v = pi * (r*r) * h;

    printf("V: %f\n", v);

    return 0;
}
```
50. Объявить необходимые переменные и написать инструкции ввода исходных данных для программы вычисления дохода по вкладу. Предполагается, что процентную ставку программа определяет на основе данных о сумме и сроке вклада.
```
#include <stdio.h>

int main()
{
    float sum = 0; //Задача говно, не буду решать
    int period = 0;
    float rate = 0.01;
    float profit = 0;
    
    float value = 0;
    printf("Enter Summ -> ");
    scanf("%f", &sum);
    printf("Enter Period -> ");
    scanf("%i", &period);
    
    profit = 
    
    return 0;
}
```
51. Написать программу вычисления площади прямоугольника. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float length = 0, width = 0;
    float S = 0;

    printf("Calculating the area of a rectangle\n");
    printf("Enter Data:\n");
    printf("Length -> ");
    scanf("%f", &length);
    printf("Width -> ");
    scanf("%f", &width);

    S = length * width;

    printf("Area of a rectangle: %.2f sq. cm.\n", S);

    return 0;
}
```
52. Написать программу вычисления площади параллелограмма.
```
#include <stdio.h>

int main()
{
    float d1 = 0, d2 = 0;
    float S = 0;

    printf("Enter Alpha and height: ");
    scanf("%f %f", &d1, &d2);

    S = 0.5 * d1 * d2;

    printf("S: %f", S);

    return 0;
}
```
53. Написать программу вычисления объема параллелепипеда. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float length = 0, width = 0, height = 0;
    float v = 0;

    printf("Сalculating the volume of a parallelepiped\n");
    printf("Enter initial data:");
    printf("length -> ");
    scanf("%f", &length);
    printf("width -> ");
    scanf("%f", &width);
    printf("heigth -> ");
    scanf("%f", &height);

    v = length * width * height;

    printf("Volume: %.2f c. cm.", v);

    return 0;
}
```
54. Написать программу вычисления площади поверхности параллелепипеда. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float l, w, h;
    float s;

    printf("\nCalculating square of surface rectangle\n");
    printf("Enter initial data:\n");
    printf("Length -> ");
    scanf("%f", &l);
    printf("Width -> ");
    scanf("%f", &w);
    printf("Height -> ");
    scanf("%f", &h);

    s = (l*w + l*h + w*h)*2;

    printf("Square of surface: %6.2f sq. cm.\n", s);
    printf("\n\nTo complete calculating press <Enter>");
    getchar();

    return 0;
}
```
55. Написать программу вычисления объема куба. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float edge_length = 0;
    float ValueOfCube = 0;

    printf("Enter the lenght of the edge: ");
    scanf("%f", &edge_length);

    ValueOfCube = edge_length * edge_length * edge_length;

    printf("Value of Cube: %f\n", ValueOfCube);

    return 0;
}
```
56. Написать программу вычисления объема цилиндра. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    const float PI = 3.141592;
    float radius = 0;
    float height = 0;
    float Value = 0;

    printf("Calculating Value of Cylinder\n");
    printf("Enter initial data:\n");
    printf("Base Radius -> ");
    scanf("%f", &radius);
    printf("Height -> ");
    scanf("%f", &height);

    Value = PI * (radius * radius) * height;

    printf("Value of Cylinder: %f\n", Value);

    printf("Press <Enter> to finish\n");
    getchar();

    return 0;
}
```
57. Написать программу вычисления стоимости покупки, состоящей из нескольких тетрадей и карандашей. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float price_notebook;
    unsigned cnt_notebook;
    float price_pen;
    unsigned cnt_pen;

    float sum;

    printf("Calculating purchase value\n");
    printf("Enter initial data:\n");
    printf("Notebook price -> ");
    scanf("%f", &price_notebook);
    printf("Number of notebook -> ");
    scanf("%u", &cnt_notebook);
    printf("Pen price -> ");
    scanf("%f", &price_pen);
    printf("Number of pen -> ");
    scanf("%u", &cnt_pen);

    sum = price_notebook * cnt_notebook + price_pen * cnt_pen;

    printf("Purchase Amount: %6.2f\n", sum);
    getchar();

    return 0;
}
```
58. Написать программу вычисления стоимости покупки, состоящей из нескольких тетрадей и такого же количества обложек к ним. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float price_notebook = 0;
    float price_cover = 0;
    unsigned cnt_set = 0;
    float sum = 0;

    printf("Calculating purchase value\n");
    printf("Enter initial data:\n");
    printf("Notebook price -> ");
    scanf("%f", &price_notebook);
    printf("Cover price -> ");
    scanf("%f", &price_cover);
    printf("Number of Sets: ");
    scanf("%u", &cnt_set);

    sum = (price_notebook + price_cover) * cnt_set;

    printf("Purchase Amount: %.2f", sum);

    return 0;
}
```
59. Написать программу вычисления стоимости некоторого количества (по весу), например, яблок. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float price_kg = 0;
    float weight = 0;
    float sum = 0;

    printf("Calculating purchase value\n");
    printf("Enter initial data:\n");
    printf("Price per kg -> ");
    scanf("%f", &price_kg);
    printf("Apple weight -> ");
    scanf("%f", &weight);

    sum = price_kg * weight;

    printf("Purchase Amount: %.2f\n", sum);

    return 0;
}
```
60. Написать программу вычисления площади треугольника, если известна длина его основания и высота. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float base = 0;
    float height = 0;
    float square = 0;

    printf("Calculating the area of a triangle\n");
    printf("Enter initial data:\n");
    printf("Length Base -> ");
    scanf("%f", &base);
    printf("Height -> ");
    scanf("%f", &height);

    square = 0.5 * base * height;

    printf("\nSquare of Triangle: %f\n", square);

    return 0;
}
```
61. Написать программу вычисления площади треугольника, если известны длины двух его сторон и величина угла между этими сторонами. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#define _USE_MATH_DEFINES

#include <stdio.h>
#include <math.h>

int main()
{
    float a = 0, b = 0;
    float angle = 0;
    float square = 0;

    printf("Calculating the area of a triangle\n");
    printf("Enter the lengths of the sides on one line:\n-> ");
    scanf("%f %f", &a, &b);
    printf("Enter the angle between sidie:\n-> ");
    scanf("%f", &angle);

    square = a*b*sin(angle*M_PI/180)/2;

    printf("\nSquare of Triangle: %f\n", square);

    return 0;
}
```
62. Написать программу вычисления сопротивления электрической цепи, состоящей из двух параллельно соединенных сопротивлений. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float R1 = 0, R2 = 0;
    float R = 0;

    printf("Calculating of the resistance of an electrical\n");
    printf("circuit with parallel connection of elements\n");
    printf("Enter the initial data:\n");
    printf("The value of the first resistance -> ");
    scanf("%f", &R1);
    printf("The value of the second resistance -> ");
    scanf("%f", &R2);

    R = R1*R2/(R1+R2);

    printf("\nCircuit resistance: %f\n", R);

    return 0;
}
```
63. Написать программу вычисления сопротивления электрической цепи, состоящей из двух последовательно соединенных сопротивлений. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float R1 = 0, R2 = 0;
    float R = 0;

    printf("Calculating of the resistance of an electrical circuit\n");
    printf("Enter the initial data:\n");
    printf("The value of the first resistance -> ");
    scanf("%f", &R1);
    printf("The value of the second resistance -> ");
    scanf("%f", &R2);

    R = R1 + R2;

    printf("\nCircuit resistance (Serial connection ): %f\n", R);

    return 0;
}
```
64. Написать программу вычисления силы тока в электрической цепи. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float V = 0, R = 0;
    float I = 0;

    printf("Calculation of the current in an electrical target\n");
    printf("Enter the initial data:\n");
    printf("Voltage -> ");
    scanf("%f", &V);
    printf("Resistance -> ");
    scanf("%f", &R);

    I = V / R;

    printf("\nCurrent: %f\n", I);

    return 0;
}
```
65. Написать программу вычисления расстояния между населенными пунктами, показанными на карте. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float scale_map = 0, distance_cm = 0;
    float distance_km = 0;

    printf("Calculation of the distance between settlements\n");
    printf("Enter the initial data:\n");
    printf("Scale -> ");
    scanf("%f", &scale_map);
    printf("Between points -> ");
    scanf("%f", &distance_cm);

    distance_km = scale_map * distance_cm;

    printf("\nThe distance between the points is %f\n", distance_km);

    return 0;
}
```
66.  Написать программу вычисления стоимости поездки на автомобиле. Исходные данные: расстояние (км); количество бензина (в литрах), которое потребляет автомобиль на 100 км пробега; цена одного литра бензина. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float distance = 0, gasoline_consumption = 0, price = 0;
    float cost = 0;

    printf("Calculating the cost of a trip by car\n");
    //printf("Enter the initial data:\n");
    printf("Distance -> ");
    scanf("%f", &distance);
    printf("Gasoline consumption -> ");
    scanf("%f", &gasoline_consumption);
    printf("Price of a liter of gasoline -> ");
    scanf("%f", &price);

    cost = distance * (gasoline_consumption/100) * price;

    printf("\nThe trip will cost %f.2\n", cost);

    return 0;
}
```
67. Написать программу, которая вычисляет скорость, с которой спортсмен пробежал дистанцию. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float distance = 0, time = 0;
    int time_m = 0, time_s = 0;
    float ts = 0;
    float speed = 0;

    printf("Calculating running speed\n");
    //printf("Enter the initial data:\n");
    printf("Enter distance -> ");
    scanf("%f", &distance);
    printf("Enter time -> ");
    scanf("%f", &time);

    time_m = time;
    time_s = (time - time_m) * 100;
    ts = time_m * 60 + time_s;

    speed = (distance/1000) / (ts / 3600);

    printf("Distance: %f\n", distance);
    printf("Time: %i min %i sec = %f sec\n", time_m, time_s, ts);
    printf("Speed: %f km/h\n", speed);

    return 0;
}
```
68. Написать программу вычисления объема цилиндра. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    const float PI = 3.141592;
    float radius = 0, height = 0;
    float volume = 0;

    printf("Calculation of the volume of a cylinder\n");
    printf("Enter the initial data:\n");
    printf("Base radius -> ");
    scanf("%f", &radius);
    printf("Height -> ");
    scanf("%f", &height);

    volume = PI * (radius*radius) * height;

    printf("The volume of the cylinder is %.2f cm cc.\n", volume);

    return 0;
}
```
69. Написать программу вычисления площади поверхности цилиндра. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    const float PI = 3.141592;
    float radius = 0, height = 0;
    float square = 0;

    printf("Calculation of the surface area of a cylinder\n");
    printf("Enter the initial data:\n");
    printf("Base radius -> ");
    scanf("%f", &radius);
    printf("Height -> ");
    scanf("%f", &height);

    square = 2 * (PI * (radius*radius)) + (2 * PI * radius * height);

    printf("Cylinder surface area: %.2f sq. cm.\n", square);

    return 0;
}
```
70. Написать программу вычисления объема параллелепипеда. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    const float PI = 3.141592;
    float length = 0, width = 0, height = 0;
    float volume = 0;

    printf("Calculating the volume of a box\n");
    printf("Enter the box's length, width, and height (in centimeters) on one line\n-> ");
    scanf("%f %f %f", &length, &width, &height);

    volume = length * width * height;

    printf("The volume of the parallelepiped is %.2f cm cb.\n", volume);

    return 0;
}
```
71. Написать программу пересчета расстояния из миль в километры (1 миля равна 1600,94 м). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float miles = 0;
    float kilometres = 0;

    printf("Converting distance from miles to kilometers\n");
    printf("Enter distance in miles -> ");
    scanf("%f", &miles);

    kilometres = miles * 1600.94 / 1000;

    printf("\n%.2f miles is %.2f km\n", miles, kilometres);

    return 0;
}
```
72. Написать программу пересчета веса из фунтов в килограммы (1 российский фунт равен 405,9 г). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float pounds = 0;
    float killogramms = 0;

    printf("Conversion of weight from pounds to kilograms\n");
    printf("Enter weight in pounds -> ");
    scanf("%f", &pounds);

    killogramms = pounds * 405.9 / 1000;

    printf("\n%.2f pounds - is %.2f kg\n", pounds, killogramms);

    return 0;
}
```
73. Написать программу вычисления дохода по вкладу. Сумма, процентная ставка (% годовых) и срок вклада (в месяцах) задаются во время работы программы. Далее приведен рекомендуемый вид экрана (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float amount, term, rate;
    float Income, Summ;

    printf("Calculation of deposit income\n");
    printf("Enter the initial data:\n");
    printf("Deposit amount -> ");
    scanf("%f", &amount);
    printf("Deposit term -> ");
    scanf("%f", &term);
    printf("Interest rate -> ");
    scanf("%f", &rate);

    Income = amount * rate/12/100 * term;
    Summ = amount + Income;

    printf("-----------------------------\n");
    printf("Income: %.2f\n", Income);
    printf("Amount at the end of the term of the deposit: %.2f\n", Summ);

    return 0;
}
```
74. Написать программу пересчета величины временного интервала, заданного в минутах, в величину, выраженную в часах и минутах. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int minutes;
    int time_h, time_m;

    printf("Enter the time interval -> ");
    scanf("%i", &minutes);

    time_h = minutes / 60;
    time_m = minutes % 60;

    printf("%i minutes - is %i h. %i min.\n", minutes, time_h, time_m);

    return 0;
}
```
75. Написать программу, которая преобразует введенное с клавиатуры дробное число в денежный формат. Например, число 12.5 должно быть преобразовано к виду 12 руб. 50 коп. Далее приведен рекомендуемый вид экрана (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float number;
    int rub, kop;

    printf("Convert number to currency format\n");
    printf("Enter fractional number -> ");
    scanf("%f", &number);

    rub = number;
    kop = number * 100 - rub * 100;

    printf("%.2f rubles - is %i rub. %i kop.\n", number, rub, kop);

    return 0;
}
```
76. Написать программу пересчета веса из фунтов в килограммы (1 фунт= 405,9 г). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float pounds;
    float weight;
    int kg, gr;

    printf("Converting weight from pounds to kilograms\n");
    printf("Enter the weight in pounds\n-> ");
    scanf("%f", &pounds);

    weight = pounds * 405.9;
    kg = weight / 1000;
    gr = weight - kg * 1000;

    printf("%.2f lb - is %i kg %i gr.\n", pounds, kg, gr);

    return 0;
}
```
77. Написать программу, которая вычисляет площадь треугольника, если известны координаты его углов. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int x1, y1;
    int x2, y2;
    int x3, y3;
    float square;

    printf("Calculating the area of a triangle\n");
    printf("Enter the coordinates of the angles\n");
    printf("x1, y1 -> ");
    scanf("%i %i", &x1, &y1);
    printf("x2, y2 -> ");
    scanf("%i %i", &x2, &y2);
    printf("x3, y3 -> ");
    scanf("%i %i", &x3, &y3);

    square = abs((x2-x1)*(y3-y1)-(x3-x1)*(y2-y1))/2;

    printf("\nArea of the triangle: %.2f square meters\n", square);

    return 0;
}
```
78. Написать программу вычисления сопротивления электрической цепи, состоящей из двух сопротивлений, которые могут быть соединены последовательно или параллельно. Далее приведен рекомендуемый вид экрана (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>

int main()
{
//    const float PI = 3.141592;
    float R1, R2;
    unsigned choose;
    float R;

    printf("Calculating the resistance of the electrical circuit\n");
    printf("Enter the initial data:\n");
    printf("The value of the first resistance -> ");
    scanf("%f", &R1);
    printf("The value of the second resistance -> ");
    scanf("%f", &R2);
    printf("Connection type (1-series, 2-parallel) -> ");
    scanf("%u", &choose);

    if (0 < choose && choose < 3) {
        if (choose == 1)
            R = R1 + R2;
        else
            R = R1*R2/(R1+R2);
    }
    else {
        printf("\nError: choose series or parallel connection\n");
        return -1;
    }

    printf("\nCircuit resistance: %.2f Om.\n", R);
    getchar();

    return 0;
}
```
79. Написать программу вычисления дохода по вкладу. Исходные данные: сумма и срок вклада. Процентная ставка зависит от суммы. Если сумма меньше 5000 руб., то процентная ставка 10%, если больше, то 13%. Далее приведен рекомендуемый вид экрана (данные, введенные пользователем, выделены полужирным)
```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    float amount, term;
    float annual_interest, income, end_amount;

    printf("Income\n");
    printf("Amount -> ");
    scanf("%f", &amount);
    printf("Deposit term -> ");
    scanf("%f", &term);

    if (amount < 5000)
        annual_interest = 10;
    else
        annual_interest = 13;

    income = amount * annual_interest/100/12 * term;
    end_amount = amount + income;

    printf("--------------------\n");
    printf("Amount: %.2f\n", amount);
    printf("Deposit term: %.2f\n", term);
    printf("Annual interest: %.2f\n", annual_interest);
    printf("Income: %.2f\n", income);
    printf("Amount at the end of the term of the deposit: %.2f\n", end_amount);

    return 0;
}
```
80. Написать программу вычисления дохода по вкладу. Исходные данные: сумма и срок вклада. Процентная ставка зависит от суммы. Если сумма меньше 5000 руб., то процентная ставка 9%, если больше 5000 руб., но меньше 10 000 руб., то 11%, а если больше 10 000, то 13%. Далее приведен рекомендуемый вид экрана (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    float amount, term;
    float annual_interest, income, end_amount;

    printf("Income\n");
    printf("Amount -> ");
    scanf("%f", &amount);
    printf("Deposit term -> ");
    scanf("%f", &term);

    if (amount < 5000)
        annual_interest = 10;
    else
        if (amount < 10000)
            annual_interest = 11;
        else
            annual_interest = 13;

    income = amount * annual_interest/100/12 * term;
    end_amount = amount + income;

    printf("--------------------\n");
    printf("Amount: %.2f\n", amount);
    printf("Deposit term: %.2f mon.\n", term);
    printf("Annual interest: %.2f\n", annual_interest);
    printf("Income: %.2f\n", income);
    printf("Amount at the end of the term of the deposit: %.2f\n", end_amount);

    return 0;
}
```
81. Написать программу вычисления стоимости печати фотографий. Формат фотографий 9x12 или 10x15. Если количество фотографий больше 10, то заказчику предоставляется скидка 5%. Далее приведен рекомендуемый вид экрана (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>
#include <conio.h>

int main()
{
    int format, quantity;
    float price, amount;
    float discount = 0, total;

    printf("PHOTO\n");
    printf("Format (1 - 9x12; 2 - 10x15) -> ");
    scanf("%i", &format);
    printf("Quantity, pcs. -> ");
    scanf("%i", &quantity);

    if (0 < format && format < 3) {
        if (format == 1)
            price = 2.50;
        else
            price = 3.20;
    }
    else {
        printf("Error\n");
        return -1;
    }

    amount = quantity * price;

    if (quantity > 10) {
        discount = amount * 0.05;
        total = amount - discount;
    }

    printf("--------------------\n");
    printf("Price: %f\n", price);
    printf("Quantity: %i pcs.\n", quantity);
    printf("Amount: %.2f\n", amount);
    if(discount != 0) {
        printf("Discount: %.2f\n", discount);
        printf("To pay: %.2f\n", total);
    }
    
    return 0;
}
```
82. Написать программу, которая вычисляет величину тока, потребляемого электроприбором (/ = P/U, где: I— ток, А; Р — мощность, Вт; U— напряжение, В). Программа должна проверять правильность введенных пользователем данных и, если они неверные (делитель равен нулю), выводить сообщение об ошибке. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float power, voltage, amperage;

    char c;

    printf("Current in electric circuit\n");
    printf("Power, W - > ");
    scanf("%f", &power);
    printf("Voltage, V - > ");
    scanf("%f", &voltage);

    if (voltage != 0) {
        amperage = power / voltage;
        printf("\nCurrent in circuit: %.2f A\n", amperage);
    }
    else
        printf("\nError! The voltage must not be zero\n");

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
83. Написать программу вычисления площади кольца. Программа должна проверять правильность исходных данных. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float r_ring, r_hole;
    float s;

    printf("Calculating the area of the ring\n");
    printf("Enter the initial data\n");
    printf("Radius of the ring (cm) -> ");
    scanf("%f", &r_ring);
    printf("radius of the hole (cm) - > ");
    scanf("%f", &r_hole);

    if (r_ring > r_hole) {
        s = 2 * 3.141592 * (r_ring-r_hole);
        printf("\nSquare of circle: %.2f sq. cm.\n", s);
    }
    else
        printf("\nError! The radius of the hole should not be larger than the radius of the rings\n");

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
84. Написать программу, которая переводит время из минут и секунд в секунды. Программа должна проверять правильность введенных пользователем данных и в случае, если данные неверные, выводить соответствующее сообщение. Далее приведен рекомендуемый вид экрана программы (ошибочные данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float time;
    int timeInSec, minutes, secondes;

    printf("Enter the time (minutes.seconds) -> ");
    scanf("%f", &time);

    minutes = time;
    secondes = (time - minutes) * 100;

    if (secondes > 60) {
        printf("\nError!\nThe number of seconds cannot be more than 60\n");
    }
    else {
        timeInSec = minutes * 60 + secondes;
        printf("%i min. %i sec. = %i sec\n", minutes, secondes, timeInSec);
    }
    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
85. Написать программу, которая проверяет, является ли год високосным. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int year;
    int r;

    printf("Enter the year\n-> ");
    scanf("%i", &year);

    r = year % 4;

    if (r) {
        printf("\n%i not leap year\n", year);
    }
    else {
        printf("%i is leap year\n", year);
    }

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
86. Написать программу решения квадратного уравнения. Программа должна проверять правильность исходных данных и в случае, если коэффициент при второй степени неизвестного равен нулю, выводить соответствующее сообщение. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <math.h>

int main()
{
    float a, b, c;
    float x1, x2;
    float d;

    printf("Solution of the quadratic equation\n");
    printf("Type the values of the coefficients in one line\n-> ");
    scanf("%f %f %f", &a, &b, &c);

    d = b*b - 4*a*c;

    if (d < 0) {
        printf("\nThe equation has no solution\n");
    }
    else {
        x1 = (-b + sqrt(d))/(2*a);
        x2 = (-b - sqrt(d))/(2*a);
        printf("\nThe roots of the equation:\n");
        printf("x1 = %.2f\n", x1);
        printf("x2 = %.2f\n", x2);
    }

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
87. Написать программу вычисления стоимости покупки с учетом скидки. Скидка в 10% предоставляется, если сумма покупки больше 1000 руб. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <math.h>

int main()
{
    float amount, total;
    int discount = 0;

    printf("Calculation of the purchase price taking into account the discount\n");
    printf("Purchase amount -> ");
    scanf("%f", &amount);

    if (amount > 1000) {
        discount = 10;
        total = amount - (amount/discount);
    }
    else {
        total = amount;
    }

    printf("You are given a discount of %i%%\n", discount);
    printf("Purchase amount including discount: %.2f\n", total);

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
88. Написать программу вычисления стоимости покупки с учетом скидки. Скидка в 3% предоставляется, если сумма покупки больше 500 руб, в 5% — если сумма больше 1000 руб. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <math.h>

int main()
{
    float amount, total;
    int discount = 0;

    printf("Calculating purchase price including discount\n");
    printf("Enter purchase amount -> ");
    scanf("%f", &amount);

    if (amount < 500) {
        total = amount;
    }
    else {
        if (amount < 1000) {
            discount = 3;
        }
        else
            discount = 5;
        total = amount - (amount/discount);
    }

    printf("You are given a discount of %i%%\n", discount);
    printf("Purchase amount including discount: %.2f\n", total);

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
89. Написать программу проверки знания истории — например, даты основания Санкт-Петербурга. В случае неправильного ответа пользователя программа должна выводить правильную дату. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int year;

    printf("In what year was St. Petersburg founded?\n");
    printf("Enter the number -> ");
    scanf("%i", &year);

    if (year == 1703)
        printf("Correct answer.\n");
    else
        printf("You are wrong. St. Petersburg was founded in 1703.\n");

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
90. Написать программу проверки знания даты начала Второй мировой войны. В случае неправильного ответа пользователя программа должна выводить правильную дату. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int year;

    printf("In what year did World War II begin?\n");
    printf("Enter the number -> ");
    scanf("%i", &year);

    if (year == 1939)
        printf("Correct.\n");
    else
        printf("You are wrong. World War II began in 1939.\n");

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
91. Написать программу проверки знания истории архитектуры. Программа должна вывести вопрос и три варианта ответа. Пользователь должен выбрать правильный ответ и ввести его номер. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int var;

    printf("Architect of St. Isaac's Cathedral:\n");
    printf("1. Domenico Trezzini\n");
    printf("2. Auguste Ionferrand\n");
    printf("3. Carl Rossi\n");
    printf("Enter the correct answer\n-> ");
    scanf("%i", &var);

    if (var == 2)
        printf("Correct.\n");
    else
        printf("You are wrong. Architect of St. Isaac's Cathedral - Auguste Ionferrand\n");

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
92. Написать программу проверки знания истории архитектуры. Программа должна вывести вопрос и три варианта ответа. Пользователь должен выбрать правильный ответ и ввести его номер. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int var;

    printf("Nevsky Prospekt got its name:\n");
    printf("1. Named after the river on the banks of which is located St. Petersburg.\n");
    printf("2. Named after the nearby monastery of the Alexander Nevsky Lavra.\n");
    printf("3. In memory of the 6 famous commander Alexander Nevsky.\n");
    printf("Enter the correct answer\n-> ");
    scanf("%i", &var);

    if (var == 2)
        printf("Correct.\n");
    else {
        printf("You are wrong.\n");
        printf("Correct answer: 2\n");
    }
    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
93. Написать программу, которая сравнивает два введенных с клавиатуры числа. Программа должна указать, какое число больше, или, если числа равны, вывести соответствующее сообщение. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int i1, i2;

    printf("Enter two integers in one line\n-> ");
    scanf("%i %i", &i1, &i2);

    if (i1 < i2)
        printf("%i less than %i\n", i1, i2);
    else if (i1 > i2)
        printf("%i more than %i\n", i1, i2);
    else
        printf("The numbers are equal\n");

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
94. Написать программу, которая выводит пример на умножение двух однозначных чисел, запрашивает ответ пользователя, проверяет его и выводит сообщение «Правильно!» или «Вы ошиблись» и правильный результат. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int m1, m2, p;
    int answer;
    time_t t;

    srand((unsigned) time(&t));

    m1 = rand() % 9 + 1;
    m2 = rand() % 9 + 1;

    p = m1 * m2;


    printf("How much will %ix%i be?", m1, m2);
    printf("Enter the answer -> ");
    scanf("%i", &answer);

    if (answer == p)
        printf("Correct.\n");
    else
        printf("You are wrong. %ix%i=%i\n", m1, m2, p);

    printf("Press <Enter> to continue");
    fflush(stdin);
    getchar();

    return 0;
}
```
95. Написать программу, которая выводит пример на вычитание (в пределах 100), запрашивает ответ пользователя, проверяет его и выводит сообщение «Правильно!» или «Вы ошиблись» и правильный результат. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int a, b;
    int res;
    int answer;

    srand(time(NULL));

    a = rand() % 100 + 1;
    b = rand() % 100 + 1;
    res = a - b;

    printf("How much %i-%i?\n", a, b);
    printf("Enter the answer -> ");
    scanf("%i", &answer);

    if (answer == res)
        printf("Correct!\n");
    else
        printf("You are wrong. %i-%i=%i %i\n", a, b, res, answer);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
96. Написать программу, которая проверяет, является ли введенное пользователем целое число четным. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int answer;

    printf("Enter an integer -> ");
    scanf("%i", &answer);

    if (answer % 2 == 0)
        printf("The number %i is even\n", answer);
    else
        printf("The number %i is odd\n", answer);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
97. Написать программу, которая проверяет, делится ли на три введенное с клавиатуры целое число. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int answer;

    printf("Enter an integer -> ");
    scanf("%i", &answer);

    if (answer % 3 == 0)
        printf("%i is divisible by three\n", answer);
    else
        printf("%i is not divisible by three\n", answer);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
98. Написать программу вычисления стоимости разговора по телефону с учетом 20%-ной скидки, предоставляемой по субботам и воскресеньям. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int time;
    int day;
    float amount;

    printf("Calculating the cost of a telephone call\n");
    printf("Enter the initial data:\n");
    printf("Duration of the call -> ");
    scanf("%i", &time);
    printf("Day of the week -> ");
    scanf("%i", &day);

    amount = 2.3 * time;

    if (day == 6 || day == 7) {
        printf("Discount 20%\n");
        amount = amount * 0.8;
    }
    printf("The cost: %.2f\n", amount);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
99. Написать программу, которая вычисляет оптимальный вес человека, сравнивает его с реальным и выдает рекомендацию о необходимости поправиться или похудеть. Оптимальный вес вычисляется по формуле: Рост (см) - 100. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float w;
    float h;
    float opt;
    float d;

    printf("Enter in one line, with a space, height (cm) and weight (kg)\n-> ");
    scanf("%f %f", &h, &w);

    opt = h - 100;

    if (w == opt) {
        printf("Your weight is optimal\n");
    }
    else if (w < opt) {
        d = opt - w;
        printf("You need to recover by %.2f kg.\n", d);
    }
    else {
        d = w - opt;
        printf("You need to recover by %.2f kg.\n", d);
    }

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
100. Написать программу, которая запрашивает у пользователя номер месяца и затем выводит соответствующее название времени года. Если пользователь введет недопустимое число, программа должна вывести сообщение «Ошибка данных». Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int month;

    puts("Enter number of month (1 - 12)");
    printf("-> ");
    scanf("%i", &month);

    if (month < 1 || month > 12)
        printf("Enter number between 1 - 12\n");
    else if (month >= 3 && month <= 5)
        printf("Spring\n");
    else if (month >= 6 && month <= 8)
        printf("Summer\n");
    else if (month >= 9 && month <= 11)
        printf("Autumn\n");
    else
        printf("Winter\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
101. Написать программу, которая запрашивает у пользователя номер дня недели и выводит одно из сообщений: «Рабочий День», «Суббота» или «Воскресенье.
```
#include <stdio.h>

int main()
{
    int day;

    printf("Enter number of week -> ");
    scanf("%i", &day);

    if (day < 1 || day > 7)
        printf("Enter number between 1 - 7\n");
    else if (day == 6)
        printf("Saturday\n");
    else if (day == 7)
        printf("Sunday\n");
    else
        printf("Weekdays\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
102. Написать программу, которая отображает введенное пользователем число (от 1 до 999) в денежном формате: дописывает слово «рубль» в правильной форме— например, 12 рублей, 21 рубль и т. д.
```
#include <stdio.h>

int main()
{
    int n;
    int r;

    printf("Enter an integer, no more than 999 -> ");
    scanf("%i", &n);
    printf("%i ", n);

    if (n > 100)
        r = n % 100;
    else
        r = n;

    if (r >= 11 && r <= 14)
        printf("rubley\n");
    else {
        r = r % 10;
        if (r >= 2 && r <= 4)
            printf("rublya\n");
        else if (r == 1)
            printf("ruble\n");
        else
            printf("rubley");
    }

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
103. Написать программу, которая после введенного с клавиатуры числа (в диапазоне от 1 до 99), обозначающего денежную единицу, дописывает слово «копейка» в правильной форме — например, 5 копеек, 41 копейка и т. д.
```
#include <stdio.h>

int main()
{
    int n;

    printf("Enter an integer, no more than 99 -> ");
    scanf("%i", &n);
    printf("%i ", n);

    if (n == 1)
        printf("kopeyka\n");
    else if (n >= 2 && n <= 4)
        printf("kopeyki\n");
    else
        printf("kopeek\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
104. Написать программу, которая вычисляет дату следующего дня. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int day;
    int month;
    int year;
    int last = 0;
    int r;

    printf("Enter today's date in numbers in one line (number month year) -> ");
    scanf("%i %i %i", &day, &month, &year);

    if (month == 2) {
        if ((year % 4) != 0 && day == 28) last = 1;
        if ((year % 4) == 0 && day == 29) last = 1;
    }
    else if ((month == 4 || month == 6 || month == 9 || month == 11)
             && (day == 31))
                last = 1;
    else if (day == 31)
        last = 1;

    if (last == 1) {
        printf("Last day in month!\n");
        day = 1;
        if (month == 12) {
            month = 1;
            ++year;
            printf("Happy New Year!\n");
        }
        else
            ++month;
    }
    else
        ++day;

    printf("Tomorrow %i %i %i\n", day, month, year);

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
105. Написать программу, которая позволяет вычислить цену жалюзи. Исходные данные: размер (ширина и высота, выраженные в сантиметрах) и тип материала (пластик, текстиль, алюминий). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float w, h;
    int m;

    float price;
    float s;
    float amount;

    printf("Blinds\n");

    printf("Width -> ");
    scanf("%f", &w);
    printf("Height -> ");
    scanf("%f", &h);

    printf("Material:\n");
    printf("1 - plastic\n");
    printf("2 - textile\n");
    printf("3 - aluminum\n");
    scanf("%i", &m);

    switch (m) {
    case 1:
        price = 200;
        break;
    case 2:
        price = 250;
        break;
    case 3:
        price = 350;
        break;
    default:
        price = 0;
        break;
    }

    if (price != 0) {
        s = (w * h) / 10000;
        amount = s * price;
        printf("Price for sq. m.: %.2f\n", price);
        printf("Square: %.2f sq. m.\n", s);
        printf("To payment: %.2f\n", amount);
    }
    else
        printf("The material is not specified correctly\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
106. Написать программу, которая позволяет вычислить стоимость печати фотографий. Исходные данные: размер фотографий (9x12, 10x15 или 18x24) и их количество. Если заказанных фотографий больше 10, заказчику должна предоставляться скидка 10%. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int format, quantity;

    float price;
    float amount;
    float discount;
    float total;

    printf("Photo\n");

    printf("Size:\n");
    printf("1 - 9x12\n");
    printf("2 - 10x15\n");
    printf("3 - 18x24\n");
    printf("Your choice -> ");
    scanf("%i", &format);
    printf("Quantity -> ");
    scanf("%i", &quantity);

    switch (format) {
    case 1:
        price = 3.50;
        break;
    case 2:
        price = 5.00;
        break;
    case 3:
        price = 8.50;
        break;
    default:
        price = 0;
        break;
    }

    if (price != 0) {
        amount = quantity * price;
        printf("Price: %.2f\n", price);
        printf("Quantity: %i\n", quantity);
        if (quantity > 10) {
            discount = amount * 0.1;
            total = amount - discount;
            printf("Amount: %.2f\n", amount);
            printf("Discount: %.2f\n", discount);
            printf("Total: %.2f\n", total);
        }
        else
            printf("To pay: %.2f\n", total);
    }
    else
        printf("Material code is incorrect\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
107. Написать программу, которая позволяет вычислить стоимость заправки автомобиля. Исходные данные: тип топлива (бензин 92, 95, 98 или дизельное топливо) и количество литров. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int brand;
    float price;

    float liters;
    float amount;

    printf("Petrol\n");
    printf("Petrol brand:\n");
    printf("1 - 92\n");
    printf("2 - 95\n");
    printf("3 - 98\n");
    printf("4 - DT\n");
    printf("Your choice -> ");
    scanf("%i", &brand);
    printf("Liters -> ");
    scanf("%f", &liters);

    switch (brand) {
    case 1:
        price = 17.50;
        break;
    case 2:
        price = 20.30;
        break;
    case 3:
        price = 25.40;
        break;
    case 4:
        price = 18.50;
        break;
    default:
        price = 0;
        break;
    }

    if (price != 0) {
        amount = liters * price;
        printf("Price per liter: %.2f\n", price);
        printf("Liters: %.2f\n", liters);
        printf("To pay: %.2f\n", amount);
    }
    else
        printf("The fuel code is incorrect\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
108. Написать программу, которая запрашивает у пользователя номер дня недели и затем выводит его название. Если введены неправильные данные, программа должна вывести сообщение об ошибке.
```
#include <stdio.h>

int main()
{
    int nd;

    puts("Enter number of week (1..7)");
    printf("-> ");
    scanf("%i", &nd);

    switch (nd) {
    case 1:
        puts("Monday\n");
        break;
    case 2:
        puts("Tuesday\n");
        break;
    case 3:
        puts("Wednesday\n");
        break;
    case 4:
        puts("Thursday\n");
        break;
    case 5:
        puts("Friday\n");
        break;
    case 6:
        puts("Saturday\n");
        break;
    case 7:
        puts("Sunday\n");
        break;
    default:
        puts("Enter number between 1..7\n");
        break;
    }

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
109. Написать программу, которая вычисляет доход по вкладу. Процентная ставка зависит от срока вклада:
```
#include <stdio.h>

int main()
{
    float val;
    int period;
    float rate;
    float profit;

    printf("Value -> ");
    scanf("%f", &val);
    printf("Period -> ");
    scanf("%i", &period);

    switch (period) {
    case 3:
        rate = 9.0;
        break;
    case 6:
        rate = 11.5;
        break;
    case 12:
        rate = 13.5;
        break;
    case 18:
        rate = 15.0;
        break;
    case 24:
        rate = 18.0;
        break;
    case 36:
        rate = 24;
        break;
    default:
        period = 0;
        break;
    }

    if (period != 0) {
        printf("Rate: %.2f\n", rate);
        profit = val * rate/100/2 * period;
        printf("Profit: %.2f\n", profit);
    }
    else
        printf("Not valid period\n");

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
110. Написать программу, которая вычисляет стоимость междугороднего телефонного разговора (цена одной минуты зависит от расстояния до города, в котором находится абонент). Исходные данные для программы: код города и длительность разговора. Далее приведены коды некоторых городов и рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int code;
    float price;
    int duration;
    float amount;

    printf("Calculation of the cost of a phone call\n");
    printf("Enter the initial data:\n");
    puts("Vladivostok\t432");
    puts("Moscow\t\t495");
    puts("Murmansk\t815");
    puts("Samara\t\t846");
    printf("Area code -> ");
    scanf("%i", &code);
    printf("Call duration (whole number of minutes) -> ");
    scanf("%i", &duration);

    printf("City: ");
    switch (code) {
    case 432:
        puts("Vladivostok");
        price = 2.2;
        break;
    case 495:
        puts("Moscow");
        price = 1;
        break;
    case 815:
        puts("Murmansk");
        price = 1.2;
        break;
    case 846:
        puts("Samara");
        price = 1.4;
        break;
    default:
        printf("Invalid code entered\n");
        break;
    }

    if (price != 0) {
        amount = price * duration;
        printf("Price per minute: %.2f\n", price);
        printf("Call cost: %.2f\n", amount);
    }

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
111. Написать программу, которая по дате определяет соответствующий ей день недели. Для вычисления дня недели воспользуйтесь формулой: d = (day+(13*m-1)/5+y+y/4+c/4-2*c+777)%7;
```
#include <stdio.h>

int main()
{
    int day, month, year;

    int c, y;
    int m;
    int d;

    puts("Determination of the day of the week by date\n");
    puts("Enter date: day month year");
    puts("For example: 5 12 2001");
    printf("-> ");
    scanf("%i %i %i", &day, &month, &year);

    if (month == 1 || month == 2)
        --year;

    m = month - 2;
    if (m <= 0) m += 12;
    c = year / 100;
    y = year - c*100;

    d = (day+(13*m-1)/5+y+y/4+c/4-2*c+777)%7;

    switch (d) {
    case 1: puts("Monday"); break;
    case 2: puts("Tuesday"); break;
    case 3: puts("Wednesday"); break;
    case 4: puts("Thursday"); break;
    case 5: puts("Friday"); break;
    case 6: puts("Saturday"); break;
    case 0: puts("Sunday");
    }

    printf("Press <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
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
#include <stdio.h>

int main()
{
    float price;
    float total;

    printf("Enter price per kg\n-> ");
    scanf("%f", &price);

    printf("Weight\t\tPrice\n");

    for (int i = 1; i <= 10; ++i) {
        total = price*(i*100)/1000;
        printf("%i\t\t%.2f\n", i, total);
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
133. Написать программу, которая выводит таблицу значений функции у = | х |. Диапазон изменения аргумента от -4 до 4, шаг приращения аргумента 0,5.
```
#include <stdio.h>
#include <math.h>

#define LB -4
#define HB 4
#define DX 0.5

int main()
{
    float x, y;
    int n;
    int i;

    printf("Table of func. values y = |x|\n");
    n = (HB - LB)/DX + 1;
    x = LB;

    for (i = 1; i <= n; ++i) {
        y = fabs(x);
        printf("%4.2f\t%3.2f\n", x, y);
        x += DX;
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
134. Написать программу, которая выводит таблицу значений функции у = | х - 2 | + | х + 1 |. Диапазон изменения аргумента от -4 до 4, шаг приращения аргумента 0,5.
```
#include <stdio.h>
#include <math.h>

#define LB -4
#define HB 4
#define DX 0.5

int main()
{
    float x, y;
    int n;
    int i;

    printf("Table of func. values y = |x-2|+|x+1|\n");
    n = (HB - LB)/DX + 1;
    x = LB;

    for (i = 1; i <= n; ++i) {
        y = fabs(x - 2) + fabs(x + 1);
        printf("%.2f\t\t%.2f\n", x, y);
        x += DX;
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
135. Написать программу, которая выводит на экран таблицу умножения, например, на 7. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>

int main()
{
    int m;

    int n;
    int p;

    m = 7;
    printf("Multiplication table\n");
    for (n = 1; n <= 9; ++n) {
        p = m * n;
        printf("%ix%i=%i\n", m, n, p);
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
136. Написать программу, которая выводит на экран квадрат Пифагора— таблицу умножения. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>

int main()
{
    int i, j;

    printf("%4s", " ");
    for (j = 1; j <= 10; ++j)
        printf("%4i", j);
    printf("\n");

    for (i = 1; i <= 10; ++i) {
        for (j = 1; j <= 10; ++j) {
            if (j == 1)
                printf("%4i", i);
            printf("%4i", i*j);
        } printf("\n");
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
137. Написать программу, которая вычисляет частичную сумму ряда: 1 - 1/3 + 1/5 - 1/7 + 1/9... и сравнивает полученное значение с я/4 (при суммировании достаточно большого количества членов этого ряда, величина частичной суммы приближается к я/4).
```
#include <stdio.h>

int main()
{
    float x;
    int n;
    float sum;
    int i;

    printf("Calculation of the number ""PI"" using\n");
    printf("the properties of the series 1 -1/3 + 1/5 - 1/7 + ...\n");
    printf("Enter the number of summed members of the series -> ");
    scanf("%i", &n);
    sum = 0;
    for (i = 1; i <= n; ++i) {
        x = (float)1/(2*i - 1);

        if ((i % 2) == 0) x = -1 * x;
        sum += x;
    }

    printf("Sum of the series: %2.6f\n", sum);
    printf("Calculated value of PI = %2.6f\n", sum*4);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
138. Написать программу приближенного вычисления интеграла функции XX) = 5х2-х + 2 методом прямоугольников. Диапазон xl, х2 и шаг изменения аргумента Ах должны задаваться во время работы программы.
```
#include <stdio.h>

int main()
{
    float a, b;
    float dx;
    float s;
    int n;
    float x;
    float y;

    printf("Approximate calculation of the integral\n");
    printf("Lower bound of the range -> ");
    scanf("%f", &a);
    printf("Upper bound of the range -> ");
    scanf("%f", &b);
    printf("Argument equals -> ");
    scanf("%f", &dx);

    n = (b - a) / dx + 1;
    x = a;
    s = 0;

    for (int i = 1; i <= n; ++i) {
        y = x*x + 2;
        s += y*dx;
        x += dx;
    }

    printf("Integral value: %.2f\n", s);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
139. Написать программу приближенного вычисления интеграла функции Дх) = 5х2 - х + 2 методом трапеций. Границы интервала xl, х2 и шаг приращения аргумента Дх должны задаваться во время работы программы.
```
#include <stdio.h>

int main()
{
    float a, b;
    float dx;
    float s;
    int n;
    float x;
    float y1, y2;
    int i;

    printf("Approximate calculation of the integral\n");
    printf("Lower bound of the range -> ");
    scanf("%f", &a);
    printf("Upper bound of the range -> ");
    scanf("%f", &b);
    printf("Argument equals -> ");
    scanf("%f", &dx);

    n = (b - a) / dx;
    x = a;
    s = 0;

    for (i = 1; i <= n; ++i) {
        y1 = x*x + 2;
        x += dx;
        y2 = x*x + 2;
        s += (y1 + y2)*dx/2;
    }

    printf("Integral value: %6.3f\n", s);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
140. Написать программу, которая выводит на экран изображение шахматной доски. Черные клетки отображать «звездочкой», белые — пробелом. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>

int main()
{
    for (int i = 1; i < 10; ++i) {
        if (i % 2)
            printf(" ");
        printf("*****\n");
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
141. Написать программу, которая преобразует введенное пользователем десятичное число в двоичное. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int dec;
    int v;
    int i;

    printf("Decimal to Binary Conversion\n");
    printf("Enter an integer from 0 to 255 and press <Enter> -> ");
    scanf("%i", &dec);
    printf("Decimal %i is binary ", dec);

    v = 128;

    for (i = 1; i <= 8; ++i) {
        if (dec >= v) {
            printf("1");
            dec -= v;
        }
        else printf("0");
        v = v / 2;
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
142.  Написать программу проверки знания таблицы умножения. Программа должна вывести 10 примеров и выставить оценку: за 10 правильных ответов — «отлично», за 9 и 8 — «хорошо», за 7 и 6 — «удовлетворительно», за 6 и менее — «неудовлетворительно». Далее приведен рекомендуемый вид экрана программы (ответы пользователя выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int numb1, numb2;
    int res;
    int ans;
    int cnt = 0;

    printf("");
    printf("");

    srand(time(NULL));

    for (int i = 1; i <= 10; ++i) {
        numb1 = rand() % 7 + 2;
        numb2 = rand() % 7 + 2;
        res = numb1 * numb2;
        printf("%ix%i=", numb1, numb2);
        scanf("%i", &ans);
        if (ans == res)
            ++cnt;
        else
            printf("You are wrong. %ix%i=%i\nGo next\n", numb1, numb2, res);
    }
    printf("Correct ans: %i\n", cnt);
    printf("Your mark: ");

    switch (cnt) {
    case 10:
        puts("5"); break;
    case 9:
        puts("4"); break;
    case 8:
        puts("4"); break;
    case 7:
        puts("2"); break;
    default:
        puts("2"); break;
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
143. Написать программу проверки умения складывать и вычитать числа в пределах 100. Программа должна вывести 10 примеров, причем в каждом примере на вычитание уменьшаемое должно быть больше или равно вычитаемому, т. е. не допускается предлагать испытуемому примеры с отрицательным результатом. Оценка выставляется по следующему правилу: за 10 правильных ответов — «отлично», за 9 и 8 — «хорошо», за 7 и 6 — «удовлетворительно», за 6 и менее — «плохо». Далее приведен рекомендуемый вид экрана программы (ответы пользователя выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

#define LEVEL 97+2

int main()
{
    int numb1, numb2;
    int op;

    int zop;
    int res;
    int otv;
    int cnt = 0;
    int buf;

    printf("");
    printf("");

    srand(time(NULL));

    for (int i = 1; i <= 10; ++i) {
        numb1 = rand() % LEVEL;
        numb2 = rand() % LEVEL;
        op = rand()%2;
        if (op == 0) {
            res = numb1 + numb2;
            zop = '+';
        }
        else {
            zop = '-';
            if (numb1 < numb2) {
                buf = numb2;
                numb2 = numb1;
                numb1 = buf;
            }
            res = numb1 - numb2;
        }
        printf("%i%c%i=", numb1, zop, numb2);
        scanf("%i", &otv);
        if (otv == res)
            ++cnt;
        else
            printf("You are wrong. %i%c%i=%i\n", numb1, zop, numb2, res);
    }

    printf("Correct ans: %i\n", cnt);
    printf("Your mark: ");

    switch (cnt) {
    case 10:
        puts("5"); break;
    case 9:
        puts("4"); break;
    case 8:
        puts("4"); break;
    case 7:
        puts("2"); break;
    default:
        puts("2"); break;
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
144. Написать программу, которая проверяет знание таблицы умножения. Программа должна вывести 10 примеров Оценка выставляется по следующему правилу: за 10 правильных ответов — «отлично», за 9 и 8 — «хорошо», за 7 и 6 — «удовлетворительно», за 6 и менее — «плохо». Программа должна вывести 10 примеров и после последнего ответа вывести оценку. Если в процессе тестирования количество ошибок достигнет 5 (т. е. получить положительную оценку испытуемый уже точно не сможет), то процесс тестирования должен быть прекращен.
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

#define LEVEL 97+2

int main()
{
    int numb1, numb2;
    int op;

    int zop;
    int res;
    int otv;
    int cnt = 0;
    int buf;

    printf("");
    printf("");

    srand(time(NULL));

    for (int i = 1; i <= 10; ++i) {
        numb1 = rand() % LEVEL;
        numb2 = rand() % LEVEL;
        op = rand()%2;
        if (op == 0) {
            res = numb1 * numb2;
            zop = '*';
        }
        else {
            zop = '/';
            if (numb1 < numb2) {
                buf = numb2;
                numb2 = numb1;
                numb1 = buf;
            }
            res = numb1 / numb2;
        }
        printf("%i%c%i=", numb1, zop, numb2);
        scanf("%i", &otv);
        if (otv == res)
            ++cnt;
        else
            printf("You are wrong. %i%c%i=%i\n", numb1, zop, numb2, res);
    }

    printf("Correct ans: %i\n", cnt);
    printf("Your mark: ");

    switch (cnt) {
    case 10:
        puts("5"); break;
    case 9:
        puts("4"); break;
    case 8:
        puts("4"); break;
    case 7:
        puts("2"); break;
    default:
        puts("2"); break;
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
145. Написать программу, которая выводит на экран таблицу значений функции у = -2,4х2+ 5х-3. Диапазон и шаг изменения аргумента должны задаваться во время работы программы. Далее приведен рекомендуемый вид экрана программы.
```
#include <stdio.h>

int main()
{
    float x, y;
    float x1, x2, dx;

    printf("x1 -> ");
    scanf("%f", &x1);
    printf("x2 -> ");
    scanf("%f", &x2);
    printf("dx -> ");
    scanf("%f", &dx);

    x = x1;
    printf("-----------------------\n");
    printf("     x     |      y    \n");
    printf("-----------------------\n");
    do {
        y = -2.4*x*x+5*x-3;
        printf("%9.2f  | %9.2f\n", x, y);
        x += dx;
    }
    while (x <= 2);

    printf("-----------------------\n");

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
146. Написать программу, которая выводит на экран таблицу соответствия температуры в градусах Цельсия и Фаренгейта (7?°= 5/9 С°+32). Диапазон изменения температуры в градусах Цельсия и шаг должны вводиться во время работы программы. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    float t1, t2, dt;
    float c, f;

    printf("t1 -> ");
    scanf("%f", &t1);
    printf("t2 -> ");
    scanf("%f", &t2);
    printf("dt -> ");
    scanf("%f", &dt);

    c = t1;
    printf("-----------------------\n");
    printf("     C     |      F    \n");
    printf("-----------------------\n");
    do {
        f = 9.0/5 * c + 32;
        printf("%9.2f  | %9.2f\n", c, f);
        c += dt;
    }
    while (c <= t2);

    printf("-----------------------\n");

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
147. Написать программу, вычисляющую сумму и среднее арифметическое последовательности положительных чисел, которые вводятся с клавиатуры. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int a;
    int n;
    int s;
    float m;

    s = 0;
    n = 0;

    printf("Calculating Avg. mean\n");
    printf("Enter numbers. To complete press <Enter>\n");

    do {
        printf("-> ");
        scanf("%i", &a);
        if (a > 0) {
            s += a;
            ++n;
        }
    }
    while (a > 0);

    printf("Numbers Entered: %i\n", n);
    printf("Sum of numbers: %i\n", s);
    m = (float) s / n;
    printf("Avg. Mean: %3.2f\n", m);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
148. Написать программу, которая определяет максимальное число из введенной с клавиатуры последовательности положительных чисел (длина последовательности не ограничена). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int a;
    int m;

    puts("Defines max number\n");
    puts("Enter numbers; To complete enter 0\n");
    m = 0;
    do {
        printf("-> ");
        scanf("%i", &a);
        if (a > m)
            m = a;
    }
    while (a > 0);
    printf("Max number: %i\n", m);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
149. Написать программу, которая определяет минимальное число во введенной с клавиатуры последовательности положительных чисел (длина последовательности не ограничена). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int a;
    int minimum;

    printf("Defines minimum number\n");
    printf("Enter numbers. To complete enter 0\n");
    printf("-> ");
    scanf("%i", &a);
    minimum = a;
    while (a > 0) {
        if (a < minimum) minimum = a;
        printf("-> ");
        scanf("%i", &a);
    }
    printf("Minimum number: %i\n", minimum);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
150. Написать программу, которая проверяет, является ли введенное пользователем целое число простым (простым называется число, которое делится только на единицу и на само себя). Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

int main()
{
    int n;
    int d;
    int r;

    printf("Enter whole number and press <Enter>\n-> ");
    scanf("%i", &n);
    d = 2;
    do {
        r = n % d;
        if (r != 0) ++d;
    }
    while (r != 0);
    if (d == n)
        printf("%i - simply number\n", n);
    else printf("%i - not simply number\n", n);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
151. Написать программу приближенного вычисления интеграла методом прямоугольников. Интервал и точность вычисления должны задаваться во время работы программы, функция — в программе. После каждого цикла вычислений программа должна выводить вычисленное значение интеграла.
```
#include <stdio.h>
#include <math.h>

int main()
{
    float x1, x2;
    float e;

    float dx;
    float n;
    float x;
    float y;
    float st;
    float sp;

    int i;

    printf("Calculating integral\n");
    printf("Low edge -> ");
    scanf("%f", &x1);
    printf("Up edge -> ");
    scanf("%f", &x2);

    printf("Accuracy - > ");
    scanf("%f", &e);

    dx = 0.5;
    st = 0;

    do {
        sp = st;
        dx = dx / 2;
        n = (x2 - x1) / dx;
        x = x1;
        st = 0;
        for (i = 0; i <= n; ++i) {
            y = x + 2;
            st = st + (y * dx);
            x += dx;
        }
        printf("Value of integral: %6.3f\n", st);
    }
    while (abs(sp - st) > e);

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
152. Написать программу, которая «задумывает» число в диапазоне от 1 до 10 и предлагает пользователю угадать его за пять попыток. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
#include <conio.h>

int main()
{
    int comp;
    int player;
    int n;
    time_t t;

    srand((unsigned) time(&t));
    comp = rand() % 10 + 1;

    system("cls");
    printf("Computer number 1...10\n\r");
    printf("You should guess in 5 try\n");
    printf("Enter number and press <Enter>\n");
    n = 0;
    do {
        printf("\n\r-> ");
        scanf("%i", &player);
        ++n;
    }
    while ((player != comp) && (n < 3));

    if (player == comp) {
        printf("\n\rYou Win! Congratulations!");
    }
    else {
        printf("\n\rYou Lose");
        printf("PC think number %d", comp);
    }

    printf("\nPress <Enter> to close\n");
    fflush(stdin);
    getchar();

    return 0;
}
```
153. Написать программу приближенного вычисления интеграла методом трапеций. Интервал и точность вычисления должны задаваться во время работы программы. После каждого цикла вычислений программа должна выводить вычисленное значение интеграла, число интервалов и шаг изменения аргумента.
```
```
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
#include <stdio.h>

#define ROW 3
#define COL 5

int main()
{
    int a[ROW][COL];
    int s[COL];
    int i, j;

    for (i = 0; i < ROW; ++i) {
        printf("-> ");
        for (j = 0; j < COL; ++j)
            scanf("%i", &a[i][j]);
    }

    for (i = 0; i < ROW; ++i) {
        for (j = 0; j < COL; ++j)
            printf("%i ", a[i][j]);
        printf("\n");
    }

    for (i = 0; i < COL; ++i)
        s[i] = 0;

    for (j = 0; j < COL; ++j)
        for (i = 0; i < ROW; ++i)
            s[j] += a[i][j];

    printf("----------------------\n");

    for (i = 0; i < COL; ++i)
        printf("%i ", s[i]);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
174. Написать программу, которая вводит по строкам с клавиатуры двумерный массив и вычисляет сумму его элементов по строкам.
```
#include <stdio.h>

#define ROW 3
#define COL 3

int main()
{
    int a[ROW][COL];
    int s[COL];
    int i, j;

    for (i = 0; i < ROW; ++i) {
        printf("-> ");
        for (j = 0; j < COL; ++j)
            scanf("%i", &a[i][j]);
    }

    for (i = 0; i < ROW; ++i) {
        for (j = 0; j < COL; ++j)
            printf("%i ", a[i][j]);
        printf("\n");
    }

    for (i = 0; i < COL; ++i)
        s[i] = 0;

    for (i = 0; i < COL; ++i)
        for (j = 0; j < ROW; ++j)
            s[i] += a[i][j];

    printf("----------------------\n");

    for (i = 0; i < COL; ++i)
        printf("%i ", s[i]);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
175. Написать программу, которая обрабатывает результаты экзамена. Для каждой оценки программа должна вычислить процент от общего количества оценок. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

#define ROW 3
#define COL 3

int main()
{
    int n[6];
    int s = 0;
    float p[6];

    char *mes[6] = {"\0", "\0", "2\0", "3\0", "4\0", "5\0"};

    int i;

    for (i = 5; i >= 2; --i) {
        printf("%s -> ", mes[i]);
        scanf("%i", &n[i]);
        s += n[i];
    }

    for (i = 2; i < 6; ++i)
        p[i] = (float)n[i]/s*100;

    for (i = 5; i >= 2; --i)
        printf("%-8s %2i  %2.0f\n", mes[i], n[i], p[i]);


    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
176. Написать программу, которая вводит по строкам с клавиатуры двумерный массив дробного типа (3x5— три строки по пять элементов) и вычисляет среднее арифметическое элементов строк. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>

#define ROW 3
#define COL 3

int main()
{
    int a[3][5];
    int r;
    int c;

    int sum;
    float m;

    int k;

    k = 1;
    for (r = 0; r < 3; ++r) {
        printf("S %i -> ", k);
        for (c = 0; c < 5; ++c) {
            scanf("%i", &a[r][c]);
        }
        ++k;
    }

    for (r = 0; r < 3; ++r) {
        for (c = 0; c < 5; ++c)
            printf("%5i ", a[r][c]);
        printf("\n");
    }

    k = 1;
    for (r = 0; r < 3; ++r) {
        sum = 0;
        for (c = 0; c < 5; ++c)
            sum = sum + a[r][c];
        m = (float)sum/5;
        printf("S %i: %5.2f\n", k, m);
        ++k;
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
177. Написать программу, которая определяет номер строки двумерного массива, сумма элементов которой максимальна.
```
#include <stdio.h>

#define N 3

int main()
{
    int m[N][N+1];

    int mx;

    int i, j;

    for (i = 0; i < N; ++i) {
        printf("E %i -> ", i+1);
        for (j = 0; j < N; ++j)
            scanf("%i", &m[i][j]);
    }

    for (i = 0; i < N; ++i) {
        m[i][N] = 0;
        for (j = 0; j < N; ++j)
            m[i][N] += m[i][j];
    }

    mx = 0;
    for (i = 1; i < N; ++i)
        if (m[i][N] > m[mx][N])
            mx = i;

    printf("%i S sum", mx+1);
    printf("max %i\n", m[mx][N]);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
178. Написать программу, которая проверяет, является ли введенная с клавиатуры квадратная матрица «магическим квадратом». Магическим квадратом называется матрица, у которой сумма чисел в каждом горизонтальном ряду, в каждом вертикальном и по каждой из диагоналей одна и та же (см. приведенный далее рисунок).
```
#include <stdio.h>

#define SZ 5

int main()
{
    int a[SZ][SZ];
    int n;
    int ok;
    int i, j;
    int sum;
    int temp;

    printf("(3..%i) -> ", SZ);
    scanf("%i", &n);

    for (i = 0; i < n; ++i) {
        printf("-> ");
        for (j = 0; j < n; ++j)
            scanf("%i", &a[i][j]);
    }

    ok = 1;
    sum = 0;

    for (i = 0; i < n; ++i)
        sum += a[i][i];

    i = 0;
    do {
        temp = 0;
        for (j = 0; j < n; ++j)
            temp += a[i][j];
        if (temp != sum) ok = 0;
        ++i;
    } while (ok && i < n);

    if (ok) {
        j = 0;
        do {
            temp = 0;
            for (i = 0; i < n; ++i)
                temp += a[i][j];
            if (temp != sum) ok = 0;
            ++j;
        } while (ok && j < n);
    }

    if (ok) {
        temp = 0;
        i = n - 1;
        for (j = 0; j < n; ++j)
            temp += a[i--][j];
        if (temp != sum) ok = 0;
    }

    if (!ok)
        printf("Not ");
    printf("magic square\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
179. Написать программу, которая вычисляет доход по вкладу. Процентная ставка по вкладу определяется на основе данных, приведенных в таблице.
```
#include <stdio.h>

int main()
{
    float rate[3][6] = {15.0, 16.5, 18.0, 19.5, 21.0, 22.0,
                        16.5, 18.0, 19.5, 21.0, 22.5, 24.0,
                        18.5, 19.5, 21.0, 22.5, 24.0, 27.0};

    float value;
    int period;
    float profit;

    int r, c;

    for (int r = 0; r < 3; ++r) {
        for (int c = 0; c < 6; ++c)
            printf("%8.2f ", rate[r][c]);
        printf("\n");
    }

    printf("Sum -> ");
    scanf("%f", &value);

    printf("Term -> ");
    scanf("%i", &period);

    if (value <= 50000)
        r = 0;
    else
        if (value <= 250000)
            r = 1;
        else
            r = 2;

    switch (period) {
        case 3: c = 0; break;
        case 6: c = 1; break;
        case 12: c = 2; break;
        case 18: c = 3; break;
        case 24: c = 4; break;
        case 36: c = 5; break;
        default: period = 0;
    }

    if (period != 0) {
        printf("Interest rate: %5.2f\n", rate[r][c]);
        profit = value * rate[r][c]/100/12 * period;
        printf("Profit: %6.2f\n", profit);
    }
    else
        printf("No correct term\n");

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
180. Написать программу, которая обрабатывает результаты спортивных соревнований: выстраивает команды в соответствии с количеством набранных очков, вычисляемым по формуле К= 1Ng + 6NS+ 5NB, где Na, Ns и NB— количество золотых, серебряных и бронзовых медалей. Далее приведен рекомендуемый вид экрана программы (данные, введенные пользователем, выделены полужирным).
```
#include <stdio.h>
#include <string.h>

#define NC 5

int main()
{
    char *team[] = {"Hungary", "Germany", "Norway", "Russia", "Finland"};

    int result[NC+1][6];

    int i, j;
    int mx;

    for (i = 0; i < NC; ++i) {
        printf("%s -> ", team[i]);
        scanf("%i%i%i", &result[i][0],
                        &result[i][1],
                        &result[i][2]);
        result[i][5] = i;
    }

    for (i = 0; i < NC; ++i) {
        result[i][3] = result[i][0]+result[i][1]+result[i][2];
        result[i][4] = result[i][0]*7+result[i][1]*6+result[i][2]*5;
    }

    for (i = 0; i < NC+1; ++i) {
        mx = i;
        for (j = i+1; j < NC; ++j) {
            if (result[j][4] > result[mx][4])
                mx = j;
        }

        for (j = 0; j < 6; ++j)
            result[NC][j] = result[i][j];
        for (j = 0; j < 6; ++j)
            result[i][j] = result[mx][j];
        for (j = 0; j < 6; ++j)
            result[mx][j] = result[NC][j];
    }

    printf("%3s%12s%8s%8s%8s%8s%8s", " ", "Team", "Gold",
                                     "Silver", "Bronze",
                                     "Total", "Points");
    for (i = 0; i < NC; ++i) {
        printf("\n%12s", team[result[i][5]]);
        for (j = 0; j < 5; ++j)
            printf("%8i", result[i][j]);
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
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
```
#include <iostream>
#include <string>

using std::cin; using std::cout; using std::endl; using std::string;

int main()
{
    const string morse[] = {".-", "-...", "-.-.", "-..", ".", "..-.",
                            "--.", "....", "..", ".---", "-.-", ".-..",
                            "--", "-.", "---", ".--.", "--.-", ".-.",
                            "...", "-", "..-", "...-", ".--", "-..-",
                            "-.--", "--..", "-----", ".----", "..---", "...--",
                            "....-", ".....", "-....", "--...", "---..",
                            "----."};

    string user_input;
    cout << "-> ";
    getline(cin, user_input);
    cout << endl;

    for (decltype(user_input.size()) i = 0; i != user_input.size(); ++i) {
        if (user_input[i] >= 'A' && user_input[i] <= 'Z')
            cout << morse[user_input[i] - 65];
        else if (user_input[i] >= 'a' && user_input[i] <= 'z')
            cout << morse[user_input[i] - 97];
        else if (user_input[i] >= '0' && user_input[i] <= '9')
            cout << morse[user_input[i] - 22];
        else if (user_input[i] == ' ')
            cout << " ";
        else continue;
        cout << " ";
    }
    cout << endl;

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
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
221. Объявите структуру empl (от employee — сотрудник), состоящую из полей name и salary, предназначенную для хранения информации о зарплате сотрудников организации.
```
#include <stdio.h>

struct empl {
    char name[15];
    double salary;
};

int main()
{
    empl person1 = {"Eto", 1};

    printf("%s, %f\n", person1.name, person1.salary);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
222. Напишите программу, которая формирует массив staff, состоящий из структур empl (см. задачу 221).
```
#include <stdio.h>
#include <string.h>

struct empl {
    char name[15] = {};
    double salary = 0;
};

int main()
{
    empl staff[5];

    strcpy(staff[0].name, "Homer Simpson");
    staff[0].salary = 5000;

    strcpy(staff[1].name, "James Bond");
    staff[1].salary = 120000;

    for (int i = 0; i < 5; ++i) {
        if (strlen(staff[i].name) != 0)
            printf("%-15s %9.2f $\n", staff[i].name, staff[i].salary);
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
223. Объявите класс TPerson, позволяющий создавать объекты, содержащие информацию о людях (имя, фамилия). Класс должен содержать конструктор, деструктор, а также свойство FullName, значением которого является полное имя (имя и фамилия как одна строка).
```
#include <stdio.h>
#include <string.h>

class TPerson {
public:
    TPerson(char *FirstName, char *LastName);
    ~TPerson();
    char *FullName() {
        if (fullname != NULL) delete[] fullname;

        fullname = new char[strlen(fname)+strlen(lname)+2];
        sprintf(fullname, "%s %s", fname, lname);
        return fullname;
    }
private:
    char *fname;
    char *lname;
    char *fullname;
};

TPerson::TPerson(char *firstname, char *lastname) {
    fname = new char[strlen(firstname)];
    lname = new char[strlen(lastname)];

    strcpy(fname, firstname);
    strcpy(lname, lastname);

    fullname = NULL;
}

TPerson::~TPerson() {
    delete[] fname;
    delete[] lname;
    delete[] fullname;
}

int main()
{
    TPerson person("Eto", "Tenma");

    printf("%s\n", person.FullName());

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
224. Измените объявление класса TPerson (см. задачу 221) так, чтобы он помимо имени и фамилии содержал адрес e-Mail.
```
#include <stdio.h>
#include <string.h>

class TPerson {
public:
    TPerson(char *FirstName, char *LastName, char *EMail);

    ~TPerson();

    char *FullName() {
        if (fullname != NULL) delete[] fullname;

        fullname = new char[strlen(fname)+strlen(lname)+2];
        sprintf(fullname, "%s %s %s", fname, lname, email);
        return fullname;
    }
private:
    char *fname;
    char *lname;
    char *email;

    char *fullname;
};

TPerson::TPerson(char *firstname, char *lastname, char *mail) {
    fname = new char[strlen(firstname)];
    lname = new char[strlen(lastname)];
    email = new char[strlen(mail)];

    strcpy(fname, firstname);
    strcpy(lname, lastname);
    strcpy(email, mail);

    fullname = NULL;
}

TPerson::~TPerson() {
    delete[] fname;
    delete[] lname;
    delete[] email;
    delete[] fullname;
}

int main()
{
    TPerson person("Eto", "Tenma", "my.Mail");

    printf("%s\n", person.FullName());

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
225. Напишите программу, которая для хранения информации о человеке использует класс TPerson.
```
#include <stdio.h>
#include <string.h>

class TPerson {
public:
    TPerson(char *FirstName, char *LastName, char *EMail);

    ~TPerson();

    char *FullName() {
        if (fullname != NULL) delete[] fullname;

        fullname = new char[strlen(fname)+strlen(lname)+2];
        sprintf(fullname, "%s %s %s", fname, lname, email);
        return fullname;
    }
private:
    char *fname;
    char *lname;
    char *email;

    char *fullname;
};

TPerson::TPerson(char *firstname, char *lastname, char *mail) {
    fname = new char[strlen(firstname)];
    lname = new char[strlen(lastname)];
    email = new char[strlen(mail)];

    strcpy(fname, firstname);
    strcpy(lname, lastname);
    strcpy(email, mail);

    fullname = NULL;
}

TPerson::~TPerson() {
    delete[] fname;
    delete[] lname;
    delete[] email;
    delete[] fullname;
}

int main()
{
    TPerson *person;

    person = new TPerson("Bart", "Simpson", "Mail");

    printf("%s\n", person->FullName());

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
226. Напишите программу, которая для хранения информации о людях использует массив объектов класса TPerson. Имена людей должны вводиться с клавиатуры во время работы программы.
```
#include <stdio.h>
#include <string.h>

#define HB 3

class TPerson {
public:
    TPerson(char *FirstName, char *LastName, char *EMail);

    ~TPerson();

    char *FullName() {
        if (fullname != NULL) delete[] fullname;

        fullname = new char[strlen(fname)+strlen(lname)+2];
        sprintf(fullname, "%s %s %s", fname, lname, email);
        return fullname;
    }
private:
    char *fname;
    char *lname;
    char *email;

    char *fullname;
};

TPerson::TPerson(char *firstname, char *lastname, char *mail) {
    fname = new char[strlen(firstname)];
    lname = new char[strlen(lastname)];
    email = new char[strlen(mail)];

    strcpy(fname, firstname);
    strcpy(lname, lastname);
    strcpy(email, mail);

    fullname = NULL;
}

TPerson::~TPerson() {
    delete[] fname;
    delete[] lname;
    delete[] email;
    delete[] fullname;
}

int main()
{
    TPerson *persones[HB];

    char *fname = new char[20];
    char *lname = new char[20];
    char *email = new char[20];

    for (int i = 0; i < HB; ++i) {
        printf("fname -> ");
        scanf("%s", fname);

        printf("lname -> ");
        scanf("%s", lname);

        printf("ename -> ");
        scanf("%s", email);

        persones[i] = new TPerson(fname, lname, email);
    }

    for (int i = 0; i < HB; ++i) {
        printf("%s\n", persones[i]->FullName());
    }

    for (int i = 0; i < HB; ++i) {
        persones[i]->~TPerson();
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
227. Объявите класс TPerson и производные от него классы TStud и TProf. Класс TPerson должен содержать общую информацию о персоне. Классы TStud и TProf должны расширять информацию о персоне как о студенте и, соответственно, преподавателе.
```
#include <stdio.h>
#include <string.h>

class TPerson {
public:
    TPerson() {}

    TPerson(char *FirstName, char *LastName) {
        fname = new char[strlen(FirstName) + 1];
        strcpy(fname, FirstName);
        lname = new char[strlen(LastName) + 1];
        strcpy(lname, LastName);
    }

    ~TPerson() {
        delete[] fname;
        delete[] lname;
    }

    char *FullName() {
        char *fullname = new char[strlen(fname) + strlen(lname) + 2];
        sprintf(fullname, "%s %s", fname, lname);
        return fullname;
    }

    virtual void print() {}
private:
    char *fname;
    char *lname;
};

class TStud : public TPerson {
public:
    TStud() {}

    TStud(char *FirstName, char *LastName, int Group):
        TPerson(FirstName, LastName) { group = Group; }

    ~TStud() {}

    void print() {
        printf("%s, gr. %i\n", this->FullName(), group);
    }
private:
    int group;
};

class TProf : public TPerson {
public:
    TProf() {}

    TProf(char *FirstName, char *LastName, char *Kafedra):
        TPerson(FirstName, LastName) { kafedra = new char[strlen(Kafedra) + 1];
                                       strcpy(kafedra, Kafedra);}
    ~TProf() {
        delete[] kafedra;
    }

    void print() {
        printf("%s, dep. %s\n", this->FullName(), kafedra);
    }
private:
    char *kafedra;
};

int main()
{
    TPerson ordinaryPerson("Eto", "Tenma");
    TStud studentPerson("Shiraha", "Main", 2);
    TProf professorPerson("Kuanai", "Breadx333", "IT");

    printf("%s\n", ordinaryPerson.FullName());
    studentPerson.print();
    professorPerson.print();

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
228. Напишите программу, которая хранит в одном массиве информацию о студентах и преподавателях (см. задачу 227).
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

class TPerson {
public:
    TPerson() {}

    TPerson(char *FirstName, char *LastName) {
        fname = new char[strlen(FirstName) + 1];
        strcpy(fname, FirstName);
        lname = new char[strlen(LastName) + 1];
        strcpy(lname, LastName);
    }

    ~TPerson() {
        delete[] fname;
        delete[] lname;
    }

    char *FullName() {
        char *fullname = new char[strlen(fname) + strlen(lname) + 2];
        sprintf(fullname, "%s %s", fname, lname);
        return fullname;
    }

    virtual void print() {}
private:
    char *fname;
    char *lname;
};

class TStud : public TPerson {
public:
    TStud() {}

    TStud(char *FirstName, char *LastName, int Group):
        TPerson(FirstName, LastName) { group = Group; }

    ~TStud() {}

    void print() {
        printf("%s, gr. %i\n", this->FullName(), group);
    }
private:
    int group;
};

class TProf : public TPerson {
public:
    TProf() {}

    TProf(char *FirstName, char *LastName, char *Kafedra):
        TPerson(FirstName, LastName) { kafedra = new char[strlen(Kafedra) + 1];
                                       strcpy(kafedra, Kafedra);}
    ~TProf() {
        delete[] kafedra;
    }

    void print() {
        printf("%s, dep. %s\n", this->FullName(), kafedra);
    }
private:
    char *kafedra;
};

int main()
{
    TPerson *persones[10];

    int K = sizeof(persones)/sizeof(TPerson*);

    for (int i = 0; i < K; ++i)
        persones[i] = NULL;

    persones[0] = new TStud("Eto", "Tenma", 1358);
    persones[1] = new TStud("Shiraha", "Main", 1358);
    persones[2] = new TProf("Kuanai", "Breadx333", "IT");

    printf("All:\n");
    int i = 0;
    while (persones[i] != NULL) {
        persones[i]->print();
        ++i;
    }

    printf("\nStudents:\n");
    i = 0;
    while (persones[i] != NULL) {
        if (typeid(*persones[i]) == typeid(TStud)) {
            persones[i]->print();
        }
        ++i;
    }

    i = 0;
    while (persones[i] != NULL) {
        delete persones[i];
        ++i;
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
229. Объявите структуру book для программы работы с информацией о книгах, например, в книжном магазине.
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

struct Book {
    char *id;
    char *name;
    char *author;
    int year;
    float price;
};

int main()
{
    Book book = {"228", "Disorder", "Eto Tenma", 1337, 10};

    printf("ID: %s\n", book.id);
    printf("Name: %s\n", book.name);
    printf("Author: %s\n", book.author);
    printf("Year: %d\n", book.year);
    printf("Price: %.2f $\n", book.price);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
230. Напишите программу, формирующую массив структур book (см. задачу 229). Информация о книгах должна вводиться с клавиатуры во время работы программы.
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

#define CNT 2

struct Book {
    Book() {}
    Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE) {
        id = new char[strlen(ID)];
        name = new char[strlen(NAME)];
        author = new char[strlen(AUTHOR)];

        strcpy(id, ID);
        strcpy(name, NAME);
        strcpy(author, AUTHOR);
        year = YEAR;
        price = PRICE;
    }
    char *id;
    char *name;
    char *author;
    int year;
    float price;
};

int main()
{
    Book *book[CNT];

    char *id = new char[20];
    char *name = new char[20];
    char *author = new char[20];
    int year;
    float price;

    for (int i = 0; i < CNT; ++i) {
        printf("Book id -> ");
        scanf("%s", id);
        printf("Book name -> ");
        scanf("%s", name);
        printf("Book author -> ");
        scanf("%s", author);
        printf("Book year -> ");
        scanf("%i", &year);
        printf("Book price -> ");
        scanf("%f", &price);

        book[i] = new Book(id, name, author, year, price);
    }

    for (int i = 0; i < CNT; ++i) {
        printf("ID: %s\n", book[i]->id);
        printf("Name: %s\n", book[i]->name);
        printf("Author: %s\n", book[i]->author);
        printf("Year: %d\n", book[i]->year);
        printf("Price: %.2f $\n", book[i]->price);
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
231. Объявите класс твоок для программы работы с информацией о книгах, например, в книжном магазине.
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

#define CNT 2

class Book {
public:
    Book() {}
    Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE);
    ~Book();
    print() {
        printf("ID: %s\n", id);
        printf("Name: %s\n", name);
        printf("Author: %s\n", author);
        printf("Year: %d\n", year);
        printf("Price: %.2f $\n", price);
    }
private:
    char *id;
    char *name;
    char *author;
    int year;
    float price;
};

Book::Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE){
    id = new char[strlen(ID)];
    name = new char[strlen(NAME)];
    author = new char[strlen(AUTHOR)];

    strcpy(id, ID);
    strcpy(name, NAME);
    strcpy(author, AUTHOR);
    year = YEAR;
    price = PRICE;
}

Book::~Book() {
    delete[] id;
    delete[] name;
    delete[] author;
}

int main()
{
    Book book("228", "Disorder", "EtoTenma", 1337, 10);

    book.print();

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
232. Напишите программу, формирующую массив объектов твоок (см. задачу 229). Информация о книгах должна вводиться с клавиатуры во время работы программы
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

#define CNT 2

class Book {
public:
    Book() {}
    Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE);
    ~Book();
    print() {
        printf("ID: %s\n", id);
        printf("Name: %s\n", name);
        printf("Author: %s\n", author);
        printf("Year: %d\n", year);
        printf("Price: %.2f $\n", price);
    }
private:
    char *id;
    char *name;
    char *author;
    int year;
    float price;
};

Book::Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE){
    id = new char[strlen(ID)];
    name = new char[strlen(NAME)];
    author = new char[strlen(AUTHOR)];

    strcpy(id, ID);
    strcpy(name, NAME);
    strcpy(author, AUTHOR);
    year = YEAR;
    price = PRICE;
}

Book::~Book() {
    delete[] id;
    delete[] name;
    delete[] author;
}

int main()
{
    Book *book[CNT];

    char *id = new char[20];
    char *name = new char[20];
    char *author = new char[20];
    int year;
    float price;

    for (int i = 0; i < CNT; ++i) {
        printf("Book id -> ");
        scanf("%s", id);
        printf("Book name -> ");
        scanf("%s", name);
        printf("Book author -> ");
        scanf("%s", author);
        printf("Book year -> ");
        scanf("%i", &year);
        printf("Book price -> ");
        scanf("%f", &price);

        book[i] = new Book(id, name, author, year, price);
    }

    for (int i = 0; i < CNT; ++i) {
        book[i]->print();
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
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
