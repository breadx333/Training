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
