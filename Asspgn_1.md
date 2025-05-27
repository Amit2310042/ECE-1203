## **Assignment No : 01**
## **Experiment Name : Constructor.**
## **Submission Date : 28 May 2025**
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
<img src="https://github.com/user-attachments/assets/d92b2a39-e281-4ab4-86ff-bf9ffe287943">



</p>

----------



## **Assignment No : 02**
## **Experiment Name : Constructor.**
## **Submission Date : 28 May 2025**
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
<img src="https://github.com/user-attachments/assets/2d75b059-342d-4338-aefc-32292766a7b1">



</p>

----------


## **Assignment No : 03 **
## **Experiment Name : Constructor.**
## **Submission Date : 28 May 2025**
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
<img src="https://github.com/user-attachments/assets/5821e97f-84d0-4086-84fa-075714e45cc5">



</p>

------------
## **Assignment No : 04**
## **Experiment Name : Constructor.**
## **Submission Date : 28 May 2025**
----------

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
<img src="https://github.com/user-attachments/assets/ec2ad3ad-4732-4df9-9243-73b6e808e41a">



</p>

----------



## **Assignment No : 05**
## **Experiment Name : Constructor.**
## **Submission Date : 28 May 2025**
----------

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
<img src="https://github.com/user-attachments/assets/0bffb663-2950-41cb-80e6-cf32f0f3913a">



</p>

----------


## **Assignment No : 06**
## **Experiment Name : Constructor.**
## **Submission Date : 28 May 2025**
----------

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
<img src="https://github.com/user-attachments/assets/b4e81991-7132-4b2a-889f-5854bd0327f7">



</p>

----------



## **Assignment No : 07**
## **Experiment Name : Constructor.**
## **Submission Date : 28 May 2025**
----------

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
<img src="https://github.com/user-attachments/assets/6ed62e6d-5c16-4b3f-83e1-9f07baf370d2">



</p>

----------


## **Assignment No : 08**
## **Experiment Name : Constructor.**
## **Submission Date : 28 May 2025**
----------

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
        brand = "BMW";
        model = "e3";
        int year = 2026;
    }

    void display()
    {
        cout << "brand " << brand << endl;
        cout << "model " << model << endl;
        cout << "year " << year << endl;
    }
};
int main()
{
    car c1, c2;
    c1.display();
    c2.display();
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/cd64c0bb-d2c4-4429-b8c5-8122757f738a">



</p>

----------


## **Assignment No : 09**
## **Experiment Name : Constructor.**
## **Submission Date : 28 May 2025**
----------

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
        brand = "mustang";
    }
    car(string mod, int ye)
    {
        model = mod;
        year = ye;
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
    car c1, c2("f3", 2020);
    c1.display();
    c2.display();
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/3f6d1e01-c81d-49e0-974d-4f6ac7b1ec5b">



</p>

----------

