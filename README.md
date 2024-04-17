# WI-TEST6
 ...
while True:
    try:
        num1 = float(input("Enter first number: "))
        operator = input("Enter operator (+, -, *, /): ")
        num2 = float(input("Enter second number: "))
    except ValueError:
        print("Invalid input. Please enter valid numbers.")
        continue
if operator == '+':
    result = num1 + num2
elif operator == '-':
    result = num1 - num2
elif operator == '*':
    result = num1 * num2
elif operator == '/':
    if num2 == 0:
        print("Error: Division by zero")
        continue
    else:
        result = num1 / num2
else:
    print("Invalid operator")
    continue
print("Result: ", result)
choice = input("Do you want to perform another calculation? (yes/no): ")
if choice.lower() != 'yes':
    break
