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
```
#include <iostream>

using std::cin; using std::cout; using std::endl;

int doubleDigitalValue(int digit) {
    int doubleDigit = digit * 2;
    int sum;
    if (doubleDigit >= 10) sum = 1 + doubleDigit % 10;
    else sum = doubleDigit;
    return sum;
}

int main() {
    char digit;
    int oddLengthCheckSum = 0;
    int evenLengthCheckSum = 0;
    int position = 1;

    cout << "Enter a number with an even number of digits: ";
    digit = cin.get();

    while (digit != 10) {
        if (position % 2 == 0) {
            oddLengthCheckSum += doubleDigitalValue(digit - '0');
            evenLengthCheckSum += digit - '0';
        }
        else {
            oddLengthCheckSum += digit - '0';
            evenLengthCheckSum += doubleDigitalValue(digit - '0');
        }
        digit = cin.get();
        ++position;
    }

    int checkSum;
    int checkNum;

    if ((position - 1) % 2 == 0) checkSum = evenLengthCheckSum;
    else checkSum = oddLengthCheckSum;

    checkNum = (10 - checkSum % 10);

    cout << "CheckSum is " << checkSum << ". \n";
    if (checkSum % 10 == 0) {
        cout << "CheckSum is divisible by 10. Valid. \n";
    }
    else if ((checkSum + checkNum) % 10 == 0) {
        cout << "CheckSum is divisible by 10. Valid. \n";
        cout << "CheckNum Generated: " << checkNum << endl;
    }
    else {
        cout << "CheckSum is not divisible by 10. Invalid. \n";
    }
}
```
2.6
```
