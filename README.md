# respitirie-name-Lab-1-to-7-
#include <iostream>
using namespace std;

int main() {
    // Declare integer variables
    int a = 5, b = 10, c = 5;

    // Relational operator tests
    cout << "a == b: " << (a == b) << endl;       // checks if a equals b
    cout << "a != c: " << (a != c) << endl;       // checks if a is not equal to c
    cout << "a < b: " << (a < b) << endl;         // checks if a is less than b
    cout << "b > c: " << (b > c) << endl;         // checks if b is greater than c
    cout << "(a + c) <= b: " << ((a + c) <= b) << endl; // checks if sum of a and c is less than or equal to b

    // Character comparison
    cout << "'A' < 'a': " << ('A' < 'a') << endl; // compares ASCII values of 'A' and 'a'

    return 0;
}

#include <iostream>
using namespace std;

int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;

    // One-way selection: only execute if condition is true
    if (num > 0) {
        cout << "The number is positive." << endl;
    }

    return 0;
}
#include <iostream>
using namespace std;

int main() {
    int grade;
    cout << "Enter grade: ";
    cin >> grade;

    // Two-way selection: if...else
    if (grade >= 75) {
        cout << "Result: Pass" << endl;
    } else {
        cout << "Result: Fail" << endl;
    }

    return 0;
}

#include <iostream>
using namespace std;

int main() {
    int grade;
    cout << "Enter grade: ";
    cin >> grade;

    // Two-way selection with compound statements
    if (grade >= 75) {
        // Compound statement: multiple instructions grouped with braces
        cout << "Result: Pass" << endl;
        cout << "Congratulations!" << endl;
        cout << "Keep up the good work." << endl;
    } else {
        cout << "Result: Fail" << endl;
    }

    return 0;
}
#include <iostream>
using namespace std;

int main() {
    int grade;
    cout << "Enter grade: ";
    cin >> grade;

    // Two-way selection with compound statements
    if (grade >= 75) {
        // Compound statement: multiple instructions grouped with braces
        cout << "Result: Pass" << endl;
        cout << "Congratulations!" << endl;
        cout << "Keep up the good work." << endl;
    } else {
        cout << "Result: Fail" << endl;
    }

    return 0;
}

#include <iostream>
using namespace std;

int main() {
    int grade;
    cout << "Enter grade: ";
    cin >> grade;

    // Nested if statements
    if (grade >= 75) {           // First main condition: passing grades
        if (grade >= 90) {
            cout << "Remark: Excellent" << endl;
        } else if (grade >= 80) {
            cout << "Remark: Very Good" << endl;
        } else {
            cout << "Remark: Satisfactory" << endl;
        }
    } else {                      // Failing grades
        cout << "Remark: Fail" << endl;
    }

    return 0;
}
#include <iostream>
using namespace std;

int main() {
    int choice;
    const double PI = 3.14159;

    cout << "Menu:\n";
    cout << "1. Compute Area of Circle\n";
    cout << "2. Compute Area of Rectangle\n";
    cout << "3. Exit\n";

    cout << "Enter your choice: ";
    cin >> choice;

    switch (choice) {
        case 1: {  // Area of Circle
            double radius;
            cout << "Enter radius: ";
            cin >> radius;
            cout << "Area of Circle: " << PI * radius * radius << endl;
            break;
        }
        case 2: {  // Area of Rectangle
            double length, width;
            cout << "Enter length: ";
            cin >> length;
            cout << "Enter width: ";
            cin >> width;
            cout << "Area of Rectangle: " << length * width << endl;
            break;
        }
        case 3:  // Exit
            cout << "Goodbye!" << endl;
            break;
        default:  // Invalid input
            cout << "Invalid choice." << endl;
    }

    return 0;
}

#include <iostream>
using namespace std;

int main() {
    int grade, courseCode;
    string courseName;

    // Ask for input
    cout << "Enter grade (0-100): ";
    cin >> grade;
    cout << "Enter course code (1-3): ";
    cin >> courseCode;

    // Determine Pass/Fail using if-else
    if (grade >= 75) {
        cout << "Result: Pass" << endl;
    } else {
        cout << "Result: Fail" << endl;
    }

    // Determine course name using switch
    switch (courseCode) {
        case 1:
            courseName = "Programming Fundamentals";
            break;
        case 2:
            courseName = "Data Structures";
            break;
        case 3:
            courseName = "Computer Networks";
            break;
        default:
            courseName = "Invalid course code";
    }

    cout << "Course: " << courseName << endl;

    return 0;
}

