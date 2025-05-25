SEB - RECURSION

AIM:
To write a python program to find the result of a! - b! using recursion.

ALGORITHM:
STEP 1:Start the Program.
STEP 2:Define a recursive function factorial(n):
       If 𝑛 is 0 or 1, return 1.
       Otherwise, return 𝑛×factorial(n-1).
STEP 3:Compute 𝑎!and 𝑏! using the recursive function.
STEP 4:Subtract 𝑏!from 𝑎! to get the final result.
STEP 5:Return the computed difference.
STEP 6:End the program.

PROGRAM:

```
def factorial(n):
    if n==0:
        return 1
    return (n* factorial(n-1))
    
a=int(input())
b=int(input())
c=factorial(a)-factorial(b)
print(c)
```

OUTPUT:


![image](https://github.com/user-attachments/assets/4f7b2528-7e73-4ccc-a57a-5851da10815d)


RESULT:
Thus the python program to find the result of a! - b! using recursion is done successfully.
