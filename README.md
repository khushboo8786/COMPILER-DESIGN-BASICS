# COMPILER-DESIGN-BASICS

*COMPANY*:CODTECH IT SOLUTIONS

*NAME*:KHUSHBOO KUMARI

*INTERN ID*:CT04DN1859

*DOMAIN*:C++

*DURATION*:4 WEEKS

*MENTOR*:NEELA SANTHOSH KUMAR

This project demonstrates the implementation of a recursive descent parser — a technique commonly used in the front-end of compilers and interpreters. The evaluator allows users to enter arithmetic expressions involving addition, subtraction, multiplication, division, and parentheses, and returns the evaluated result. It mimics the behavior of a basic calculator but is built entirely through custom logic without relying on any external libraries for parsing or evaluation.

Project Overview
The goal of the project was to build a system that could understand and compute the result of complex mathematical expressions typed by the user in real time. The expressions can include multiple levels of nested parentheses and follow the standard order of operations (also known as BODMAS or PEMDAS rules). For instance, an input such as (3 + 5) * (10 - 4) / 2 would be parsed and evaluated correctly by this system.

To achieve this, I designed a class that internally processes each input expression. The evaluator is structured to read the input from left to right, identify numerical values and operators, and evaluate them in the correct order of precedence. It provides a real-time interface where the user can continuously enter new expressions or exit the program at any point.

Technical Design
At the core of the project is a recursive parsing system that breaks the evaluation process into distinct stages based on operator precedence. The system consists of the following layers:

Expression Layer: Handles the lowest precedence operations — addition and subtraction.

Term Layer: Handles multiplication and division, which have higher precedence than addition/subtraction.

Factor Layer: Responsible for evaluating parentheses and numeric values.

The parsing begins from the highest level (expressions) and recursively evaluates terms and factors within them. This structure ensures that each part of the expression is evaluated correctly and in the right order, even when parentheses are used to override precedence.

The input string is processed character by character using a simple cursor system that tracks the current position. Special functions handle the extraction of numbers, skipping of white spaces, and identification of operators. Proper error checking is implemented to detect issues such as malformed expressions, unexpected characters, or division by zero. If an error is found during parsing or evaluation, the program responds with an appropriate error message, allowing the user to retry.

User Experience
The interface is text-based and runs entirely within the command line. When launched, the program displays a welcome message and prompts the user to enter a mathematical expression. The system supports continuous input — users can evaluate as many expressions as they like until they type "exit" to terminate the program.

For each input, the evaluator attempts to parse and compute the result. If successful, the result is displayed immediately. If the expression is invalid, a descriptive error message is printed. This interaction loop allows users to experiment with a variety of expressions and receive instant feedback.

Key Features Implemented
Evaluation of complex expressions with multiple operators and parentheses.

Operator precedence handling (e.g., multiplication before addition).

Robust error handling for invalid inputs, syntax errors, and divide-by-zero cases.

Interactive input loop using standard input/output.

Clean, modular design using object-oriented principles.

Learning Outcomes
This project deepened my understanding of how interpreters and compilers handle expression parsing. I gained hands-on experience with recursive functions, operator precedence management, and building custom parsers. It also reinforced key programming concepts like string manipulation, control structures, and exception handling in C++.

Moreover, I learned how to write maintainable code using classes and how to separate logic cleanly across methods. The project mirrors real-world problems in programming language development, data processing, and scripting engine implementation.

Conclusion
The Arithmetic Expression Evaluator is a powerful example of how low-level parsing techniques can be used to create an interactive and intelligent system. It showcases a blend of algorithmic thinking and practical C++ programming. As part of my internship, this project was not only a technical achievement but also a significant learning milestone, giving me insight into how complex user input can be validated, interpreted, and executed systematically.
