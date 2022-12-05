# SIP_CALCULATOR
# Mutual Funds SIP Calculator Using Python
###### SIP stands for 'Systematic Investment Plan' which allows you to invest small amounts in mutual funds at regular intervals.

Mathematical formula to calculate SIP:

fV= mA * ((((1 + mR)**(m))-1)*(1 + mR))/mR

***where,fV = future value,
         mA = monthly SIP amount, 
         mR = monthly rate of return, 
         m  = number of months. 
         yR = yearly rate, 
         Y  = number of years***
         
mA = float(input("Enter the monthly SIP amount: "))
yR = float(input("Enter the yearly rate of return: "))
Y = int(input("Enter the number of years: "))

mR = yR/12/100
m = Y * 12

fV = mA * ((((1 + mR)**(m))-1) * (1 + mR))/mR
fV = round(fV)
print("The expected amount you will get is:",fV)
