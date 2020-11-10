## 📦Challenge:
Write a function that returns True if the word is balanced, and False if it's not.

For more details of the challenge, [Click here][https://edabit.com/challenge/55f9SDtxuLgSaJdcK]
## ✏️My Solution:
```
def balanced_word(word):
	lhssum,rhssum = 0,0
	lhs = word[:len(word)//2]
	if len(word)%2==0: rhs = word[(len(word)//2):]
	else: rhs = word[(len(word)//2)+1:]
	for i in range(len(rhs)):
		lhssum+=ord(lhs[i])-96
		rhssum+=ord(rhs[i])-96
	return lhssum == rhssum	
```

[https://edabit.com/challenge/55f9SDtxuLgSaJdcK]: https://edabit.com/challenge/55f9SDtxuLgSaJdcK