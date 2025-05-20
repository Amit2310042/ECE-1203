## **Assignment No : 02**
## **Experiment Name : Constructor example.**
## **Submission Date : 21 May 2025**
----------

## **Code :**
```C
#include<iostream>
#include<string>
using namespace std;
class myclass{
    public:
    myclass(){
        cout<<"Hello world";
    }
};
int main(){
    myclass m1;
    return 0;
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/379adb83-1933-41b5-9aae-9f672aed0d53">

    
## **Code :**
```C
#include <iostream>
#include <string>
using namespace std;
class myclass
{
private:
    int x;
    int y;

public:
    myclass()
    {
    }
    void display()
    {
        cout << "vlaue of x" << x << endl;
        cout << "vlaue of y" << y << endl;
    }
};
int main()
{
    myclass c2;
    c2.display();
    return 0;
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/bb36353f-1d1a-403a-ab09-5a048e2a0106">


</p>

----------


## **Code :**
```C
#include <iostream>
#include <string>
using namespace std;
class myclass
{
private:
    int x;

public:
    myclass(int value)
    {
        x = value;
        cout << "parameterized constructor called" << endl;
    }
    void display()
    {
        cout << "vlaue of x " << x << endl;
    }
};
int main()
{
    myclass c2(20);
    c2.display();
    return 0;
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/10180865-e7db-48d3-bc3c-0197fc22b0de">



## **Code :**
```C
#include <iostream>
#include <string>
using namespace std;
class car
{
public:
    string brand;
    string model;
    int year;
    car(string x, string y, int z)
    {
        brand = x;
        model = y;
        year = z;
    }
};
int main()
{
    car c1("bmw", "sf", 2025);
    car c2("mustang", "t3", 2026);

    cout << "car1 " << c1.brand << " " << c1.model << " " << c1.year << endl;
    cout << "car2 " << c2.brand << " " << c2.model << " " << c2.year << endl;
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/02b8b0e4-1130-4581-9167-b0f0ed1e91aa">



## **Code :**
```C
#include <iostream>
#include <string>
using namespace std;
class car
{
public:
    string brand;
    string model;
    int year;
    car(string x, string y, int z);
};
car::car(string x, string y, int z)
{ // outside class
    {
        brand = x;
        model = y;
        year = z;
    }
}
int main()
{
    car c1("bmw", "sf", 2025);
    car c2("mustang", "t3", 2026);

    cout << "car1 " << c1.brand << " " << c1.model << " " << c1.year << endl;
    cout << "car2 " << c2.brand << " " << c2.model << " " << c2.year << endl;
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/b2b5ef4a-0973-48f0-bc8b-f9deafc99d28">



## **Code :**
```C
// constructor example 1
#include <iostream>
#include <string>
using namespace std;
class car
{
private:
    string brand;
    string model;
    int year;

public:
    car()
    {
        cout << "default" << endl;
    }
};
int main()
{
    car c1, c2;
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/e4db00a1-c0ab-475d-befa-d3e66bb69642">


## **Code :**
```C
// constructor example 1
#include <iostream>
#include <string>
using namespace std;
class car
{
private:
    string brand;
    string model;
    int year;

public:
    car() {}
    void set(string a, string b, int c)
    {
        brand = a;
        model = b;
        year = c;
    }
    void display()
    {
        cout << "brand" << brand << endl;
        cout << "model" << model << endl;
        cout << "year" << year << endl;
    }
};
int main()
{
    car c1;
    c1.display();
}
```
## **Output :**
<p align="center">
<img src="">


