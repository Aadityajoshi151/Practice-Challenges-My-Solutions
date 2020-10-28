## 📦Challenge:
Write a function that selects all words that have all the same vowels (in any order and/or number) as the first word, including the first word.

For more details of the challenge, [Click here][https://edabit.com/challenge/uwFHSRewNpmBNvbME]
## ✏️My Solution:
```
def same_vowel_group(w):
	vowelpresent = []
	vowels = ["a","e","i","o","u"]
	res = []
	for i in w[0]:
		if i == "a" or i == "e" or i == "i" or i == "o" or i == "u":
			if i not in vowelpresent: vowelpresent.append(i)
			if i in vowels: vowels.remove(i)
	for i in w:
		flag=0
		for j in vowelpresent:
			if j not in i:
				flag=1
				break
		for k in i:
			if k in vowels:
				flag=1
				break
		if flag==0: res.append(i)
	return res
```
*It could have been done in much less lines of code.*

[https://edabit.com/challenge/uwFHSRewNpmBNvbME]: https://edabit.com/challenge/uwFHSRewNpmBNvbME