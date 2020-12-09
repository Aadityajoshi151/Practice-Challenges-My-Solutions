## 📦Challenge:
Create a function that, when given two positive integers a b, returns the string "a" if integer a took fewer steps to reach 1 than b when passed through the Collatz sequence, or "b" if integer b took fewer steps to reach 1 than a.
For more details of the challenge, [Click here][https://edabit.com/challenge/6JNHBeGxY8dhTaPhs]

## ✏️My Solution:
```
def collatz(a, b):
	def findsteps(x):
		steps = 0
		while(x!=1):
			if x%2==0:
				x=x/2
				steps+=1
			else:
				x = (x*3)+1
				steps+=1
		return steps
	return "a" if findsteps(a)<findsteps(b) else "b"
```

[https://edabit.com/challenge/6JNHBeGxY8dhTaPhs]: https://edabit.com/challenge/6JNHBeGxY8dhTaPhs