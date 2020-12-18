## 📦Challenge:
Create a function that takes a number n as input. If n is an interprime number, print the two consecutive primes between which it lies.

## ✏️My Solution:
```
n = input("Please Enter The Number\n")
def isprime(x):
    flag = 0
    for i in range(2,x):
        if x%i==0:
            flag=1
            break
    return True if flag == 0 else False
if not isprime(n):
    step = 1
    while(True):
        if isprime(n-step) and isprime(n+step):
            print(n-step)
            print(n+step)
            break
        else:
            step+=1
else: print("Already A Prime Number")
```
