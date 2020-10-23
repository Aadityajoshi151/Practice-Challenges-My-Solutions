## 📦Challenge:
Write a function that returns True if you can use the letters of the first string to create the second string. Letters are case sensitive.
For more details of the challenge, [Click here][https://edabit.com/challenge/EHzL3v25wYp7E4AFC]
## ✏️My Solution:
```
from itertools import permutations
def can_build(s1, s2):
	flag = False
	if s2 == "":
		return True
	elif s1 == "":
		return False
	else:
		permut = permutations(s1,len(s2))
		for i in list(permut):
			if "".join(j for j in i) == s2:
				flag=True
				break
		return flag
```
*Permutations were not necessary. Simple count method would have sufficed.*

[https://edabit.com/challenge/EHzL3v25wYp7E4AFC]: https://edabit.com/challenge/EHzL3v25wYp7E4AFC