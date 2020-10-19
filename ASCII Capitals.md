## 📦Challenge:
Given a sentence, return the sentence with one change:
For a word, if the sum of its letter's char codes is above the global average sum of char codes (i.e if the sum of char codes for a word is 205) and on average, a word in the sentence has a char code sum of 189, capitalise the word.

For more details of the challenge, [Click here][https://edabit.com/challenge/Q8XSxTfzP3HLS57h5]
## ✏️My Solution:
```
def average_ascii(txt):
	globe = 0
	for i in txt:
		if i.isalpha(): globe+=ord(i)
	txt = txt.split()
	globe=round(globe/len(txt),2)
	for i in range(len(txt)):
		if globe< sum(ord(j) for j in txt[i]): txt[i] = txt[i].upper()
	return " ".join(i for i in txt)
```

[https://edabit.com/challenge/Q8XSxTfzP3HLS57h5]: https://edabit.com/challenge/Q8XSxTfzP3HLS57h5