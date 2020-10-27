## 📦Challenge:
Create a function that identifies the very first item that has recurred in the string argument passed. It returns the identified item with the index where it first appeared and the very next index where it resurfaced ⁠— entirely as an dictionary; or as an empty dictionary if the argument is either None, an empty string, or no recurring item exists.

For more details of the challenge, [Click here][https://edabit.com/challenge/9jhTpvYgTCJyD46hA]
## ✏️My Solution:
```
def recur_index(txt):
	if txt == "" or txt == None: return {}
	else:
		counts = []
		for i in range(1,len(txt)):
			if txt[i] in txt[:i]:
				letter = txt[i]
				break
		try:
			for i in range(len(txt)):
				if txt[i] == letter:
					counts.append(i)
					if len(counts) == 2: break
			return {letter:counts} 
		except:
			return {}
```

[https://edabit.com/challenge/9jhTpvYgTCJyD46hA]: https://edabit.com/challenge/9jhTpvYgTCJyD46hA