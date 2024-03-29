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
4
```
#include <iostream>
#include <string>

using std::cin; using std::cout; using std::endl; using std::string;

typedef char *arrayString;

int length(arrayString s) {
    int cnt = 0;
    while (s[cnt] != 0) ++cnt;
    return cnt;
}

void concatenate(arrayString &s1, arrayString &s2) {
    int s1_OldLength = length(s1);
    int s2_Length = length(s2);
    int s1_NewLength = s1_OldLength + s2_Length;
    arrayString newS = new char[s1_NewLength + 1];
    for (int i = 0; i < s1_OldLength; ++i) newS[i] = s1[i];
    for (int i = 0; i < s2_Length; ++i) newS[s1_OldLength + i] = s2[i];
    newS[s1_NewLength] = 0;
    delete[] s1;
    s1 = newS;
}

void append(arrayString &s, char c) {
    int oldLength = length(s);
    arrayString newS = new char[oldLength + 2];
    for (int i = 0; i < oldLength; ++i) newS[i] = s[i];
    newS[oldLength] = c;
    newS[oldLength + 1] = 0;
    delete[] s;
    s = newS;
}

void appendTester() {
    arrayString a = new char[5];
    a[0] = 't'; a[1] = 'e'; a[2] = 's'; a[3] = 't'; a[4] = 0;
    append(a, '!');
    cout << a << "\n";
}

void concatenateTester() {
    arrayString a = new char[5];
    a[0] = 't'; a[1] = 'e'; a[2] = 's'; a[3] = 't'; a[4] = 0;
    arrayString b = new char[1];
    b[0] = 0;
    concatenate(b, a);
    cout << a << ' ' << b << endl;
    cout << (void *)a << ' ' << (void *)b << endl;
}

char characterAt(arrayString s, int postintion) {
    return s[postintion];
}

int main()
{
    appendTester();
    concatenateTester();
    return 0;
}
```
4.2
```
#include <iostream>
#include <string>

using std::cin; using std::cout; using std::endl; using std::string;

struct listNode {
    int studentNum;
    int grade;
    listNode *next;
};

typedef listNode * studentCollection;

void addRecord(studentCollection &sc, int stuNum, int gr) {
    listNode *newNode = new listNode;
    newNode->studentNum = stuNum;
    newNode->grade = gr;
    newNode->next = sc;
    sc = newNode;
}

double averageRecord(studentCollection sc) {
    if (sc == NULL) return 0;
    int cnt = 0;
    double sum = 0;
    listNode *loopPtr = sc;
    while (loopPtr != NULL) {
        sum += loopPtr->grade;
        ++cnt;
        loopPtr = loopPtr->next;
    }
    double avg = sum / cnt;
    return avg;
}

int main()
{
    studentCollection sc;

    listNode *node1 = new listNode;
    node1->studentNum = 1001; node1->grade = 78;

    listNode *node2 = new listNode;
    node2->studentNum = 1012; node2->grade = 93;

    listNode *node3 = new listNode;
    node3->studentNum = 1076; node3->grade = 85;

    sc = node1;

    node1->next = node2;
    node2->next = node3;
    node3->next = NULL;

    node1 = node2 = node3 = NULL;

    addRecord(sc, 1274, 91);

    listNode *ptr = sc;

    while (ptr != NULL) {
        cout << ptr->studentNum << ' ' << ptr->grade << endl;
        ptr = ptr->next;
    }

    cout << averageRecord(sc) << endl;

	return 0;
}
```
5.1
```
#include <iostream>
#include <string>

using std::cin; using std::cout; using std::endl; using std::string;

class studentRecord {
public:
    studentRecord() {
        setGrade(0);
        setStudentID(-1);
        setName("");
    }
    studentRecord(int newGrade, int newID, string newName) {
        setGrade(newGrade);
        setStudentID(newID);
        setName(newName);
    }

    int getGrade();
    void setGrade(int newGrade);
    int getStudentID();
    void setStudentID(int newID);
    string getName();
    void setName(string newName);
    string letterGrade();
private:
    bool isValidGrade(int grade);
    int _grade;
    int _studentID;
    string _name;
};

bool studentRecord::isValidGrade(int grade) {
    if ((grade >= 0) && (grade <= 100))
        return true;
    else
        return false;
}

int studentRecord::getGrade() {
    return _grade;
}

void studentRecord::setGrade(int newGrade) {
    if (isValidGrade(newGrade))
        _grade = newGrade;
}

int studentRecord::getStudentID() {
    return _studentID;
}

void studentRecord::setStudentID(int newID) {
    _studentID = newID;
}

string studentRecord::getName() {
    return _name;
}

void studentRecord::setName(string newName) {
    _name = newName;
}

string studentRecord::letterGrade() {
    if (!isValidGrade(_grade)) return "Error\n";
    const int NUMBER_CATEGORIES = 11;
    const string GRADE_LETTER[] = {"F", "D", "D+", "C-", "C", "C+", "B-", "B", "B+", "A-", "A"};
    const int LOWEST_GRADE_SCORE[] = {0, 66, 67, 70, 73, 77, 80, 83, 87, 90, 93};
    int category = 0;
    while (category < NUMBER_CATEGORIES && LOWEST_GRADE_SCORE[category] <= _grade)
        ++category;
    return GRADE_LETTER[category-1];
}

int main()
{
    studentRecord test;

    cout << test.getGrade() << ' ' << test.getStudentID() << ' ' << test.getName() << endl;

	return 0;
}
```
5.2
```
#include <iostream>
#include <string>

using std::cin; using std::cout; using std::endl; using std::string;

class studentRecord {
public:
    studentRecord() {
        setGrade(0);
        setStudentID(-1);
        setName("");
    }
    studentRecord(int newGrade, int newID, string newName) {
        setGrade(newGrade);
        setStudentID(newID);
        setName(newName);
    }

    int getGrade();
    void setGrade(int newGrade);
    int getStudentID();
    void setStudentID(int newID);
    string getName();
    void setName(string newName);
    string letterGrade();
private:
    bool isValidGrade(int grade);
    int _grade;
    int _studentID;
    string _name;
};

bool studentRecord::isValidGrade(int grade) {
    if ((grade >= 0) && (grade <= 100))
        return true;
    else
        return false;
}

int studentRecord::getGrade() {
    return _grade;
}

void studentRecord::setGrade(int newGrade) {
    if (isValidGrade(newGrade))
        _grade = newGrade;
}

int studentRecord::getStudentID() {
    return _studentID;
}

void studentRecord::setStudentID(int newID) {
    _studentID = newID;
}

string studentRecord::getName() {
    return _name;
}

void studentRecord::setName(string newName) {
    _name = newName;
}

string studentRecord::letterGrade() {
    if (!isValidGrade(_grade)) return "Error\n";
    const int NUMBER_CATEGORIES = 11;
    const string GRADE_LETTER[] = {"F", "D", "D+", "C-", "C", "C+", "B-", "B", "B+", "A-", "A"};
    const int LOWEST_GRADE_SCORE[] = {0, 66, 67, 70, 73, 77, 80, 83, 87, 90, 93};
    int category = 0;
    while (category < NUMBER_CATEGORIES && LOWEST_GRADE_SCORE[category] <= _grade)
        ++category;
    return GRADE_LETTER[category-1];
}

class studentCollection {
private:
    struct studentNode {
        studentRecord studentData;
        studentNode *next;
    };
public:
    studentCollection() {
        _listHead = NULL;
    }
    studentCollection(const studentCollection &original);
    studentCollection& operator=(const studentCollection &rhs);
    void addRecord(studentRecord newStudent);
    studentRecord recordWithNumber(int idNum);
    void removeRecord(int idNum);
    ~studentCollection() {
        delete(_listHead);
    }
private:
    typedef studentNode * studentList;
    studentList _listHead;
    void deleteList(studentList &listPtr);
    studentList copiedList(const studentList original);
};

void studentCollection::addRecord(studentRecord newStudent) {
    studentNode *newNode = new studentNode;
    newNode->studentData = newStudent;
    newNode->next = _listHead;
    _listHead = newNode;
}
studentRecord studentCollection::recordWithNumber(int idNum) {
    studentNode *loopPtr = _listHead;
    while (loopPtr->studentData.getStudentID() != idNum)
        loopPtr = loopPtr->next;
    if (loopPtr == NULL) {
        studentRecord dummyRecord(-1, -1, "");
        return dummyRecord;
    }
    else
        return loopPtr->studentData;
}

void studentCollection::removeRecord(int idNum) {
    studentNode *loopPtr = _listHead;
    studentNode *trailing = NULL;
    while (loopPtr != NULL && loopPtr->studentData.getStudentID() != idNum) {
        trailing = loopPtr;
        loopPtr = loopPtr->next;
    }
    if (loopPtr == NULL) return;
    if (trailing == NULL)
        _listHead = _listHead->next;
    else
        trailing->next = loopPtr->next;
    delete loopPtr;
}

void studentCollection::deleteList(studentList &listPtr) {
    while (listPtr != NULL) {
        studentNode *temp = listPtr;
        listPtr = listPtr->next;
        delete temp;
    }
}

studentCollection& studentCollection::operator=(const studentCollection &rhs) {
    if (this != &rhs) {
        delete(_listHead);
        _listHead = copiedList(rhs._listHead);
    }
    return *this;
}

studentCollection::studentList studentCollection::copiedList(const studentList original) {
    if (original == NULL) {
        return NULL;
    }
    studentList newList = new studentNode;
    newList->studentData = original->studentData;
    studentNode *oldLoopPtr = original->next;
    studentNode *newLoopPtr = newList;
    while (oldLoopPtr != NULL) {
        newLoopPtr->next = new studentNode;
        newLoopPtr = newLoopPtr->next;
        newLoopPtr->studentData = oldLoopPtr->studentData;
        oldLoopPtr = oldLoopPtr->next;
    }
    newLoopPtr->next = NULL;
    return newList;
}

studentCollection::studentCollection(const studentCollection &original) {
    _listHead = copiedList(original._listHead);
}

int main()
{
    studentCollection s;
    studentRecord stu3(84, 1152, "Sue");
    studentRecord stu2(75, 4875, "Edd");
    studentRecord stu1(98, 2938, "Todd");
    s.addRecord(stu3);
    s.addRecord(stu2);
    s.addRecord(stu1);
    studentCollection s1(s);
    cout << s1.recordWithNumber(4875).getGrade() << endl;

	return 0;
}
```
