## **Assignment No : 01**
## **Experiment Name :  Assigning Object**
## **Submission Date : 13 June 2025**
----------

## **Code :**
```C
#include <iostream>
using namespace std;

class A{
    int a,b;
    public:
    void set(int p,int q){a=p;b=q;}
    void show() {cout << a <<" "<< b<<endl;}
};
int main(){
    A o1,o2;
    o1.set(45,34);
    o2=o1;  //assign o1 to o2.
    o1.show();
    o2.show();
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/9e66e4e6-886f-4e48-a36c-a5329952deb7">

## **Discussion :**
This c++ code is an example of assigning object.Here,in the class set function is for set value of a,b.In the main function two object is created for the class.First, set is called with by object o1.And value is passed to the set funtion.Next, we assign o1 to o2.and called the show function by o2.When one object assign to another a bit wise copy of all the data members is made.By assigning the the contents of all of data of o1's are copied to o2.Then o2.show() will print the same data as o1.show().
