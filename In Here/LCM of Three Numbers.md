## 📦Challenge:
Create a function that takes an array of three numbers and returns the Least Common Multiple (LCM).
For more details of the challenge, [Click here][https://edabit.com/challenge/7kZhB4FpJfYHnQYBq]
## ✏️My Solution:
```
def lcm_three(num):
	num = sorted(num)
	maximum = num[-1]
	i=1
	while(True):
		lcm = maximum*i
		if lcm%num[0] == 0 and lcm%num[1] == 0: break
		else: i+=1
	return lcm
```

[https://edabit.com/challenge/7kZhB4FpJfYHnQYBq]: https://edabit.com/challenge/7kZhB4FpJfYHnQYBq