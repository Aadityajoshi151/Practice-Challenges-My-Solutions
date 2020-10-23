## 📦Challenge:
Write a function that returns True if the first string is the second string stretched, and False otherwise. A stretch is to repeat each character in a string the same number of times.
For more details of the challenge, [Click here][https://edabit.com/challenge/4Pe4nySfRnWPCjEwr]
## ✏️My Solution:
```
def is_stretched(s1, s2):
	return True if str(len(s1)/len(s2)).split(".")[1] == "0" else False
```
*It took me about an hour to figure out this one line code*

[https://edabit.com/challenge/4Pe4nySfRnWPCjEwr]: https://edabit.com/challenge/4Pe4nySfRnWPCjEwr