# Module 3 Challenge

## Customer Banking

This is an application to simulate customer banking.

### Requirements and Answers

#### Create the Savings Account Function

* The Account class from the Accounts.py file is imported.

``` python
from Account import Account
```

* In the create_savings_account function, an instance of the Account class is created and the balance and interest parameters are passed to the Account class.

``` python
account = Account(balance, interest_rate)
```

* The interest earned is calculated and assigned to a variable.

``` python
interest_earned = balance * (interest_rate/100 * months/12)
```

* The savings account balance is updated by adding the interest earned to the balance and assigned to a variable.

``` python
updated_balance = balance + interest_earned
```

* The updated balance is passed to the set balance method using the instance of the Account class.

``` python
account.set_balance(updated_balance)
```

* The interest earned is passed to the set balance method using the instance of the Account class.

``` python
account.set_interest(interest_earned)
```

* The updated balance and interest earned are returned by the function.

``` python
return updated_balance, interest_earned
```

#### Create the CD Account Function

* The Account class from the Accounts.py file is imported.

``` python
from Account import Account
```

* In the create_cd_account function, an instance of the Account class is created and the balance and interest parameters are passed to the Account class.

``` python
cd_account = Account(balance, interest_rate)
```

* The interest earned is calculated and assigned to a variable.

``` python
interest_earned = balance * (interest_rate/100 * months/12)
```

* The CD account balance is updated by adding the interest earned to the balance and assigned to a variable.

``` python
updated_balance = balance + interest_earned
```

* The updated balance is passed to the set balance method using the instance of the Account class.

``` python
cd_account.set_balance(updated_balance)
```

* The interest earned is passed to the set balance method using the instance of the Account class.

``` python
cd_account.set_interest(interest_earned)
```

* The updated balance and interest earned are returned by the function.

``` python
return updated_balance, interest_earned
```

#### Create the Main Function

* The user is prompted to set the savings balance, interest rate, and months for the savings account. 

``` python
savings_balance = float(input("Enter the Savings Account Balance: "))
savings_interest = float(input("Enter the Savings Account Interest Rate: "))
savings_maturity = int(input("Enter the Savings Account Months: ")) 
```

* Code is written to print out the interest earned and updated savings account balance with interest earned for the given months. The values are formatted to two decimal places and thousandths.

``` python
print(f"After {savings_maturity} months, the interest earned is ${interest_earned:.2f} bringing the savings balance to ${updated_savings_balance:.2f}")
```

* The user is prompted to set the savings balance, interest rate, and months for the CD account.

``` python
cd_balance = float(input("Enter the CD Account Balance: "))
cd_interest = float(input("Enter the CD Account Interest Rate: "))
cd_maturity = int(input("Enter the CD Account Months: "))
```

* Code is written to print out the interest earned and updated CD account balance with interest earned for the given months. The values are formatted to two decimal places and thousandths.

``` python
print(f"After {cd_maturity} months, the interest earned is ${interest_earned:.2f} bringing the cd balance to ${updated_cd_balance:.2f}")
```

* The main function is called to run the program.

``` python
main()
```
