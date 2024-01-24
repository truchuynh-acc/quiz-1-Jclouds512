[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/tYncE4AO)
# quiz1_class_and_objects

## Instructions:
Please fill in the blank
```cplusplus
/*
* Name: Jason Lavery
*/

// Question: Create a C++ class representing a car with attributes like model, year, and color. Include a method to display car details.
// Answer: -------------I designed my solution below-------------------------- here
// This is my Program for the

#include <iostream> // include input and output
#include <iomanip> // include input and output manipulation
#include <cstring> // include strings

using namespace std; // standard namess

class Car {
private:
    string model;
    int year;
    string color;
public:
    
    string setModel()
    {
        string myModel;
        cout << "What is the model of your car? ";
        cin >> myModel;
        return myModel;
    }


    void getModel(string myModel)
    {
       model = myModel;
    }

    int setYear()
    {
        int myYear;
        cout << "What is the model of your car? ";
        cin >> myYear;
        return myYear;
    }

    void getYear(int myYear)
    {
       year = myYear;
    }

    string setColor()
    {
        string myColor;
        cout << "What is the model of your car? ";
        cin >> myColor;
        return myColor;
    }

    void getColor(string myColor)
    {
       color = myColor;
    }

    void displayDetails() {
        cout << "Model: " << model << ", Year: " << year << ", Color: " << color << std::endl;
    }
};

int main() {
    Car myCar;
    string theModel = myCar.setModel();
    myCar.getModel(theModel);

    int theYear = myCar.setYear();
    myCar.getYear(theYear);

    string theColor = myCar.setColor();
    myCar.getColor(theColor);

    myCar.displayDetails();
    return 0;
}
