# Stage 1: Basic Calculator

num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
operator = input("Enter operator (+, -, *, /): ")

if operator == "+":
    result = num1 + num2
    print("Result =", result)

elif operator == "-":
    result = num1 - num2
    print("Result =", result)

elif operator == "*":
    result = num1 * num2
    print("Result =", result)

elif operator == "/":
    if num2 == 0:
        print("Error! Division by zero is not allowed.")
    else:
        result = num1 / num2
        print("Result =", result)

else:
    print("Invalid operator!")