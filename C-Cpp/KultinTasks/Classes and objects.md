221. Объявите структуру empl (от employee — сотрудник), состоящую из полей name и salary, предназначенную для хранения информации о зарплате сотрудников организации.
```
#include <stdio.h>

struct empl {
    char name[15];
    double salary;
};

int main()
{
    empl person1 = {"Eto", 1};

    printf("%s, %f\n", person1.name, person1.salary);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
222. Напишите программу, которая формирует массив staff, состоящий из структур empl (см. задачу 221).
```
#include <stdio.h>
#include <string.h>

struct empl {
    char name[15] = {};
    double salary = 0;
};

int main()
{
    empl staff[5];

    strcpy(staff[0].name, "Homer Simpson");
    staff[0].salary = 5000;

    strcpy(staff[1].name, "James Bond");
    staff[1].salary = 120000;

    for (int i = 0; i < 5; ++i) {
        if (strlen(staff[i].name) != 0)
            printf("%-15s %9.2f $\n", staff[i].name, staff[i].salary);
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
223. Объявите класс TPerson, позволяющий создавать объекты, содержащие информацию о людях (имя, фамилия). Класс должен содержать конструктор, деструктор, а также свойство FullName, значением которого является полное имя (имя и фамилия как одна строка).
```
#include <stdio.h>
#include <string.h>

class TPerson {
public:
    TPerson(char *FirstName, char *LastName);
    ~TPerson();
    char *FullName() {
        if (fullname != NULL) delete[] fullname;

        fullname = new char[strlen(fname)+strlen(lname)+2];
        sprintf(fullname, "%s %s", fname, lname);
        return fullname;
    }
private:
    char *fname;
    char *lname;
    char *fullname;
};

TPerson::TPerson(char *firstname, char *lastname) {
    fname = new char[strlen(firstname)];
    lname = new char[strlen(lastname)];

    strcpy(fname, firstname);
    strcpy(lname, lastname);

    fullname = NULL;
}

TPerson::~TPerson() {
    delete[] fname;
    delete[] lname;
    delete[] fullname;
}

int main()
{
    TPerson person("Eto", "Tenma");

    printf("%s\n", person.FullName());

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
224. Измените объявление класса TPerson (см. задачу 221) так, чтобы он помимо имени и фамилии содержал адрес e-Mail.
```
#include <stdio.h>
#include <string.h>

class TPerson {
public:
    TPerson(char *FirstName, char *LastName, char *EMail);

    ~TPerson();

    char *FullName() {
        if (fullname != NULL) delete[] fullname;

        fullname = new char[strlen(fname)+strlen(lname)+2];
        sprintf(fullname, "%s %s %s", fname, lname, email);
        return fullname;
    }
private:
    char *fname;
    char *lname;
    char *email;

    char *fullname;
};

TPerson::TPerson(char *firstname, char *lastname, char *mail) {
    fname = new char[strlen(firstname)];
    lname = new char[strlen(lastname)];
    email = new char[strlen(mail)];

    strcpy(fname, firstname);
    strcpy(lname, lastname);
    strcpy(email, mail);

    fullname = NULL;
}

TPerson::~TPerson() {
    delete[] fname;
    delete[] lname;
    delete[] email;
    delete[] fullname;
}

int main()
{
    TPerson person("Eto", "Tenma", "my.Mail");

    printf("%s\n", person.FullName());

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
225. Напишите программу, которая для хранения информации о человеке использует класс TPerson.
```
#include <stdio.h>
#include <string.h>

class TPerson {
public:
    TPerson(char *FirstName, char *LastName, char *EMail);

    ~TPerson();

    char *FullName() {
        if (fullname != NULL) delete[] fullname;

        fullname = new char[strlen(fname)+strlen(lname)+2];
        sprintf(fullname, "%s %s %s", fname, lname, email);
        return fullname;
    }
private:
    char *fname;
    char *lname;
    char *email;

    char *fullname;
};

TPerson::TPerson(char *firstname, char *lastname, char *mail) {
    fname = new char[strlen(firstname)];
    lname = new char[strlen(lastname)];
    email = new char[strlen(mail)];

    strcpy(fname, firstname);
    strcpy(lname, lastname);
    strcpy(email, mail);

    fullname = NULL;
}

TPerson::~TPerson() {
    delete[] fname;
    delete[] lname;
    delete[] email;
    delete[] fullname;
}

int main()
{
    TPerson *person;

    person = new TPerson("Bart", "Simpson", "Mail");

    printf("%s\n", person->FullName());

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
226. Напишите программу, которая для хранения информации о людях использует массив объектов класса TPerson. Имена людей должны вводиться с клавиатуры во время работы программы.
```
#include <stdio.h>
#include <string.h>

#define HB 3

class TPerson {
public:
    TPerson(char *FirstName, char *LastName, char *EMail);

    ~TPerson();

    char *FullName() {
        if (fullname != NULL) delete[] fullname;

        fullname = new char[strlen(fname)+strlen(lname)+2];
        sprintf(fullname, "%s %s %s", fname, lname, email);
        return fullname;
    }
private:
    char *fname;
    char *lname;
    char *email;

    char *fullname;
};

TPerson::TPerson(char *firstname, char *lastname, char *mail) {
    fname = new char[strlen(firstname)];
    lname = new char[strlen(lastname)];
    email = new char[strlen(mail)];

    strcpy(fname, firstname);
    strcpy(lname, lastname);
    strcpy(email, mail);

    fullname = NULL;
}

TPerson::~TPerson() {
    delete[] fname;
    delete[] lname;
    delete[] email;
    delete[] fullname;
}

int main()
{
    TPerson *persones[HB];

    char *fname = new char[20];
    char *lname = new char[20];
    char *email = new char[20];

    for (int i = 0; i < HB; ++i) {
        printf("fname -> ");
        scanf("%s", fname);

        printf("lname -> ");
        scanf("%s", lname);

        printf("ename -> ");
        scanf("%s", email);

        persones[i] = new TPerson(fname, lname, email);
    }

    for (int i = 0; i < HB; ++i) {
        printf("%s\n", persones[i]->FullName());
    }

    for (int i = 0; i < HB; ++i) {
        persones[i]->~TPerson();
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
227. Объявите класс TPerson и производные от него классы TStud и TProf. Класс TPerson должен содержать общую информацию о персоне. Классы TStud и TProf должны расширять информацию о персоне как о студенте и, соответственно, преподавателе.
```
#include <stdio.h>
#include <string.h>

class TPerson {
public:
    TPerson() {}

    TPerson(char *FirstName, char *LastName) {
        fname = new char[strlen(FirstName) + 1];
        strcpy(fname, FirstName);
        lname = new char[strlen(LastName) + 1];
        strcpy(lname, LastName);
    }

    ~TPerson() {
        delete[] fname;
        delete[] lname;
    }

    char *FullName() {
        char *fullname = new char[strlen(fname) + strlen(lname) + 2];
        sprintf(fullname, "%s %s", fname, lname);
        return fullname;
    }

    virtual void print() {}
private:
    char *fname;
    char *lname;
};

class TStud : public TPerson {
public:
    TStud() {}

    TStud(char *FirstName, char *LastName, int Group):
        TPerson(FirstName, LastName) { group = Group; }

    ~TStud() {}

    void print() {
        printf("%s, gr. %i\n", this->FullName(), group);
    }
private:
    int group;
};

class TProf : public TPerson {
public:
    TProf() {}

    TProf(char *FirstName, char *LastName, char *Kafedra):
        TPerson(FirstName, LastName) { kafedra = new char[strlen(Kafedra) + 1];
                                       strcpy(kafedra, Kafedra);}
    ~TProf() {
        delete[] kafedra;
    }

    void print() {
        printf("%s, dep. %s\n", this->FullName(), kafedra);
    }
private:
    char *kafedra;
};

int main()
{
    TPerson ordinaryPerson("Eto", "Tenma");
    TStud studentPerson("Shiraha", "Main", 2);
    TProf professorPerson("Kuanai", "Breadx333", "IT");

    printf("%s\n", ordinaryPerson.FullName());
    studentPerson.print();
    professorPerson.print();

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
228. Напишите программу, которая хранит в одном массиве информацию о студентах и преподавателях (см. задачу 227).
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

class TPerson {
public:
    TPerson() {}

    TPerson(char *FirstName, char *LastName) {
        fname = new char[strlen(FirstName) + 1];
        strcpy(fname, FirstName);
        lname = new char[strlen(LastName) + 1];
        strcpy(lname, LastName);
    }

    ~TPerson() {
        delete[] fname;
        delete[] lname;
    }

    char *FullName() {
        char *fullname = new char[strlen(fname) + strlen(lname) + 2];
        sprintf(fullname, "%s %s", fname, lname);
        return fullname;
    }

    virtual void print() {}
private:
    char *fname;
    char *lname;
};

class TStud : public TPerson {
public:
    TStud() {}

    TStud(char *FirstName, char *LastName, int Group):
        TPerson(FirstName, LastName) { group = Group; }

    ~TStud() {}

    void print() {
        printf("%s, gr. %i\n", this->FullName(), group);
    }
private:
    int group;
};

class TProf : public TPerson {
public:
    TProf() {}

    TProf(char *FirstName, char *LastName, char *Kafedra):
        TPerson(FirstName, LastName) { kafedra = new char[strlen(Kafedra) + 1];
                                       strcpy(kafedra, Kafedra);}
    ~TProf() {
        delete[] kafedra;
    }

    void print() {
        printf("%s, dep. %s\n", this->FullName(), kafedra);
    }
private:
    char *kafedra;
};

int main()
{
    TPerson *persones[10];

    int K = sizeof(persones)/sizeof(TPerson*);

    for (int i = 0; i < K; ++i)
        persones[i] = NULL;

    persones[0] = new TStud("Eto", "Tenma", 1358);
    persones[1] = new TStud("Shiraha", "Main", 1358);
    persones[2] = new TProf("Kuanai", "Breadx333", "IT");

    printf("All:\n");
    int i = 0;
    while (persones[i] != NULL) {
        persones[i]->print();
        ++i;
    }

    printf("\nStudents:\n");
    i = 0;
    while (persones[i] != NULL) {
        if (typeid(*persones[i]) == typeid(TStud)) {
            persones[i]->print();
        }
        ++i;
    }

    i = 0;
    while (persones[i] != NULL) {
        delete persones[i];
        ++i;
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
229. Объявите структуру book для программы работы с информацией о книгах, например, в книжном магазине.
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

struct Book {
    char *id;
    char *name;
    char *author;
    int year;
    float price;
};

int main()
{
    Book book = {"228", "Disorder", "Eto Tenma", 1337, 10};

    printf("ID: %s\n", book.id);
    printf("Name: %s\n", book.name);
    printf("Author: %s\n", book.author);
    printf("Year: %d\n", book.year);
    printf("Price: %.2f $\n", book.price);

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
230. Напишите программу, формирующую массив структур book (см. задачу 229). Информация о книгах должна вводиться с клавиатуры во время работы программы.
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

#define CNT 2

struct Book {
    Book() {}
    Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE) {
        id = new char[strlen(ID)];
        name = new char[strlen(NAME)];
        author = new char[strlen(AUTHOR)];

        strcpy(id, ID);
        strcpy(name, NAME);
        strcpy(author, AUTHOR);
        year = YEAR;
        price = PRICE;
    }
    char *id;
    char *name;
    char *author;
    int year;
    float price;
};

int main()
{
    Book *book[CNT];

    char *id = new char[20];
    char *name = new char[20];
    char *author = new char[20];
    int year;
    float price;

    for (int i = 0; i < CNT; ++i) {
        printf("Book id -> ");
        scanf("%s", id);
        printf("Book name -> ");
        scanf("%s", name);
        printf("Book author -> ");
        scanf("%s", author);
        printf("Book year -> ");
        scanf("%i", &year);
        printf("Book price -> ");
        scanf("%f", &price);

        book[i] = new Book(id, name, author, year, price);
    }

    for (int i = 0; i < CNT; ++i) {
        printf("ID: %s\n", book[i]->id);
        printf("Name: %s\n", book[i]->name);
        printf("Author: %s\n", book[i]->author);
        printf("Year: %d\n", book[i]->year);
        printf("Price: %.2f $\n", book[i]->price);
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
231. Объявите класс твоок для программы работы с информацией о книгах, например, в книжном магазине.
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

#define CNT 2

class Book {
public:
    Book() {}
    Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE);
    ~Book();
    print() {
        printf("ID: %s\n", id);
        printf("Name: %s\n", name);
        printf("Author: %s\n", author);
        printf("Year: %d\n", year);
        printf("Price: %.2f $\n", price);
    }
private:
    char *id;
    char *name;
    char *author;
    int year;
    float price;
};

Book::Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE){
    id = new char[strlen(ID)];
    name = new char[strlen(NAME)];
    author = new char[strlen(AUTHOR)];

    strcpy(id, ID);
    strcpy(name, NAME);
    strcpy(author, AUTHOR);
    year = YEAR;
    price = PRICE;
}

Book::~Book() {
    delete[] id;
    delete[] name;
    delete[] author;
}

int main()
{
    Book book("228", "Disorder", "EtoTenma", 1337, 10);

    book.print();

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
232. Напишите программу, формирующую массив объектов твоок (см. задачу 229). Информация о книгах должна вводиться с клавиатуры во время работы программы
```
#include <stdio.h>
#include <string.h>
#include <typeinfo.h>

#define CNT 2

class Book {
public:
    Book() {}
    Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE);
    ~Book();
    print() {
        printf("ID: %s\n", id);
        printf("Name: %s\n", name);
        printf("Author: %s\n", author);
        printf("Year: %d\n", year);
        printf("Price: %.2f $\n", price);
    }
private:
    char *id;
    char *name;
    char *author;
    int year;
    float price;
};

Book::Book(char *ID, char *NAME, char *AUTHOR, int YEAR, float PRICE){
    id = new char[strlen(ID)];
    name = new char[strlen(NAME)];
    author = new char[strlen(AUTHOR)];

    strcpy(id, ID);
    strcpy(name, NAME);
    strcpy(author, AUTHOR);
    year = YEAR;
    price = PRICE;
}

Book::~Book() {
    delete[] id;
    delete[] name;
    delete[] author;
}

int main()
{
    Book *book[CNT];

    char *id = new char[20];
    char *name = new char[20];
    char *author = new char[20];
    int year;
    float price;

    for (int i = 0; i < CNT; ++i) {
        printf("Book id -> ");
        scanf("%s", id);
        printf("Book name -> ");
        scanf("%s", name);
        printf("Book author -> ");
        scanf("%s", author);
        printf("Book year -> ");
        scanf("%i", &year);
        printf("Book price -> ");
        scanf("%f", &price);

        book[i] = new Book(id, name, author, year, price);
    }

    for (int i = 0; i < CNT; ++i) {
        book[i]->print();
    }

    printf("\nPress <Enter> to close");
    fflush(stdin);
    getchar();

    return 0;
}
```
