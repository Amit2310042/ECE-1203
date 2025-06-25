## **Assignment No : 01**
## **Experiment Name :  Assigning Object**
## **Submission Date : 25 June 2025**
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


-------------



## **Assignment No : 02**
## **Experiment Name :  Assigning Object (stack)**
## **Submission Date : 25 June 2025**
----------

## **Code :**
```C
#include <iostream>
using namespace std;
#define size 10
class stack
{
    char stk[size];//hold the stack..
    int tos;//top of the stack..

public:
    stack();
    void push(char ch);
    char pop();
};
//initialize stack
stack::stack()
{
    tos = 0;
}
void stack::push(char ch)
{
    if (tos == size)
    {
        cout << "stack is full" << endl;
        return;
    }
    stk[tos] = ch;
    tos++;
}
char stack::pop()
{
    if (tos == 0)
    {
        cout << "Stack is empty" << endl;
        return 0;
    }
    tos--;
    return stk[tos];
}

int main()
{
    stack s1, s2;

    s1.push('a');
    s1.push('b');
    s1.push('c');
    // clone s1
    s2 = s1; // now s1 and s2 are identical
    for (int i = 0; i < 3; i++)
    {
        cout << s1.pop() << endl;
    }

    for (int i = 0; i < 3; i++)
    {
        cout << s2.pop() << endl;
    }
    return 0;
}
```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/d340e68e-51b0-4382-a756-8de1438a8466">

## **Discussion :**
This C++ program demonstrates a simple implementation of a stack using a class and a fixed-size character array. The stack class manages data with two key elements an array stk to hold up to 10 characters and an integer tos (top of stack) to track where new elements should be pushed or popped. The push function adds a character to the stack unless it’s full, while pop removes the most recently added character unless the stack is empty. In the main() function, two stack objects s1 and s2 are created. After pushing three characters ('a', 'b', and 'c') onto s1, the assignment s2 = s1 is used to clone the state of s1 into s2. This line is tells the program to make s2 an exact copy of s1 at that moment, including all elements in the stack and the current top position.


------------------------------


## **Assignment No : 03**
## **Experiment Name :  Passing objects to function**
## **Submission Date : 25 June 2025**
----------

## **Code :**
```C
#include <iostream>
using namespace std;
class Pass{
    int a;
    public:
    Pass(int p){
        a=p;
    }
    int get(){
        return a;
    }
};
int  square(Pass ob){
    return ob.get()*ob.get();
}

int main(){
    Pass x(10),y(4);
    cout<<square(x)<<endl;
    cout<<square(y)<<endl;
}

```
## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/9e66e4e6-886f-4e48-a36c-a5329952deb7">

## **Discussion :**
The class Pass contains a private integer a, which is initialized through the constructor.THe get method used to return the value oa a.In the main() function, two objects x and y are created with values 10 and 4 and then constructor is called and value of a is set.Then when square function is called, it called the get function and get function return the value a.so square function return the square of a.The same as object y. 
