## 📦Challenge:
A number is Zygodrome if can be partitioned into clusters of repeating digits with a length equals or greater than two (as to say that repeating digits need to be placed as an adjacent pair or a greater group, and that no single digits are allowed).

Given a non-negative integer num, implement a function that returns True if num is a Zygodrome number, or False otherwise

For more details of the challenge, [Click here][https://edabit.com/challenge/xFme9FBuvHLveh5nE]
## ✏️My Solution:
```
def is_zygodrome(num):
	num = str(num)
	myset = set(num)
	flag=0
	for i in myset:
		if num.count(i)<=1:
			flag=1
			break
	if flag==0:
		for i in myset:
			if num[num.find(i)+1] != i:
				flag = 1
				break
		return False if flag==1 else True
	else:
		return False
```

[https://edabit.com/challenge/xFme9FBuvHLveh5nE]: https://edabit.com/challenge/xFme9FBuvHLveh5nE