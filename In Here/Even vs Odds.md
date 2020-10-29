## 📦Challenge:
Odd numbers like to hangout with odd numbers. Even numbers like to hangout with even numbers.

Given a list, calculate the number of liked spots.

For more details of the challenge, [Click here][https://edabit.com/challenge/4gDNqQB355FFGFFWN]
## ✏️My Solution:
```
def available_spots(lst, num):
	res = 0
	for i in range(len(lst)-1):
		if num%2==0:
			if lst[i]%2==0 or (lst[i+1])%2==0: res+=1
		else:
			if lst[i]%2!=0 or (lst[i+1])%2!=0: res+=1
	return res
```

[https://edabit.com/challenge/4gDNqQB355FFGFFWN]: https://edabit.com/challenge/4gDNqQB355FFGFFWN