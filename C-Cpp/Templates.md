Check compiler version:
```
#include <iostream>

int main(){
    std::cout << __cplusplus;
}
```
RU Function
```
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
```
Interest Code
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

#define L 10
#define N 3

int main()
{
    int number;
    int sum;
    float avg;

    printf("Random numbers\n");

    srand((unsigned) time(NULL));

    for (int i = 0; i < N; ++i) {
        sum = 0;
        for (int j = 0; i < L; ++j) {
            number = rand() % 99 + 1;
            printf("%2i ");
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
