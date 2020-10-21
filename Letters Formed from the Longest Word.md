## 📦Challenge:
Write a function that returns True if all the strings in a list can be formed by using only the characters from the longest string.
For more details of the challenge, [Click here][https://edabit.com/challenge/zeHgBRuYyxp9TFry4]
## ✏️My Solution:
```
from itertools import permutations
def can_form(lst):
	res = max(lst,key = len)
	lst.remove(res)
	flag = 0
	for i in lst:
		temp = list(permutations(res,len(i)))
		for j in range(len(temp)): temp[j] = "".join(k for k in temp[j])
		if i not in temp:
			flag=1
			break
	return True if flag==0 else False
```

[https://edabit.com/challenge/zeHgBRuYyxp9TFry4]: https://edabit.com/challenge/zeHgBRuYyxp9TFry4