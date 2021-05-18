## 📦Challenge:
Given a positive integer n, implement a function that determines its a super-d number or not.
For more details of the challenge, [Click here][https://edabit.com/challenge/KSiC4iNjDHFiGS5oh]

## ✏️My Solution:
```
def is_super_d(n):
	ans = ""
	for i in range(2,10):
		temp = str(i * (n**i))
		if str(i)*i in temp:
			ans = "Super-"+str(i)+" Number"
			break
	return "Normal Number" if not ans else ans
```

[https://edabit.com/challenge/KSiC4iNjDHFiGS5oh]: https://edabit.com/challenge/KSiC4iNjDHFiGS5oh