## 📦Challenge:
The weight of a word can be calculated by summing the Unicode code point for each character in the word, excluding any punctuation.

Write a function that takes a sentence as a string, returning True if all word weights increase for each word in the sentence, and False if any word weight decreases or remains the same.
For more details of the challenge, [Click here][https://edabit.com/challenge/f6X7pa38iQyoytJgr]
## ✏️My Solution:
```
def increasing_word_weights(sentence):
	res = []
	for i in sentence.split(): res.append(sum(ord(j) for j in i if j.isalpha()))
	return False if res.count(res[0]) == len(res) else res==sorted(res)
```

[https://edabit.com/challenge/f6X7pa38iQyoytJgr]: https://edabit.com/challenge/f6X7pa38iQyoytJgr