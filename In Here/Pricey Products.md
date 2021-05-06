## 📦Challenge:
Return a list of the products with a minimum price of 500 in descending order.
For more details of the challenge, [Click here][https://edabit.com/challenge/SxevRSmRcshgwnAKp]

## ✏️My Solution:
```
def pricey_prod(d):
	def GetKey(val):
		for key, value in d.items():
			if val == value: return key
	prices = [d.get(i) for i in d]
	prices.sort(reverse=True)
	ans = [GetKey(i) for i in prices if i>=500]
	return ans
```

[https://edabit.com/challenge/SxevRSmRcshgwnAKp]: https://edabit.com/challenge/SxevRSmRcshgwnAKp