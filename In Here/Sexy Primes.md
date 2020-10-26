## 📦Challenge:
Sexy primes are primes that differ by 6.

Create a function that takes two numbers as argument, the set length n (2 for pairs, 3 for triplets), and the limit. Return a list of sorted tuples of sexy primes up to (but excluding) the limit.

For more details of the challenge, [Click here][https://edabit.com/challenge/GC7JWFhDdhyTsptZ8]
## ✏️My Solution:
```
def sexy_primes(n, limit):
	res = []
	def isprime(x):
		flag=0
		for i in range(2,x):
			if x%i==0:
				flag=1
				break
		return True if flag==0 else False
	for i in range(2,limit):
		if isprime(i):
			if isprime(i+6) and (i+6<limit):
				if n==3:
					if isprime(i+12) and (i+12<limit):
						temp = (i,i+6,i+12)
						res.append(temp)
				else:
					temp = (i,i+6)
					res.append(temp)
	return res
```

[https://edabit.com/challenge/GC7JWFhDdhyTsptZ8]: https://edabit.com/challenge/GC7JWFhDdhyTsptZ8