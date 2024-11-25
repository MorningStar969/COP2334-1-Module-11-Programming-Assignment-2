# COP2334-1-Module-11-Programming-Assignment-2
This is a GitHub repository link for the second Programming Assignment of Module 11.

// This program is used to figure out a college student's name, age, and Grade Point Average.

// include the iostream library
#include <iostream>
#include <string> // include the string library
using namespace std; // use the standard namespace

class Student { // create a class called Student
private: // private variables
    string name; // name of the student
    int age; // age of the student
    char grade; // grade of the student
public: // public variables
    // Constructor
    Student(string n, int a, char g) { // constructor with parameters
        name = n; // set the name to the parameter
        age = a; // set the age to the parameter
        grade = g; // set the grade to the parameter
    }
    // Setter methods
    void setName(string n) { // set the name to the parameter
        name = n; // set the name to the parameter
    }
    void setAge(int a) { // set the age to the parameter
        age = a; // set the age to the parameter
    }
    void setGrade(char g) { // set the grade to the parameter
        grade = g; // set the grade to the parameter
    }
    // Getter methods
    string getName() { // get the name
        return name; // return the name
    }
    int getAge() { // get the age
        return age; // return the age
    }
    char getGrade() { // get the grade
        return grade; // return the grade
    }
    // Display method 
    void display() { // display the student's information
        cout << "Name: " << name << endl; // display the name
        cout << "Age: " << age << endl; // display the age
        cout << "Grade: " << grade << endl; // display the grade
    } // end of display method
}; // end of class

int main() { // start of main function
    // Instantiate two Student objects
    Student student1("Greg", 20, 'A'); // create a student object with name Greg, age 20, and grade A.
    Student student2("Rowley", 19, 'B'); // create a student object with name Rowley, age 19, and grade B.
    // Use setter methods to assign values to one object
    student1.setName("Greg"); // set the name to Greg
    student1.setAge(20); // set the age to 20
    student1.setGrade('A'); // set the grade to A
    // Display details for both objects using the display method
    student1.display(); // display the details for student1
    student2.display(); // display the details for student2
    return 0; // return 0 to indicate successful execution.
}
