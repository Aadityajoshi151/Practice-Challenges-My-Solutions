## 📦Challenge:
Create a function which takes in an encoded string and returns a dictionary.

For more details of the challenge, [Click here][https://edabit.com/challenge/7vN8ZRw43yuWNoy3Y]
## ✏️My Solution:
```
def parse_code(txt):
	fname , lname = "",""
	for i in txt:
		if i.isalpha(): fname +=i
		else: break
	txt = txt.replace(fname,"")
	txt = txt.lstrip("0")
	for i in txt:
		if i.isalpha(): lname +=i
		else: break
	txt = txt.replace(lname,"")
	txt = txt.lstrip("0")
	return {"first_name": fname,
	"last_name": lname,
	"id": txt
	}
```

[https://edabit.com/challenge/7vN8ZRw43yuWNoy3Y]: https://edabit.com/challenge/7vN8ZRw43yuWNoy3Y