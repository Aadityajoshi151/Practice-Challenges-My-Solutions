## 📦Challenge:
A number has a breakpoint if it can be split in a way where the digits on the left side and the digits on the right side sum to the same number.

For instance, the number 35190 can be sliced between the digits 351 and 90, since 3 + 5 + 1 = 9 and 9 + 0 = 9. On the other hand, the number 555 does not have a breakpoint (you must split between digits).

Create a function that returns True if a number has a breakpoint, and False otherwise.
For more details of the challenge, [Click here][https://edabit.com/challenge/oCe79PHB7yoqkbNYb]
## ✏️My Solution:
```
def break_point(num):
	num = list(str(num))
	lhs = 0
	flag = False
	for i in range(len(num)):
		rhs = 0
		lhs += int(num[i])
		for j in range(i+1,len(num)): rhs+= int(num[j])
		if lhs == rhs:
			flag = True
			break
	return flag
```

[https://edabit.com/challenge/oCe79PHB7yoqkbNYb]: https://edabit.com/challenge/oCe79PHB7yoqkbNYb