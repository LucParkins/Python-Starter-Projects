# AUTHOR: Luc Parkins
# CLI Calculator
# Project: Starter Python
# This version does not allow multi input

# Functions
def addition(num1,num2):
    print("\nAddition Calculator")
    return num1 + num2

def subtraction(num1,num2):
    print("\nSubtraction Calculator")
    return num1 - num2

def multiplication(num1,num2):
    print("\nMultiplication Calculator")
    return num1 * num2

def division(num1,num2):
    print("\nDivision Calculator")
    return num1 / num2

# Utility, used to validate user input and process which function to use
functions_dictionary = {
    "+":addition,
    "-":subtraction,
    "/":division,
    "*":multiplication
}

# A Welcome message with operators to guide the user
print("-Welcome to my CLI Calculator-\n"
      "Operators: + - / *\n")

number1_success = False
while not number1_success:
    try:
        number1 = float(input("Enter a first number: "))
    except ValueError:
        print("\nInvalid input. Please enter a numeric value.")
    else:
        number1_success = True

operator_success = False
while not operator_success:
    operator = input("Enter a operator:")
    if operator in functions_dictionary:
        operator_success = True
    else:
        operator_success = False
        print("\nInvalid operator. Please enter a valid operator.")

number2_success = False
while not number2_success:
    try:
        number2 = float(input("Enter a second number: "))
    except ValueError:
        print("\nInvalid input. Please enter a numeric value.")
    else:
        number2_success = True

result = functions_dictionary[operator](number1, number2)
print(f"Result = {result}")
