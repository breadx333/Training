
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
