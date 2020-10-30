## 📦Challenge:
Create two functions that take an integer as an argument and:

1. Return its additive persistence.
2. Return its multiplicative persistence.

For more details of the challenge, [Click here][https://edabit.com/challenge/5ou6SKDtFRZugbpda]
## ✏️My Solution:
```
def additive_persistence(n):
	count = 0
	while n>=10:
		count+=1
		n = sum(int(i) for i in str(n))
	return count
def multiplicative_persistence(n):
	count = 0
	while(n>10):
		temp = 1
		count+=1
		for i in str(n):
			temp = temp*int(i)
		n = temp
	return count
```

[https://edabit.com/challenge/5ou6SKDtFRZugbpda]: https://edabit.com/challenge/5ou6SKDtFRZugbpda