# SIP-CALCULATOR
amount = float(input("Enter the monthly SIP amount: "))

yearlyRate = float(input("Enter the yearly rate of return: "))

years = int(input("Enter the number of years: "))

monthlyRate = yearlyRate/12/100

months = years * 12

futureValue = amount * ((((1 + monthlyRate)**(months))-1) * (1 + monthlyRate))/monthlyRate

futureValue = round(futureValue)

print("The expected amount you will get is:",futureValue)
