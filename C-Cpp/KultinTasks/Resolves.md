
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
