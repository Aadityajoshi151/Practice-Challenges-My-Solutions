## 📦Challenge:
For a list of ranges, find the maximum range that is contained in all the ranges. If there is no such range, return "No overlapping".
For more details of the challenge, [Click here][https://edabit.com/challenge/BbBwirMcezbqa2Adw]
## ✏️My Solution:
```
def overlapping(lst):
	minimum,maximum = [],[]
	for i in lst:
		minimum.append(i[0])
		maximum.append(i[1])
	if max(minimum) > min(maximum):
		return "No overlapping"
	else:
		return (max(minimum),min(maximum))
```

[https://edabit.com/challenge/BbBwirMcezbqa2Adw]: https://edabit.com/challenge/BbBwirMcezbqa2Adw