# 19CS301-Module7
EX: 7.1 RECURSION
### Aim: To Write a Python Program to find the sum of all digits in a number using recursion
### Algorithm:
STEP 1: Start.

STEP 2: Define a function.

STEP 3: Create a base case for termination of the function. STEP 4: Create a recursive case to calculate the result.

STEP 5: Print the result. STEP 6: Stop.

### Program:
```
def sum_digit(n):
       if n<=0:
            return 0
       else:
            return n%10+sum_digit(n//10)
n = int(input())
sum = sum_digit(n)
print(sum)
```
### Output:
![image](https://github.com/user-attachments/assets/50acc657-266e-46e6-ab17-10358494e26c)

### Result: Thus, the given program is implemented and executed successfully .
 

EX: 7.2 TYPES OF RECURSIONS
### Aim: To Write a Python Program to display first n natural numbers in reverse order using tail recursion.

### Algorithm:
Step1:Get input from the user.
Step2:Define a function reverse_natural_numbers(n, current).
Step3:Base Case: If current is zero, stop the recursion.
Step4:Print current and make a recursive call by decrementing current.
Step5:Call the function with n as the initial value of current.
Step6:Terminate the program.


### Program:
```
def fun(n):
    if n<1:
        return
    else:
        print(n,end=" ")
        return(fun(n-1))
n=int(input())
fun(n)
```
### Output:
![image](https://github.com/user-attachments/assets/983fc9e6-177b-4bb5-9d0c-f64d2fb1fb23)

###Result: Thus, the given program is implemented and executed successfully.


EX: 7.3 TAYLOR SERIES

###Aim: To python program to evaluate the series using recursion by collecting the x and n values from the user.
### ALGORITHM:
Step1:Read values x and n from the user.
Step2:Define Recursive Function: fun(x, n)
Step3:Base Case: If n == 0, return 1 (since the series starts from 1).
Step4:Recursive Case: Compute (2^n) * (x^n) + fun(x, n-1), recursively calling the function with n-1.
Step5:Call the function and print the result.
Step6:Terminate the program.

### Program:
```
def fun(x,n):
    if(n==0):
        return 1 
    else:
        return ((2**n)*(x**n)+fun(x,n-1))
x=int(input())
n=int(input())
print(fun(x,n))

```
### Output:
![image](https://github.com/user-attachments/assets/31f3f559-0f21-4bdb-b89f-ecb1ca57083e)

### Result: Thus, the given program is implemented and executed successfully .



EX: 7.4 Solve by recursion relation

### Aim: To Write a Python Program to to count the consonants in a string using recursion.

### Algorithm:
STEP 1: Start the program.
STEP 2: Read a string from the user.
STEP 3:Define Recursive Function: count_consonants(s, index)
STEP 4:Base Case: If index reaches the end of the string, return 0.
STEP 5:Check if s[index] is a consonant (i.e., an alphabet character that is not a vowel).
STEP 6:If it's a consonant, add 1 to the recursive call for the next index.
STEP 7:Otherwise, proceed to the next index without adding 1.
STEP 8:Start the recursion from index 0 and print the result.
STEP 9:Terminate the program.

### Program:
```
def consonant(c):
    c=c.upper()
    return (not(c=='A' or c=='E' or c=='I' or c=='O' or c=='U'))
def total(string,n):
    if n==1:
        return consonant(string[0])
    return total(string,n-1)+consonant(string[n-1])
string=input()
print(total(string,len(string)))

```
### Output:
![image](https://github.com/user-attachments/assets/23c10981-ac19-43f2-ada4-da4553fd105e)


### Result: Thus, the given program is implemented and executed successfully .
 

