## 📦Challenge:
A positive integer is a Modest number, accordingly to the following algorithm:
- Divide the number into two left and right partitions.
- For each combination of left and right parts, you have to check if a condition is true: the remainder of the number divided by the right part is equal to the left part.
- If at least a combination of two parts satisfies the above condition, the number is Modest, otherwise, it's not.

Given an integer, implement a function that returns True if it is a Modest number, or False if it's not.

For more details of the challenge, [Click here][https://edabit.com/challenge/5XNKfyxBosjSXCWLn]
## ✏️My Solution:
```
def is_modest(num):
	flag = False
	if num<10:
		return False
	else:
		for i in range(1,len(str(num))):
			try:
				if num%int(str(num)[i:].lstrip("0") or "0") == int(str(num)[:i].lstrip("0")):
					flag = True
					break
			except:
				flag = False
	return flag
```

[https://edabit.com/challenge/5XNKfyxBosjSXCWLn]: https://edabit.com/challenge/5XNKfyxBosjSXCWLn