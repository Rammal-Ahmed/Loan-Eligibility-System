
" Loan Eligibility System "


#  Loan  Eligibility  System
     

print('"BANK ELIGIBILITY REPORT"')


# ---------------- NAME VALIDATION ----------------

customer = input("What is your Name Sir ? ")

while not customer.replace(" ", "").isalpha():
    print("Enter Correct Name please")
    customer = input("What is your Name Sir ? ")


# ---------------- AGE VALIDATION ----------------

age = int(input("What is your Age ? "))

while age < 1 or age > 95:
    print("Enter Correct Age please")
    age = int(input("What is your Age ? "))


# ---------------- OTHER INPUTS ----------------

monthly_income = int(input("Enter your Current Monthly Income = "))

account_balance = int(input("Enter your Current Account Balance = "))

loan_amount = int(input("Enter your Existing Pending Loan Amount = "))


# ---------------- ANNUAL INCOME ----------------

annual_income = monthly_income * 12

print("Annual Income =", annual_income)


# ---------------- LOAN ELIGIBILITY ----------------

eligible = True

if monthly_income < 30000:
    print("Sorry, your monthly income does not meet our criteria.")
    eligible = False

if age < 18:
    print("Sorry, your age must be at least 18.")
    eligible = False

if loan_amount >= 500000:
    print("Sorry, your loan amount exceeds our criteria.")
    eligible = False


# ---------------- FINAL RESULT ----------------

if eligible:
    print("Congratulations, you are eligible for our bank loan.")
     
"BANK ELIGIBILITY REPORT"
What is your Name Sir ? RJ
What is your Age ? 13
Enter your Current Monthly Income = 56000
Enter your Current Account Balance = 45600
Enter your Existing Pending Loan Amount = 23000
Annual Income = 672000
Sorry, your age must be at least 18.
