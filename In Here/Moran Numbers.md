## 📦Challenge:
Create a function that takes a number and returns "M" if the number is a Moran number, "H" if it is a (non-Moran) Harshad number, or "Neither".

For more details of the challenge, [Click here][https://edabit.com/challenge/YTf8DZbTkzJ3kizNa]

## ✏️My Solution:
```
def isprime(x):
	flag=True
	for i in range(2,x):
		if x%i==0:
			flag=False
			break
	return True if flag else False
	
def moran(n):
	if n % sum(int(i) for i in str(n)) == 0:
		if isprime(int(n / sum(int(i) for i in str(n)))):
			return "M"
		else: 
			return "H"
	return "Neither"
```

[https://edabit.com/challenge/YTf8DZbTkzJ3kizNa]: https://edabit.com/challenge/YTf8DZbTkzJ3kizNa