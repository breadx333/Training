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
