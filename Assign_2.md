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

## **Discussion :**
This C++ program demonstrates the concept of a constructor in object oriented programming. A class named myclass is defined with a default constructor that prints "Hello world".When the main() function executes, it creates an object m1 of myclass. As soon as the object is created, the constructor is automatically called.


------------------
    
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

## **Discussion :**
This C++ program defines a class myclass with two private integer variables, x and y. The class includes a default constructor and a display() function that prints the values of x and y.However, the variables x and y are not initialized in the constructor or elsewhere in the program. When the display() function is called in main() through the object c2, it attempts to print these uninitialized variables and value x,y is showing garbej value.


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

## **Discussion :**
This program demonstrates the use of a parameterized constructor in C++. The class myclass contains a private integer member x. When an object c2 is created in main() with the value 20, the parameterized constructor is called automatically, initializing x with the provided value.The constructor also prints a confirmation message: "parameterized constructor called". Then, the display() function prints the value of x.


-------------

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

## **Discussion :**
This program demonstrates the use of a class with a parameterized constructor to represent car objects. The class car contains three public data members: brand, model, and year. The constructor initializes these members with the values passed during object creation.In the main() function, two objects c1 and c2 are created with specific car details. The program then outputs the details of each car using cout.


-------------------------

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

## **Discussion :**
This program is same as above but here the parameterized constructor declare in the class and define outside the class.We konow the syntax is 
class name ::constructor name(parameter).


-------------------------

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

## **Discussion :**
This program demonstrates the use of a default constructor in C++. The class car has three private data members brand, model, and year, although they are not initialized or used in this example.The constructor car() is called automatically when objects c1 and c2 are created in the main() function. Each time an object is created, the constructor prints "default".


-------------------------
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
<img src="https://github.com/user-attachments/assets/67e4fc18-5770-4a0a-831b-307b42fce7cb">

## **Discussion :**
This program defines a car class with private attributes: brand, model, and year. A default constructor is provided, but it doesn't initialize any values.The class includes a set() function to assign values to the attributes and a display() function to print them. In the main() function, a car object c1 is created, but the set() function is not called before display(). As a result, the program outputs empty strings for brand and model, and garbage value for year.

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
        year = 2026;
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
<img src="https://github.com/user-attachments/assets/9ba40376-f320-4b57-aa5b-ed67d391ac39">

## **Discussion :**
This code is same as before, here just created two object of car class and call the display function with each of the object.So output will show two times of display function.

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
<img src="https://github.com/user-attachments/assets/b38e91a5-1660-4c61-ab75-8122fadb618a">


## **Discussion :**
Here are a default constructor and a parameterized constructor.When an c1 object is created,default constructor is called and set value for brand variable.Then c2 parametized called the parameterized constructor and set the value with its argument value.Then display function is called with c1 object then the output show the brand name and model is empty and year show garbaje value.When c2 object call the display it pass the argument for model and year but brand is empty.

