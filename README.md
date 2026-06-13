# calculator
def add(a,b):
    return a+b
def subtract(a,b):
    return a-b
def multiply(a,b):
    return a*b
def divide(a,b):
    if b != 0:
        return a/b
    else:
        return "Error"
while True:
    num1 = float(input("Enter your frst number: "))
    num2 = float(input("Enter your  second number: "))
    print("Choose operation :")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Mltiplicattion")
    print("4. Division")
    choice = input("Enter your choice (1/2/3/4) :")
    print(choice)
    if choice == "1":
        print(f"{num1}+{num2}={add(num1,num2)}")
    elif choice == "2":
        print(f"{num1}-{num2}={subtract(num1,num2)}")
    elif choice == "3":
        print(f"{num1}*{num2} = {multiply(num1,num2)}")
    elif choice == "4":
        result = num1/num2
        if result == "Error":
            print("Error: Division by zero is not possible")
        else:
            print(f"{num1}/{num2}={result}")
    else:
        print("Invalid choice!")
    
    again = input("\n Calculate again? (y/n) :")
    if again.lower() == "n":
        print("Thank you, Goodbye👋...")
        break
