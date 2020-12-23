## 📦Challenge:
Given two integers create a function that counts the number of primes between the two given integers.

For more details of the challenge, [Click here][https://edabit.com/challenge/6QYwhZstMuHYtZRbT]

## ✏️My Solution:
```
def prime_count(a, b):
	count = 0
	if a==1: a=a+1
	for i in range(a,b):
		flag = 0
		for j in range(2,i):
			if i%j == 0:
			flag=1
			break
		if flag == 0: count+=1
return count
```

[https://edabit.com/challenge/6QYwhZstMuHYtZRbT]: https://edabit.com/challenge/6QYwhZstMuHYtZRbT