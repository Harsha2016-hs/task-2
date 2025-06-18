# task-2
# 📱 Phone-Style Simple Calculator

print(" 1 2 3")
print(" 4 5 6")
print(" 7 8 9")
print("   10 ")

# Input first number
num1 = float(input("Enter first number: "))

# Show operation menu
print("\nSelect operation:")
print("[1]  Add")
print("[2]  Subtract")
print("[3]   Multiply")
print("[4]  Divide")

# User selects the operation
choice = input("\nEnter your choice (1/2/3/4): ")

# Input second number
num2 = float(input("Enter second number: "))

# Perform calculation based on choice
if choice == '1':
    result = num1 + num2
    symbol = '+'
elif choice == '2':
    result = num1 - num2
    symbol = '-'
elif choice == '3':
    result = num1 * num2
    symbol = '×'
elif choice == '4':
    if num2 != 0:
        result = num1 / num2
        symbol = '÷'
    else:
        print("\n 0")
        exit()
else:
    print("\n Invalid choice. Please enter 1 to 4.")
    exit()

# Display output in a nice way like a calculator
print("\n========== RESULT ==========")
print(f"  {num1} {symbol} {num2} = {result}")
print("============================")
