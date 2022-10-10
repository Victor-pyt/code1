# code1
def welcome( ):
        print("Welcome, calculate away")
welcome( )
def calculate( ):
    operation = input('''Please choose the operation you want to carry out:
    1 for addition
    2 for subtraction
    3 for multiplication
    4 for division
    ''')
    number_1 = float(input('Enter your first number: '))
    number_2 = float(input('Enter your second number: '))
    
#To carry out addition function
    if operation == '1': 
        print("{} + {} = ".format(number_1, number_2))
        print(number_1 + number_2)
#To carry out multiplication function
    elif operation =='3':
        print("{} * {} = ".format(number_1, number_2))
        print(number_1 * number_2)
#To carry out division function
    elif operation == '4':
        print("{} / {} = ".format(number_1, number_2))
        print(number_1 / number_2)
# To carry out subtraction
    elif operation == '2':
        print("{} - {} = ".format(number_1, number_2))
        print(number_1 - number_2)
    else:
        print("invalid operator, kindly run the program again ")
    again( )
        
def again( ):
    calc_again = input('''To use calculator again type Y, to exit type N''')
    if calc_again.upper()=="Y":
        calculate ( )
    elif calc_again.upper()=="N":
        print("see you later when you need something to calculate")
    else:
        again( )
calculate()
