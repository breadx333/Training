2.2
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

    if ((position - 1) % 2 == 0) checkSum = evenLengthCheckSum;
    else checkSum = oddLengthCheckSum;

    cout << "CheckSum is " << checkSum << ". \n";
    if (checkSum % 10 == 0) {
        cout << "CheckSum is divisible by 10. Valid. \n";
    }
    else {
        cout << "CheckSum is not divisible by 10. Invalid. \n";
    }
}
```
2.3
```
#include <iostream>

using std::cin; using std::cout; using std::endl;

int main() {
    char outputCharacter;
    enum modeType {UPPERCASE, LOWERCASE, PUNCTUATION};
    modeType mode = UPPERCASE;
    cout << "Enter a three-digit or four-digit number: ";
    char digitChar;
    do {
        digitChar = cin.get();
        int number = (digitChar - '0');
        digitChar = cin.get();
        while ((digitChar != 10) && (digitChar != ',')) {
            number = number * 10 + (digitChar - '0');
            digitChar = cin.get();
        }
        switch (mode) {
            case UPPERCASE:
                number = number % 27;
                outputCharacter = number + 'A' - 1;
                if (number == 0) {
                    mode = LOWERCASE;
                    continue;
                }
                break;
            case LOWERCASE:
                number = number % 27;
                outputCharacter = number + 'a' - 1;
                if (number == 0) {
                    mode = PUNCTUATION;
                    continue;
                }
                break;
            case PUNCTUATION:
                number = number % 9;
                switch (number) {
                    case 1: outputCharacter = '!'; break;
                    case 2: outputCharacter = '?'; break;
                    case 3: outputCharacter = ','; break;
                    case 4: outputCharacter = '.'; break;
                    case 5: outputCharacter = ' '; break;
                    case 6: outputCharacter = ';'; break;
                    case 7: outputCharacter = '"'; break;
                    case 8: outputCharacter = '\\'; break;
                }
                if (number == 0) {
                    mode = UPPERCASE;
                    continue;
                }
                break;
        }
        cout << outputCharacter;
    } while (digitChar != 10);
    cout << "\n";
}
```
```
int main() {
    char digitChar = cin.get();
    int overallNumber = 0;
    char decoder = 'U';

    while (digitChar != 10) {
        if (digitChar == ',' && (digitChar = cin.get()) == ' ') {
                switch (decoder) {
                case 'U':
                    overallNumber = overallNumber % 27;
                    if (overallNumber == 0) decoder = 'L';
                    else cout << char(overallNumber + 'A' - 1) << ' ';
                    break;
                case 'L':
                    overallNumber = overallNumber % 27;
                    if (overallNumber == 0) decoder = 'P';
                    else cout << char(overallNumber + 'a' - 1) << ' ';
                    break;
                case 'P':
                    overallNumber = overallNumber % 9;
                    if (overallNumber == 0) decoder = 'L';
                    else {
                        switch (overallNumber) {
                            case 1: cout << '!'; break;
                            case 2: cout << '?'; break;
                            case 3: cout << ','; break;
                            case 4: cout << '.'; break;
                            case 5: cout << ' '; break;
                            case 6: cout << ';'; break;
                            case 7: cout << '"'; break;
                            case 8: cout << '\\'; break;
                        }
                    break;
                }
            }
            overallNumber = 0;
        }
        else {
            overallNumber = overallNumber * 10 + (digitChar - '0');
        }
        digitChar = cin.get();
    }
    cout << overallNumber << endl;
}
```
3
```
#include <iostream>

using std::cin; using std::cout; using std::endl;

int compareFunc(const void *voidA, const void *voidB) {
    int *intA = (int *)(voidA);
    int *intB = (int *)(voidB);
    return *intA - *intB;
}

int main()
{
    const int ARRAY_SIZE = 10;
    int intArray[ARRAY_SIZE] = {};
    int sortedArray[ARRAY_SIZE] = {};

    for (int i = 0; i < ARRAY_SIZE; ++i) {
        int val = 0;
        do {
            cout << "Enter " << i+1 << ": ";
            cin >> val;
        } while (val <= 0 || val > 10);
        intArray[i] = val;
        sortedArray[i] = val;
    }

    //qsort(sortedArray, ARRAY_SIZE, sizeof(int), compareFunc);

    int most;
    int mostcnt = 0;
    int cnt = 0;

    for (int i = 0; i < ARRAY_SIZE; ++i) {
        cnt++;
        if (i == ARRAY_SIZE-1 || sortedArray[i] != sortedArray[i+1]) {
            if (cnt > mostcnt) {
                most = sortedArray[i];
                mostcnt = cnt;
            }
            cnt = 0;
        }
    }

    cout << most << endl;
    cout << mostcnt << endl;

    for (const auto &e : sortedArray)
        cout << e << ' ';
    cout << endl;

    const int MAX_RESPONSE = 10;
    int histogram[MAX_RESPONSE];
    for (int i = 0; i < MAX_RESPONSE; ++i)
        histogram[i] = 0;
    for (int i = 0; i < ARRAY_SIZE; ++i)
        histogram[sortedArray[i] - 1]++;

    for (const auto &e : histogram)
        cout << e << ' ';
    cout << endl;

    int mostF = 0;
    for (int i = 1; i < MAX_RESPONSE; ++i)
        if (histogram[i] > histogram[mostF]) mostF = i;
    ++mostF;

    cout << mostF << " " << histogram[mostF-1] << endl;

	return 0;
}
```
