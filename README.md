# Function to add two numbers
def add(a, b):
    return a + b

# Function to subtract two numbers
def subtract(a, b):
    return a - b

# Function to multiply two numbers
def multiply(a, b):
    return a * b

# Function to divide two numbers
def divide(a, b):
    if b == 0:
        return "Error!"
    else:
        return a / b

# Display message
print("simple calculator")

# Prompt user for input
num1 = float(input("Enter your first number: "))
num2 = float(input("Enter  your second number: "))

print("Available operations:")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")

# Prompt user to enter operation
operation = input("Enter operation number (1/2/3/4): ")

# Perform calculation based on user choice
if operation == '1':
    print(num1, "+", num2, "=", add(num1, num2))
elif operation == '2':
    print(num1, "-", num2, "=", subtract(num1, num2))
elif operation == '3':
    print(num1, "*", num2, "=", multiply(num1, num2))
elif operation == '4':
    print(num1, "/", num2, "=", divide(num1, num2))
else:
    print("Invalid input")

print("Thank you for using the Simple Calculator!")
