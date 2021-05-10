## 📦Challenge:
Write a function that returns the longest common ending between two strings.
For more details of the challenge, [Click here][https://edabit.com/challenge/SeShBxdG2rhGf4Y5L]

## ✏️My Solution:
```
def longest_common_ending(txt1, txt2):
	if len(txt1) == len(txt2):
		small = txt1
		large = txt2
	else:
		small = min(txt1,txt2,key = len)
		large = max(txt1,txt2,key = len)
	for i in range(len(small)-1):
		if small[i:] in large: return small[i:]
	return ""
```
Remark: Could have been done in lot less lines by using 'endswith()' method.

[https://edabit.com/challenge/SeShBxdG2rhGf4Y5L]: https://edabit.com/challenge/SeShBxdG2rhGf4Y5L