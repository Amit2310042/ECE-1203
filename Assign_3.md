## **Assignment No : 01**
## **Experiment Name :  Example.**
## **Submission Date : 13 June 2025**
----------

## **Code :**
```C
#include<iostream>
#include<string>
using namespace std;
class BaseClass{
    protected:
    int value1;
    double value2;
    public:
    BaseClass(int a,double b){
        value1=a;
        value2=b;
        cout<<"Base constructor called "<<value1<<","<<value2<<endl;
    }   
};
class DeriveClass:public BaseClass{
    private:
    string name;
    public:

    // DeriveClass(int x,double y,string s):BaseClass(x,y)  .. this is legal..not error
    // DeriveClass(int x,double y,string s):BaseClass(a,b).. this is wrong...

    DeriveClass(int a,double b,string s):BaseClass(a,b){
        name=s;
        cout<<"Derive contructor called "<<name<<endl;
    }
};
int main(){
    DeriveClass d1(10,20.3,"amit");

}

```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/abe3ea85-1c4c-4fa9-81b0-fc23b2ffe6c5">

## **Discussion :**
This C++ code demonstrates inheritance where DeriveClass is derived from BaseClass.BaseClass: It has two protected members: value1 (integer) and value2 (double).it also has a parameterized constructor that initializes these values and prints them. DeriveClass: we know that if one or more argument in base class constructor derive class need to pass those argument in base class constructor.It inherits BaseClass publicly.It has additional private member name(string).The constructor of DeriveClass explicitly calls the BaseClass constructor using initializer list (BaseClass(a, b)). Derived class constructors must call the base class constructor explicitly using the correct parameter names (like a, b instead of undeclared x, y).In the main function creates an object d1 of DeriveClass and pass the value of argument(10,20.5,"amit") and the output shows. 






----------------------------------


## **Assignment No : 02**
## **Experiment Name :  Example.**
## **Submission Date : 13 June 2025**
----------

## **Code :**
```C
class A{
    public:
    A(){
        cout<<"A"<<endl;
    }
};
class B{
    public:
    B(){
        cout<<"B"<<endl;
    }
};
class C{
    public:
    C(){
        cout<<"C"<<endl;
    }
};
class D:public A,public B,public C{
    public:
    D(){
        cout<<"D"<<endl;
    }
};
int main(){
    D c1;
}

```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/e1feb1c2-7e4d-4934-bc60-2628bd4650d1">

## **Discussion :**
This C++ code demonsrates constructor execution in multiple inheritance. When an object of class D is created, the constructors of its parent classes A, B, and C are called before the constructor of D. This follows a logical top-to-bottom order, based on the way the parent classes are listed in D's declaration (public A, public B, public C). This sequence happens automatically because when D's constructor runs, it first ensures that all base class constructors execute to properly initialize inherited properties. The ouput shows according to this (public A, public B, public C) order.Then at last it shows D constructor.

 






