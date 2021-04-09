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
