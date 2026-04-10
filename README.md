C++ Calculator

A simple command-line calculator built using C++ that performs basic arithmetic operations like addition, subtraction, multiplication, and division.

📌 Features
➕ Addition
➖ Subtraction
✖️ Multiplication
➗ Division
🧠 User-friendly menu-driven interface
⚠️ Handles division by zero errors
🛠️ Technologies Used
Language: C++
Compiler: g++ / any C++ compatible compiler
Platform: Cross-platform (Windows, Linux, macOS)
📂 Project Structure
calculator/
│── main.cpp       # Main source code
│── README.md      # Project documentation
🚀 Getting Started
1. Clone the Repository
git clone https://github.com/your-username/cpp-calculator.git
cd cpp-calculator
2. Compile the Code
g++ main.cpp -o calculator
3. Run the Program
./calculator
💻 Usage
Run the program
Select an operation from the menu
Enter two numbers
View the result
Example
Select operation:
1. Add
2. Subtract
3. Multiply
4. Divide

Enter choice: 1
Enter two numbers: 5 3

Result: 8
⚠️ Error Handling
Division by zero is not allowed
Invalid menu choices are handled gracefully
📸 Sample Code Snippet
#include <iostream>
using namespace std;

int main() {
    int choice;
    double a, b;

    cout << "1. Add\n2. Subtract\n3. Multiply\n4. Divide\n";
    cin >> choice;

    cout << "Enter two numbers: ";
    cin >> a >> b;

    switch(choice) {
        case 1: cout << "Result: " << a + b; break;
        case 2: cout << "Result: " << a - b; break;
        case 3: cout << "Result: " << a * b; break;
        case 4:
            if (b != 0)
                cout << "Result: " << a / b;
            else
                cout << "Error! Division by zero.";
            break;
        default:
            cout << "Invalid choice";
    }

    return 0;
}
🔮 Future Improvements
Support for advanced operations (square root, power, etc.)
GUI-based calculator
Continuous calculation mode
Input validation enhancements
🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit a pull request.

📄 License

This project is open-source and available under the MIT License.
