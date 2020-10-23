## 📦Challenge:
You will be given a list of string "east" formatted differently every time. Create a function that returns "west" wherever there is "east". Format the string according to the input.
For more details of the challenge, [Click here][https://edabit.com/challenge/39utPCHvtWqt5vaz9]
## ✏️My Solution:
```
def direction(lst):
	for i in range(len(lst)):
		lst[i] = lst[i].replace("e","w")
		lst[i] = lst[i].replace("E","W")
		lst[i] = lst[i].replace("a","e")
		lst[i] = lst[i].replace("A","E")
	return lst
```

[https://edabit.com/challenge/39utPCHvtWqt5vaz9]: https://edabit.com/challenge/39utPCHvtWqt5vaz9