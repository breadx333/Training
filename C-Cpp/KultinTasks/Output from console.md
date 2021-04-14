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
