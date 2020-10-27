## 📦Challenge:
Write a function that returns all sets of three elements that sum to 0, from a list.

For more details of the challenge, [Click here][https://edabit.com/challenge/gbybFzt2tLa5zfpHc]
## ✏️My Solution:
```
from itertools import combinations
def three_sum(lst):
	res = []
	for i in list(combinations(lst,3)):
		if sum(i) == 0 and list(i) not in res: res.append(list(i))
	return res
```

[https://edabit.com/challenge/gbybFzt2tLa5zfpHc]: https://edabit.com/challenge/gbybFzt2tLa5zfpHc