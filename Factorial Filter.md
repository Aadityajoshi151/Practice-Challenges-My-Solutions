## 📦Challenge:
Create a function that filters out factorials from a list. In other words return a list of numbers from the input list which are factorial of some other number.
For more details of the challenge, [Click here][https://edabit.com/challenge/QcswPnY2cAbrfwuWE]
## ✏️My Solution:
```
def filter_factorials(numbers):
	res = []
	for n in numbers:
		divisor=1
		if n==1: res.append(n)
		else:
			temp = n
			while(n>1):
				divisor+=1
				if n/divisor == 1: res.append(temp)
				else: n=n/divisor
	return res
```

[https://edabit.com/challenge/QcswPnY2cAbrfwuWE]: https://edabit.com/challenge/QcswPnY2cAbrfwuWE