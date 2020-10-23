## 📦Challenge:
Given a start and an end being the initial and ending line of the sequence, you have to implement a function that returns the index of the given n, in a generated array containing the portion of the **Connell sequence**. If n is not in the array, you have to return a string "Not Found".
For more details of the challenge, [Click here][https://edabit.com/challenge/zM5ZTgCbk4hWsEBwQ]
## ✏️My Solution:
```
def connell_sequence(start, end, n):
	seq=[]
	for i in range(start,end+1):
		for j in range(i):
			seq.append((i*i)-(2*j))
	return sorted(seq).index(n) if n in seq else "Not Found"
```

[https://edabit.com/challenge/zM5ZTgCbk4hWsEBwQ]: https://edabit.com/challenge/zM5ZTgCbk4hWsEBwQ