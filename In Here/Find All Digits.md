## 📦Challenge:
Taking each four digit number of a list in turn, return the number that you are on when all of the digits 0-9 have been discovered.

For more details of the challenge, [Click here][https://edabit.com/challenge/rPnq2ugsM7zsWr3Pf]

## ✏️My Solution:
```
def find_all_digits(nums):
	digits = [0,1,2,3,4,5,6,7,8,9]
	flag=True
	for i in nums:
		for j in str(i):
			if int(j) in digits: digits.remove(int(j))
			if not digits:
				return i
	return "Missing digits!"
```

[https://edabit.com/challenge/rPnq2ugsM7zsWr3Pf]: https://edabit.com/challenge/rPnq2ugsM7zsWr3Pf