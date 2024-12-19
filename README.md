def calculator():
    print("Simple Calculator")
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")

    while True:
        choice = input("Enter choice (1/2/3/4): ")

        if choice in ['1', '2', '3', '4']:
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))

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
                    print("Error! Division by zero.")
        else:
            print("Invalid Input. Try again.")

        next_calc = input("Do you want to perform another calculation? (yes/no): ")
        if next_calc.lower() != 'yes':
            break

calculator()

<!---
degustaDD/degustaDD is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
