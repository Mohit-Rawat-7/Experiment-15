# Experiment-15
## AIM
To learn about exception handling in c++.

## Problem Statement
1.) Write a c++ program to get a customized error for entering a negative number.

2.) Write a c++ program to get a customized error for entering a year less than 2000.

## Theory
In C++, exceptions represent unexpected events or errors that occur during program execution. Exception handling is the mechanism used to manage these anomalies, allowing the program to maintain control and continue running smoothly. By implementing exception handling, developers can gracefully address errors without crashing the application, ensuring a more robust and user-friendly experience.

## Program Codes
1)
```javascript
//Mohit Singh Rawat
//23070123086
# include<iostream>
using namespace std;
 int main()
 { int year;
    cout << "Enter year greater than 2000: "<<endl;
    cin>>year;

    try{
if ( year<2000)
{
    throw "You entered a year less than 2000";

}
else{
    cout<< "Entered year is: "<<year<<endl;
}
    }

    catch ( const char*msg)

    { 
        cout << msg;
        
    }
 }
```
2)
```javascript
//Mohit Singh Rawat
//23070123086
# include<iostream>
using namespace std;
 int main()
 {  float a;
    cout<< "Enter a positive  numbers: "<<endl;
    cin>>a;

try {
    if ( a<0)
    {
        throw a;
    }
else {
 cout<< "The number  is: "<<a<<endl;
 }
}
catch (const float n)
{
    cout<<"You entered " <<a<<" which is a negative number"<<n;
}
 }
 ```

## Output 
1) <img width="300" alt="Screenshot 2024-10-11 at 9 19 29 AM" src="https://github.com/user-attachments/assets/9d887dc3-44fd-465e-a5d0-423724b3a743">

2) <img width="373" alt="Screenshot 2024-10-11 at 9 21 41 AM" src="https://github.com/user-attachments/assets/d56670e3-5160-4ade-8eb9-f4d4bd1b8e28">

## Conclusion

In summary, exception handling in C++ allows developers to manage unexpected errors during program execution, ensuring that the application remains stable and responsive. This mechanism enhances the robustness of programs, enabling them to handle anomalies gracefully without crashing.

