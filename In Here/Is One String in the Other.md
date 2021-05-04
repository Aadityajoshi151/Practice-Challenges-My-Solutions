## 📦Challenge:
Create a function that takes two strings and returns True if either of the strings appears at the very end of the other string. Return False otherwise.
For more details of the challenge, [Click here][https://edabit.com/challenge/rShXJNT2WQQiSiRx6]

## ✏️My Solution:
```
def overlap(str1, str2):
	str1 = str1.lower()
	str2 = str2.lower()
	flag=True
	if str1[-1] == "*" or str2[-1] == "*" or str1[0] == "*" or str2[0] == "*":
		ans = True
		flag=False
	else:
		if len(str1) < len(str2):
			if str2.endswith(str1):
				ans = True
				flag = False
		else:
			if str1.endswith(str2):
				ans = True
				flag=False
	if flag: return False
	else: return ans
```

[https://edabit.com/challenge/rShXJNT2WQQiSiRx6]: https://edabit.com/challenge/rShXJNT2WQQiSiRx6