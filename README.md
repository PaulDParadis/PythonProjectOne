# PythonProjectOne
A silly little arithmetic calculator as a milestone marker in my transition to writing programs.
def addition():
    FirstNum = input("First number: ")
    SecNum = input("Second number: ")
    sum = int(FirstNum) + int(SecNum)
    print(sum)

def subtraction():
    FirstNum = input("First number: ")
    SecNum = input("Second number: ")
    diff = int(FirstNum) - int(SecNum)
    print(diff)
    
def multiplication():
    FirstNum = input("First number: ")
    SecNum = input("Second number: ")
    product = int(FirstNum) * int(SecNum)
    print(product)
    
def division():
    FirstNum = input("First number: ")
    SecNum = input("Second number: ")
    try:
        quotient = int(FirstNum) / int(SecNum)
    except ZeroDivisionError:
        print("Division by zero is illegal!!!")
    else:
        print(quotient)
 
 def ArithType():
     MathChoice = input("addition, subtraction, multiplication, division: ")
     if MathChoice == 'addition':
         addition()
     if MathChoice == 'subtraction':
         subtraction()
     if MathChoice == 'multiplication':
         multiplication()
     if MathChoice == 'division':
         division()

Fname = input("Please type your first name: ")
Lname = input("Please type your last name: ")
FullName = Fname+' '+Lname

print("Welcome, "+FullName+" to the arithmetic machine!")
print("Let's have some fun with elementary mathematics!")

ArithType()
while True:
    choice = input("Try again. 'yes' or 'no': ")
    if choice == 'yes':
        ArithType()
    elif choice == 'no':
        print("Thanks, "+FullName+", hope this experience added up to a great time!")
        break
         

         
         
         
         
         
         
         
         
         
         
         
         
