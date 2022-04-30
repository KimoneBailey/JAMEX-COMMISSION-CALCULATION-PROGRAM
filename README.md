# JAMEX-COMMISSION-CALCULATION-PROGRAM
Programming Techniques -S2022 - Python Code 
# Author : Kimone Bailey
# Date Created : May 1 ,2022
# Course: ITT103
# Purpose : <The purpose of this program is to calculate the commission earned by sales persons at Jamex Limited.
# The commssion is calculated by the class and rate associated with the class selected>


print (' Welcome to JAMEX Limited Commission Calculation Program ')
# Welcome statement stating what the program does

print(' Insert 0 in class to quit program')
# The program will terminate when the user enters zero


while 1:
    
    # The program will run as long as the class entered is one or more
    
    sales_num = int(input(' Enter Sales Number : '))
    sales_person_class = int(input(' Enter Sales Person Class: '))
    sales_amt = int(input(' Enter Sales Amount: '))
    
    # The user is promted to enter their sales number which is the special employee identification number.The data type is defined as a interger.
    #The user is promted to enter their class whether it is class 1 , 2 or 3.The data type is integer. 
    # The user is promted to enter the sales amount, which is the amount of sales made for the particular period by the sales person.
    
    commission=0
    
    #The commission variable stores the result of the rate multiplied by the sales amount.
    
    rate=0
    
    #The rate is the standard value assigned based on the class the worker is listed under.
    
    if sales_person_class == 0:
        quit()
        break 

    #If the class entered by the user is 1 then the following if statement will be processed and so on for class 2 and 3.
    #When the sales amount is entered the program will check which condition in the statement will be executed
    #The condition will be executed and return the the commission of the sales person
    #If the condition is not met the error message will appear.
    
    elif sales_person_class == 1:
        if sales_amt <= 1000:
            rate=0.06
            commission = sales_amt*rate
            
        elif sales_amt > 1000 or sales_amt < 2000:
            rate=0.07
            commission = sales_amt*rate
            
        elif sales_amt >= 2000 :
             rate=0.1
             commission = sales_amt*rate
             
        else:
            print(' Error! Try Again')
            
    elif sales_person_class == 2:
        if sales_amt < 1000:
            rate=0.04
            commission = sales_amt*rate
            
        elif sales_amt >= 1000:
            rate=0.06
            commission = sales_amt*rate
            
        else:
            print(' Error! Try Again ')
            
    elif sales_person_class == 3:
        rate=0.045
        commission = sales_amt*rate
        
    else:
       print (' Error! Try Again')
       
       
    print (f' The Commission for Sales Person {sales_num} is :{commission}') 
    #This is the print statement displaying the commission for the mentioned sales person.
    
[Bailey.Kimone- PythonCode-ITT103-S2022.txt](https://github.com/KimoneBailey/JAMEX-COMMISSION-CALCULATION-PROGRAM/files/8597178/Bailey.Kimone-.PythonCode-ITT103-S2022.txt)
