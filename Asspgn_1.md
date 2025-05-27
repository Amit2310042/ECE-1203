## **Assignment No : 01**
## **Experiment Name : OOP.**
## **Submission Date : 28 May 2025**
----------

## **Code :**
```C
#include<iostream>
#include<string>
using namespace std;
//base class
class A{
    protected:
    int b;
};
//derived class
class B:public A{
    public:
    void set(int s){
        b=s;
    }
    int get(){
        return b;
    }
};


int main(){
    B c1;
   c1.set(1200);
   cout<<c1.get();
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/d92b2a39-e281-4ab4-86ff-bf9ffe287943">



</p>
