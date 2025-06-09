# Day-2-Tip-Calculator
A simple Python script that calculates how much each person should pay when splitting a bill, including the tip.  

How It Works  
The user provides:  
The total bill amount  
The desired tip percentage (e.g., 10%, 12%, or 15%)  
The number of people sharing the bill  
The program calculates the total bill (including the tip), splits it evenly, and displays the amount each person should pay, rounded to 2 decimal places.    

#code  

print("Welcome to the tip calculator!")
bill = float(input("What was the total bill? $"))
tip = int(input("What percentage tip would you like to give? 10 12 15 "))
people = int(input("How many people to split the bill? "))
tip_as_percent = tip / 100
total_tip_amount = bill * tip_as_percent
total_bill = bill + total_tip_amount
bill_per_person = total_bill / people
final_amount = round(bill_per_person, 2)
print(f" Each person should pay: ${final_amount}")
