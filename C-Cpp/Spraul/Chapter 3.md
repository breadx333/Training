3.1
```
#include <iostream>
#include <string>

using std::cin; using std::cout; using std::endl; using std::string;

struct student {
    int grade;
    int studentID;
    string name;
};

int compareFunc(const void *voidA, const void *voidB) {
    int *intA = (int *)(voidA);
    int *intB = (int *)(voidB);
    return *intA - *intB;
}

int sortByGrade(const void *voidA, const void *voidB) {
    student *studentA = (student *)(voidA);
    student *studentB = (student *)(voidB);
    return studentB->grade - studentA->grade;
}

int sortByID(const void *voidA, const void *voidB) {
    student *studentA = (student *)(voidA);
    student *studentB = (student *)(voidB);
    return studentB->studentID - studentA->studentID;
}

int main()
{
    const int ARRAY_SIZE = 10;
    student studentArray[ARRAY_SIZE] = {{87, 10001, "Fred"},
                                        {28, 10002, "Tom"},
                                        {100, 10003, "Alistair"},
                                        {78, 10004, "Sasha"},
                                        {84, 10005, "Erin"},
                                        {98, 10006, "Belinda"},
                                        {75, 10007, "Leslie"},
                                        {70, 10008, "Candy"},
                                        {81, 10009, "Aretha"},
                                        {68, 10010, "Veronica"}};

    qsort(studentArray, ARRAY_SIZE, sizeof(student), sortByID);

    for (const auto e : studentArray) {
        cout << e.grade << ' ' << e.studentID << ' ' << e.name << endl;
    }

	return 0;
}
```
3.2
```
