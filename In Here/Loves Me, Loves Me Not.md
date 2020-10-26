## 📦Challenge:
"Loves me, loves me not" is a traditional game in which a person plucks off all the petals of a flower one by one, saying the phrase "Loves me" and "Loves me not" when determining whether the one that they love, loves them back.

Given a number of petals, return a string which repeats the phrases "Loves me" and "Loves me not" for every alternating petal, and return the last phrase in **all caps**. Remember to put a comma and space between phrases.

For more details of the challenge, [Click here][https://edabit.com/challenge/6pEGXsuCAxbWTRkgc]
## ✏️My Solution:
```
def loves_me(n):
	ans = ["Loves me" if i%2!=0 else "Loves me not" for i in range(1,n+1)]
	ans[-1] = ans[-1].upper()
	return ", ".join(i for i in ans)
```

[https://edabit.com/challenge/6pEGXsuCAxbWTRkgc]: https://edabit.com/challenge/6pEGXsuCAxbWTRkgc