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
