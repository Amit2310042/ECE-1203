## **Assignment No : 01**
## **Experiment Name :  Uses of some keyword**
## **Submission Date : 19 June 2025**
----------
## **signed **
Declares that a variable can hold both positive and negative values. Typically used with char or int. int is signed by default, but it’s useful for clarity.

## **Example :**
```C
signed int temp = -15;
char letter = 'A';
signed char signChar = -20;  // explicitly signed

```
## **sizeof **
Determines the size (in bytes) of a data type or object.Evaluated at compile time. Often used for memory management or array calculations.



## **Example :**
```C
int a = 10;
cout << "Size of int: " << sizeof(a) << " bytes";  // output: 4 bytes

```

## **static **
Modifies scope and lifetime.
1.  Inside a function: variable retains value between calls.
2.  In class: shared by all objects.
3.  In global scope: restricts visibility to file 


## **Example :**
```C
void countCall() {
    static int call = 0;
    call++;
    cout << "Called " << call << " times\n";
}

countCall();  // Output: Called 1 times
countCall();  // Output: Called 2 times
countCall();  // Output: Called 3 times

```
## **static_cast **
Converts one type to another safely.Safer than C-style casts, can't cast unrelated types.

## **Example :**
```C
double pi = 3.1415;
int approx = static_cast<int>(pi);  // approx = 3


```

## **struct **
Combines variables into a single custom type.Default access modifier is public.


## **Example :**
```C
struct Book {
    string title;
    int pages;
};

Book b = {"C++ Guide", 250};
cout << b.title;

```

## **switch **
Used to choose between multiple cases.Selects code to execute based on a variable's value.Works best with integral or enum types, break prevents fall through.

## **Example :**
```C
int grade = 2;
switch (grade) {
    case 1: cout << "Poor"; break;
    case 2: cout << "Fair"; break;
    case 3: cout << "Excellent"; break;
    default: cout << "Invalid grade";
}

```
## **template **
Used to choose between multiple cases.Selects code to execute based on a variable's value.Works best with integral or enum types, break prevents fall through.

## **Example :**
```C
template <typename T>
T max(T a, T b) {
    return (a > b) ? a : b;
}

cout << max(4, 7);         // Works with int
cout << max(2.5, 1.3);     // Works with double


```

## **this **
Pointer to the current object inside a class.Useful when parameter names shadow member variables.


## **Example :**
```C
class Car {
    string model;
public:
    void setModel(string model) {
        this->model = model;  
    }
};



```


## **true **
Represents Boolean truth.Used for logic, conditionals and loops.

## **Example :**
```C
bool ready = true;
if (ready)
    cout << "All systems go!"; //output:All systems go!


```

## **throw **
The throw keyword is used to signal that an exception (error condition) has occurred during program execution. It's part of C++'s exception handling system, which uses three main components:
try block: Code that might cause an exception.
throw: Sends the exception.
catch: Handles the exception.
Errors like division by zero, invalid input, or file access failure can stop your program. Instead of crashing, you can throw an exception and gracefully recover using catch.



## **Example :**
```C
#include <iostream>
using namespace std;

void divide(int a, int b) {
    if (b == 0)
        throw "Division by zero error!";
    cout << "Result: " << a / b << endl;
}

int main() {
    try {
        divide(10, 2);   // This works
        divide(8, 0);    // This throws
        divide(5, 1);    // This is skipped
    } catch (const char* msg) {
        cout << "Caught exception: " << msg << endl;
    }

    return 0;
}

output:
Result: 5
Caught exception: Division by zero error!


```
