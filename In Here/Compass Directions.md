## 📦Challenge:
Create a function that takes in a starting direction and a sequence of left and right turns, and outputs the final direction faced.
For more details of the challenge, [Click here][https://edabit.com/challenge/6LAgr6EGHKoZWGhjd]

## ✏️My Solution:
```
def final_direction(initial, turns):
	direction_numbers = {"N":1,"E":2,"S":3,"W":4}
	initial = direction_numbers.get(initial)
	for i in turns:
		if i=="L": initial-=1
		else: initial+=1
	initial = abs(initial)
	while initial > 4:
		initial-4
	return list(direction_numbers.keys())[list(direction_numbers.values()).index(initial)]
```

[https://edabit.com/challenge/6LAgr6EGHKoZWGhjd]: https://edabit.com/challenge/6LAgr6EGHKoZWGhjd