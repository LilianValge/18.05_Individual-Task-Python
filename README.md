```py
# Create a program where the user can input deposits into a bank account. The program should use `if-else` statements, `input()`, `int()` and while True loop to keep track of deposits.

# Welcome the user to the bank
print("Welcome to the bank")

# Initialize balance = 0
total_balance = 0

# Ask the user if they want to make a deposit
while True:
    try:
        # Ask the user to input the amount of money they want to deposit.
        deposit = int(input("Please enter the amount of money you want to deposit: "))
        
        # Add the deposit amount to the total balance
        total_balance += deposit
        
        # Ask the user if they want to make another deposit or exit the bank.
        another_deposit = input("Would you like to make another deposit? (yes/no): ")
        
        # If they choose to make another deposit, repeat the process (while True).
        if another_deposit.lower() == "no":
            break
    except ValueError:
        print("Invalid input! Please enter a valid integer amount for the deposit.")

# Print the total amount deposited and exit the bank.
print("Total balance deposited:", total_balance)
```
