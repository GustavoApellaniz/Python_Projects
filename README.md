# Python_Projects
A collection of small Python programs I wrote while studying programming. Each folder is a self-contained project that focuses on one or more core concepts, from basic syntax to object-oriented programming.

The goal of this repository is to practice, experiment and keep a record of my progress.

What I studied
Basic structure of a Python program: variables, data types, input/output, f-strings and functions
Conditionals: if, elif and else to control the flow of a program
Loops: while and for, including counters and accumulators
Object-Oriented Programming (OOP): classes, objects, attributes, methods and custom exceptions
Error handling: try / except, input validation and raising exceptions
Practical examples: small programs that combine these concepts
Repository structure
.
├── Projects_python/     # Small projects grouped by topic
│   ├── project_1/
│   ├── project_2/
│   └── ...
└── README.md

Each project folder contains one or more .py files that can be run on their own.

Example

A program that asks how many numbers the user wants to add, validates each input with a custom exception and prints the total.

python
class NegativeNumberError(Exception):
    pass


i = 0
total = 0

n = int(input("How many numbers do you want to add? "))

while i < n:
    try:
        y = int(input("Enter a number: "))
        i += 1
        if y < 0:
            raise NegativeNumberError
        total += y
    except NegativeNumberError:
        print("Negative number")

print(f"Total: {total}")

Concepts used: while loop, counter and accumulator, if, custom exception class, try / except and f-strings.

How to run
Make sure Python 3 is installed:
bash
   python3 --version
Clone the repository:
bash
   git clone https://github.com/GustavoApellaniz/programas_testes_realizados.git
   cd programas_testes_realizados
Run any program:
bash
   python3 path/to/file.py
Notes

These are learning exercises, so the code is simple and may be improved over time. Feedback and suggestions are welcome.

Author

Gustavo Fraga Apellaniz GitHub: @GustavoApellaniz
