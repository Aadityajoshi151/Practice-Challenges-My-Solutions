## 📦Challenge:
Return the number of minutes it will take to get your license.
For more details of the challenge, [Click here][https://edabit.com/challenge/n53MYmznGpPLxM4K2]

## ✏️My Solution:
```
def license(me, agents, others):
	total = sorted(others.split(" ")+[me])
	for i in range(0,len(total)):
		if total[i] == me:
			ans = ((i+1)*20)-20*(agents-1)
			if ans <20: return 20
			else: return ans
```

[https://edabit.com/challenge/n53MYmznGpPLxM4K2]: https://edabit.com/challenge/n53MYmznGpPLxM4K2