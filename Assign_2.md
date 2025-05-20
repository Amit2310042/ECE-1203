## **Assignment No : 01**
## **Experiment Name : OOP.**
## **Submission Date : 19 May 2025**
----------

## **Code :**
```C
#include<iostream>
#include<string>
using namespace std;
class A{
    private:
    int a;
    void fun1(){
        cout<<"fun1"<<endl;
    }
    protected:
    int b;
    void fun2(){
        cout<<"fun2"<<endl;
    }
    public:
    int c;
    void fun3(){
        cout<<"fun3"<<endl;
    }
};
class B:public A{
    private:
    int d;
    void fun4(){
        cout<<"fun4"<<endl;
    }
    protected:
    int e;
    void fun5(){
        cout<<"fun5"<<endl;
    }
    public:
    int f;
    void fun6(){
        cout<<"fun6"<<endl;
    }
};
class C:public B{
    private:
    int g;
    void fun7(){
        cout<<"fun7"<<endl;
    }
    protected:
    int h;
    void fun8(){
        cout<<"fun8"<<endl;
    }
    public:
    int i;
    void fun9(){
        cout<<"fun9"<<endl;
    }
};
int main(){
    C c1;
    c1.f=343;
    c1.fun8();
    cout<<c1.f;
    c1.fun7();
    c1.a=34;
    cout<<c1.a<<endl;
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/0b9e3fdc-d9c9-4acc-a00a-20a525ec07c1">
<img src="https://github.com/user-attachments/assets/0e78f162-5154-43c4-b7d6-19a3aa35b176">


</p>

----------


