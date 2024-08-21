# INTERNEPEDIA
# tast 1 calculator

def calculator():
    print('hey Welcome to the calculator')
    while True:
        print("\nChoose an operation:")
        print("1. Addition")
        print("2. Subtraction")
        print("3. Multiplication")
        print("4. Division")
        print("5. Exit")
        choice = input("Enter your choice ( 1to 5): ")
        if choice == "5":
            print("Farewell Exitted !")
            break
        elif choice in ["1", "2", "3", "4"]:
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
            if choice == "1":
                print(f"Result: {num1 + num2}")
            elif choice == "2":
                print(f"Result: {num1 - num2}")
            elif choice == "3":
                print(f"Result: {num1 * num2}")
            elif choice == "4":
                if num2 != 0:
                    print(f"Result: {num1 / num2}")
                else:
                    print("Error: Division by zero is not allowed.")
        else:
            print("Invalid choice. Please choose a valid operation.")
if __name__ == "__main__":
    calculator()
