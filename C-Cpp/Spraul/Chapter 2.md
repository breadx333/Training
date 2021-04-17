2.1
```
#include <iostream>

#define N 128

using std::cin; using std::cout; using std::endl;

int main() {
    for (int i = 0; i < N; ++i) {
        for (int sp = 0; sp < i; ++sp)
            cout << ' ';
        for (int j = 0; j < N*2 - i*2; ++j)
            cout << '#';
        cout << endl;
    }
}
```
```
#include <iostream>

#define N 8

using std::cin; using std::cout; using std::endl;

int main() {
    for (int i = 1; i <= N; ++i) {
        for (int j = 1; j <= N*2; ++j)
            if (i > j || j >= N*2 - i) cout << ' ';
            else cout << '#';
        cout << endl;
    }
}
```
2.2
```
#include <iostream>

#define N 8

using std::cin; using std::cout; using std::endl;

int main() {
    for (int i = 1; i <= N; ++i) {
        for (int j = 1; j <= N; ++j)
            if (i <= N/2)
                if (j <= N/2 - i || j > N/2 + i) cout << ' ';
                else cout << '#';
            else
                if (j < i - N/2 || j > N - (i - N/2) + 1) cout << ' ';
                else cout << '#';
        cout << endl;
    }
}
```
2.3
```
#include <iostream>

#define N 8

using std::cin; using std::cout; using std::endl;

void f(int i) {
    int j, k;
    for (j = 0; j < i-1; ++j)
        cout << ' ';
    for (k = 0; k < i; ++k)
        cout << '#';
    for (int l = 0; l < ((N-1)*2 - 2*j - 2*k); ++l)
        cout << ' ';
    for (int m = 0; m < i; ++m)
        cout << '#';
    cout << endl;
}

int main() {
    for (int i = 1; i <= N/2; ++i)
        f(i);
    for (int i = N/2; i > 0; --i)
        f(i);
    cout << endl;
}
```
2.4
```
#include <iostream>

#define N 10

using std::cin; using std::cout; using std::endl;

int main() {
    for (int i = 1; i <= N; ++i) {
        for (int j = 1; j <= N*2; ++j)
            if (j == N) cout << ' ';
            else if (i == N/2) cout << ' ';
            else if (j < N - abs(N - i) || j > N + i) cout << ' ';
            else cout << '#';
        cout << endl;
    }
}
```
2.5
