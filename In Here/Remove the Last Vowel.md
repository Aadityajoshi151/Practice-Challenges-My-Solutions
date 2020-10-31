## 📦Challenge:
Write a function that removes the last vowel in each word in a sentence.

For more details of the challenge, [Click here][https://edabit.com/challenge/sG3RY2QQ2qtarAGQD]
## ✏️My Solution:
```
def remove_last_vowel(txt):
	vowels = "aeiou"
	txt = txt.split()
	for i in range(len(txt)):
		temp = list(txt[i][::-1])
		for j in temp:
			if j.lower() in vowels:
				temp.remove(j)
				break
		txt[i] = "".join(j for j in temp[::-1]) 
	return " ".join(i for i in txt)
```

[https://edabit.com/challenge/sG3RY2QQ2qtarAGQD]: https://edabit.com/challenge/sG3RY2QQ2qtarAGQD