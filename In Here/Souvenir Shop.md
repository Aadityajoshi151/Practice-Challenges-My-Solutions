## 📦Challenge:
Given a list of prices of things in the store and the amount of money you have, return the maximum number of items you could possibly buy.
For more details of the challenge, [Click here][https://edabit.com/challenge/yCGJEcij4LaXLcKXE]

## ✏️My Solution:
```
def maximum_items(prices, budget):
	ans=0
	prices = sorted[int(i.replace("$","")) for i in prices]
	budget = int(budget.replace("$",""))
	if all(i > budget for i in prices): return "Not enough funds!"
	for i in prices:
		if not budget == 0:
			if i<=budget:
				budget = budget-i
				ans+=1
	return ans
```

[https://edabit.com/challenge/yCGJEcij4LaXLcKXE]: https://edabit.com/challenge/yCGJEcij4LaXLcKXE