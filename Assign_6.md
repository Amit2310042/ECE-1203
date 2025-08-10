## **Assignment No : 01**
## **Experiment Name :  Ex-1**
## **Submission Date : 10 August 2025**
----------

## **Code :**
```C
#include <bits/stdc++.h>
using namespace std;
int main()
{
    cout << "Start" << endl;
    try
    {
        cout << "Inside try block" << endl;
        throw 10;
        cout << "This will not shown";
    }
    catch (int i)
    {
        cout << "Caught one! Number is : ";
        cout << i << endl;
    }
    cout << "End " << endl;
}
```
## **Output :**
<p align="center">
<img width="1917" height="655" alt="image" src="https://github.com/user-attachments/assets/0b2036d0-7a4d-4f03-be90-961c64422f8b" />




-----------------------------


## **Assignment No : 02**
## **Experiment Name :   Ex-2**
## **Submission Date :  10 August 2025**
----------

## **Code :**
```C
#include<bits/stdc++.h>
using namespace std;
int main()
{
    cout<<"Start"<<endl;
    try
    {
        cout<<"Inside try block"<<endl;
        throw 10;
        cout<<"This will not shown";
    }
    catch(double i)
    {
        cout<<"Caught one! Number is : ";
        cout<<i<<endl;

    }
    cout<<"End "<<endl;
}
```
## **Output :**
<p align="center">
<img width="1850" height="667" alt="image" src="https://github.com/user-attachments/assets/fa6cb3f1-d738-4818-9e16-c2f1aeb1d099" />




---------------------------




## **Assignment No : 03**
## **Experiment Name : Ex-3t**
## **Submission Date : 10 August 2025**
----------

## **Code :**
```C
#include <bits/stdc++.h>
using namespace std;
void Xtest(int test)
{
    cout << "inside Xtest, test is :" << test << endl;
    if (test)
        throw test;
}

int main()
{
    cout << "Start" << endl;
    try
    {
        Xtest(0);
        Xtest(1);
        Xtest(2);
    }
    catch (int i)
    {
        cout << "Caught one! Number is : ";
        cout << i << endl;
    }
    cout << "End " << endl;
}
```
## **Output :**
<p align="center">
<img width="1866" height="551" alt="image" src="https://github.com/user-attachments/assets/5b9da355-11bf-4e8c-93f9-28af65b82018" />




------------------------------





## **Assignment No : 04**
## **Experiment Name :  Ex-4**
## **Submission Date :  10 August 2025**
----------

## **Code :**
```C

#include <bits/stdc++.h>
using namespace std;
void Xtest(int test)
{
    try
    {
        if (test)
            throw test;
    }
    catch (int i)
    {
        cout << "Caught one! Number is : ";
        cout << i << endl;
    }
}

int main()
{
    cout << "Start" << endl;

    Xtest(0);
    Xtest(1);
    Xtest(2);
    Xtest(3);

    cout << "End " << endl;

```
## **Output :**
<p align="center">
<img width="1841" height="515" alt="image" src="https://github.com/user-attachments/assets/5d1c21d5-a26a-4df0-902c-9cbb17355696" />





----------------------------





## **Assignment No : 05**
## **Experiment Name :  Ex-5**
## **Submission Date :  10 August 2025**
----------

## **Code :**
```C

#include <bits/stdc++.h>
using namespace std;
void Xtest(int test)
{
    try
    {
        if (test)
            throw test;
            else
            throw "Value is zero";
    }
    catch (int i)
    {
        cout << "Caught one! Number is : ";
        cout << i << endl;
    }
    catch (const char *str)
    {
        cout << "Caught a string  : ";
        cout << str << endl;
    }
}

int main()
{
    cout << "Start" << endl;

    Xtest(1);
    Xtest(2);
    Xtest(0);
    Xtest(3);

    cout << "End " << endl;
}

```
## **Output :**
<p align="center">
<img width="1837" height="547" alt="image" src="https://github.com/user-attachments/assets/2d62cd93-dd3d-4c3a-8be8-36297fb35b43" />
