Begin1°. Дана сторона квадрата a. Найти его периметр P = 4·a. 
```
#include <stdio.h>

int main()
{
    int P, a;

    printf("Enter <a>: ");
    scanf("%d", &a);

    P = 4 * a;

    printf("Perimeter = %d\n", P);

    return 0;
}
```

Begin2°. Дана сторона квадрата a. Найти его площадь S = a2. 
```
#include <stdio.h>

int main()
{
    int S, a;

    printf("Enter <a>: ");
    scanf("%d", &a);

    S = a * a;

    printf("Square = %d\n", S);

    return 0;
}
```

Begin3°. Даны стороны прямоугольника a и b. Найти его площадь S = a·b и периметр P = 2·(a + b). 
```
#include <stdio.h>

int main()
{
    int P, S, a, b;

    printf("Enter <a and b>: ");
    scanf("%d:%d", &a, &b);

    S = a * b;
    P = 2 * (a + b);

    printf("Perimeter = %d\n", P);
    printf("Square = %d\n", S);

    return 0;
}
```

Begin4°. Дан диаметр окружности d. Найти ее длину L = π·d. В качестве значения π использовать 3.14.
```
#include <stdio.h>

int main()
{
    float L, d;

    const float PI = 3.14;

    printf("Enter <d>: ");
    scanf("%f", &d);

    L = PI * d;

    printf("perimeter circumference = %f\n", L);

    return 0;
}
```

Begin5°. Дана длина ребра куба a. Найти объем куба V = a^3 и площадь его поверхности S = 6·a^2. 
```
#include <stdio.h>
#include <math.h>

int main()
{
    float V, S, a;

    printf("Enter <a>: ");
    scanf("%f", &a);

    V = pow(a, 3);
    S = 6 * pow(a, 2);

    printf("Cube Volume = %f\n", V);
    printf("Cube Square = %f\n", S);

    return 0;
}
```

Begin6°. Даны длины ребер a, b, c прямоугольного параллелепипеда. Найти его объем V = a·b·c и площадь поверхности S = 2·(a·b + b·c + a·c). 
```
#include <stdio.h>
#include <math.h>

int main()
{
    float V, S, a, b, c;

    printf("Enter <a b c>: ");
    scanf("%f:%f:%f", &a, &b, &c);

    V = a * b * c;
    S = 2 * (a*b + b*c + a*c);

    printf("Cube Volume = %f\n", V);
    printf("Cube Square = %f\n", S);

    return 0;
}
```

Begin7°. Найти длину окружности L и площадь круга S заданного радиуса R: L = 2·π·R, S = π·R2. В качестве значения π использовать 3.14. 
```
#include <stdio.h>
#include <math.h>

int main()
{
    const float PI = 3.14;
    float L, S, R;

    printf("Enter <R>: ");
    scanf("%f", &R);

    L = 2 * PI * R;
    S = PI * pow(R, 2);

    printf("Lenght = %f\n", L);
    printf("Square = %f\n", S);

    return 0;
}
```

Begin8°. Даны два числа a и b. Найти их среднее арифметическое: (a + b)/2. 
```
#include <stdio.h>
#include <math.h>

int main()
{
    double Medium, a, b;

    printf("Enter <a:b>: ");
    scanf("%d:%d", &a, &b);

    Medium = (a + b) / 2;

    printf("Medium = %d\n", Medium);

    return 0;
}
```
Begin9°. Даны два неотрицательных числа a и b. Найти их среднее геометрическое, т. е. квадратный корень из их произведения: (a·b)^1/2.
```
#include <iostream>
#include <math.h>

using namespace std;

void geometry_medium(double a, double b)
{
    cout << "Result: " << sqrt(a * b) << "\n";
}

int main()
{
    int a, b;

    cout << "Add a: ";
    cin >> a;
    cout << "Add b: ";
    cin >> b;

    geometry_medium(a, b);
}
```
Begin10°. Даны два ненулевых числа. Найти сумму, разность, произведение и частное их квадратов. 
```
#include <iostream>

#include <math.h>

using namespace std;

double summary(double a, double b)
{
    return a + b;
}

double difference(double a, double b)
{
    return abs(a - b);
}

double composting(double a, double b)
{
    return a * b;
}

double private_square(double a, double b)
{
    return (a * a)/(b * b);
}

void goto_list(double a, double b)
{
    cout << "Summary: " << summary(a, b) << "\n";
    cout << "Difference: " << difference(a, b) << "\n";
    cout << "Composting: " << composting(a, b) << "\n";
    cout << "Private Square: " << private_square(a, b) << "\n\n";
}

int main()
{
    bool Check = true;

    while(Check)
    {
        double a, b;

        cout << "Add a: ";
        cin >> a;
        cout << "Add b: ";
        cin >> b;

        if (a == 0 || b == 0)
        {
            cout << "Note: Add non zero number.\n\n";
        }
        else
        {
            goto_list(a, b);
        }
    }
}

```
Begin11°. Даны два ненулевых числа. Найти сумму, разность, произведение и частное их модулей. 
```
#include <iostream>
#include <math.h>

using namespace std;

double summary(double a, double b)
{
    return a + b;
}

double difference(double a, double b)
{
    return abs(a - b);
}

double composting(double a, double b)
{
    return a * b;
}

double private_modules(double a, double b)
{
    return abs(a)/abs(b);
}

void goto_list(double a, double b)
{
    cout << "Summary: " << summary(a, b) << "\n";
    cout << "Difference: " << difference(a, b) << "\n";
    cout << "Composting: " << composting(a, b) << "\n";
    cout << "Private Modules: " << private_modules(a, b) << "\n\n";
}

int main()
{
    bool Check = true;

    while(Check)
    {
        double a, b;

        cout << "Add a: ";
        cin >> a;
        cout << "Add b: ";
        cin >> b;

        if (a == 0 || b == 0)
        {
            cout << "Note: Add non zero number.\n\n";
        }
        else
        {
            goto_list(a, b);
        }
    }
}

```
