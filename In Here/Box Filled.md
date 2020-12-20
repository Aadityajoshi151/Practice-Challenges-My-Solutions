## 📦Challenge:
Create a function that checks if the box is completely filled with the asterisk symbol *

For more details of the challenge, [Click here][https://edabit.com/challenge/wZojj7RuwnNDL4Seh]

## ✏️My Solution:
```
def completely_filled(lst):
	if len(lst[0])<=2: return True
	else:
		flag=0
		for i in range(1,len(lst)-1):
			if lst[i].count("*") != len(lst[0])-2:
				flag = 1
				break
		return True if flag == 0 else False
```

[https://edabit.com/challenge/wZojj7RuwnNDL4Seh]: https://edabit.com/challenge/wZojj7RuwnNDL4Seh