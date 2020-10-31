## 📦Challenge:
Given a sentence with numbers representing a word's location embedded within each word, return the sorted sentence.

For more details of the challenge, [Click here][https://edabit.com/challenge/af6XnEimLZTcwxJTP]
## ✏️My Solution:
```
def rearrange(sentence):
	sentence = sentence.split()
	res = []
	for i in range(1,len(sentence)+1):
		for j in sentence:
			if str(i) in j: res.append(j.replace(str(i),""))
	return " ".join(i for i in res)
```

[https://edabit.com/challenge/af6XnEimLZTcwxJTP]: https://edabit.com/challenge/af6XnEimLZTcwxJTP