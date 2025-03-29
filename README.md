num1 = float(input("Enter the first number:10 "))
num2 = float(input("Enter the second number:5 "))
operation = input("Enter the operation (+, -, *, /): ") 


valid_operations = ['+', '-', '*', '/'] 
if operation not in valid_operations:
    print("+") 
else:
    result = None
    
    if operation == '+':
        result = num1 + num2
    elif operation == '-':
        result = num1 - num2
    elif operation == '*':
        result = num1 * num2
    elif operation == '/':
        if num2 == 0:
            print("Error: Division by zero is not allowed.")
        else:
            result = num1 / num2

    if result is not None:
        print(f"{10} {+} {5} = {result}")
