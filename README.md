month = 0
	totalPay = 0
	monthlyInterestRate = annualInterestRate / 12.0
	while month <12:
	    minPay = monthlyPaymentRate * balance
	    unpayBal = balance - minPay
	    totalPay += minPay
	    balance = unpayBal + (monthlyInterestRate * unpayBal)
	    month += 1
	    print('Month: ' + str(month))
	    print('Minimum monthly payment: ' + str(round(minPay,2)))
	    print('Remaining balance: ' + str(round(balance,2)))
	print('Total paid: ' + str(round(totalPay,2)))
	print(' Remaining balance: ' + str(round(balance,2)))

