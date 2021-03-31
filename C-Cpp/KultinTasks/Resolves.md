
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
