# prime-nunmber
This is a program for check a number is prime number or not... 

n = int(input('enter the number : '))
for i in range(2,n):
    
    if n%i==0:
        break 
    i  = i+1
    
if i==n:
    print('prime number')
else:
    print('number is not prime')

# and this above program i also do using funciton ...

def is_number_prime(n, i=2):

    if n <= 2:
        return True if n == 2 else False
    if n % i == 0:
        return False
    if i * i > n:
        return True

    return is_number_prime(n, i + 1)


if is_number_prime(11):
    print("Yes, given number is prime")
else:
    print("No, given number is not prime")

# Now this is a first n prime number list program in python

def number(x):
    i=1
    for i in range(1, x+1):
        c = 0
        for j in range(1, i+1):
            a = i % j
            if a == 0:
                c = c + 1

        if c == 2:
            print(i)
        else:
            k = i - 1

        i = i + 1
        
number(100)


# now if I want to print prime number using funciton and prime number between two given number 



def number(x,y):
    
    for i in range(x, y+1):
        c = 0
        for j in range(1, i+1):
            a = i % j
            if a == 0:
                c = c + 1

        if c == 2:
            print(i)
        else:
            k = i - 1

        i = i + 1
        
number(10,50)
