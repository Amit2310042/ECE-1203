## **Assignment No : 01**
## **Experiment Name :  Use of Exection hanling in Real Life Example**
## **Submission Date : 16 August 2025**
----------

## **Code :**
```C

#include <iostream>
using namespace std;

class Calculator
{
    char operation;
    double num1, num2;

public:
    void setOperation(char op, double a, double b)
    {
        if (op != '+' && op != '-' && op != '*' && op != '/')
        {
            throw "Invalid operation. Use +, -, *, or /.";
        }
        if (op == '/' && b == 0)
        {
            throw "Cannot divide by zero.";
        }
        operation = op;
        num1 = a;
        num2 = b;
    }

    double getResult()
    {
        switch (operation)
        {
        case '+':
            return num1 + num2;
        case '-':
            return num1 - num2;
        case '*':
            return num1 * num2;
        case '/':
            return num1 / num2;
        default:
            throw "Unknown error.";
        }
    }

    void show()
    {
        cout << num1 << " " << operation << " " << num2 << " = " << getResult() << "\n";
    }
};

int main()
{
    Calculator calc;
    char op;
    double a, b;
    char choice;

    cout << " Welcome to Our Modern Calculator!\n";

    do
    {
        cout << "\nEnter operation (+, -, *, /): ";
        cin >> op;

        cout << "Enter first number: ";
        cin >> a;

        cout << "Enter second number: ";
        cin >> b;

        try
        {
            calc.setOperation(op, a, b);
            calc.show();
        }
        catch (const char *msg)
        {
            cout << " Error: " << msg << "\n";
        }

        cout << "\nDo you want to perform another operation? (y/n): ";
        cin >> choice;

    } while (choice == 'y' || choice == 'Y');

    cout << "\n Thanks for using the calculator. Goodbye!\n";
    return 0;
}
```
## **Output :**
<p align="center">
<img width="1637" height="1003" alt="image" src="https://github.com/user-attachments/assets/d63c9e74-8986-438c-b5c3-a2aaad16cdcf" />
