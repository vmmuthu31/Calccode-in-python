# Calculator

def add(x,y):
    return x+y
def sub(x,y):
    return x-y
def mul(x,y):
    return x*y
def div(x,y):
    return x/y
def exp(x,y):
    return x**y
def reminder(x,y):
    return x%y
def floordiv(x,y):
    return x//y

print("This is the calculator")
print("Type 1 for Addition")
print("Type 2 for Subraction")
print("Type 3 for Multiplication")
print("Type 4 for Division")
print("Type 5 for exponential")
print("Type 6 for remainder")
print("Type 7 for floor division")

while True:
    choice=input("Enter your Choice(1/2/3/4/5/6/7): ")

    if choice in ('1','2','3','4','5','6','7'):
            number1=float(input("Enter the first number: "))
            number2=float(input("Enter the Second number: "))
            if choice == '1':
                print( number1,"+",number2,"=",add(number1,number2))
            elif choice == '2':
                print(number1, "-", number2, "=", sub(number1, number2))
            elif choice == '3':
                print(number1, "*", number2, "=", mul(number1, number2))
            elif choice == '4':
                print(number1, "/", number2, "=",div(number1, number2))
            elif choice == '5':
                print( number1,"**",number2,"=",exp(number1,number2))
            elif choice == '6':
                print(number1, '%', number2, "=", reminder(number1, number2))
            elif choice == '7':
                print(number1, "//", number2, "=", floordiv(number1, number2))
            next_calcultation=input("Let's Continue or not (Yes/No): ")
            if next_calcultation=="no":
                break
            else:
                    print("Invalid input")
