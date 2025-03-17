# Calculator
num1 = float(input("give me the first value:  "))
print(num1)
num2 = float(input("give me the second value:  "))
print(num2)
print("1. Addition (+)")
print("2. Subtraction (-)")
print("3. Multiplication (*)")
print("4. Division (/)")
choice = input("enter choice(1/2/3/4): ")
if choice == '1':
    print(f"The result is: {num1 + num2}")
elif choice == '2':
    print(f"The result is: {num1 - num2}")
elif choice == '3':
    print(f"The result is: {num1 * num2}")
elif choice == '4':
    if num2 != 0:
        print(f"The result is: {num1 / num2}")
    else:
        print("Error: Division by zero is not allowed.")
next_calculation = input("Do you want to perform another calculation? (yes/no): ").lower()
if next_calculation != 'yes':
    print("Thank you for using the calculator. Goodbye!")
else:
    print("Run it again")
