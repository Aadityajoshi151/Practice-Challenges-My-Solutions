## 📦Challenge:
In this challenge, you have to verify if a number is exactly divisible by a combination of its digits. There are three possible conditions to test:

- The given number is exactly divisible by each of its digits **excluding the zeros**.
- The given number is exactly divisible by the sum of its digits.
- The given number is exactly divisible by the product of its digits.

Given an integer `n`, implement a function that returns:

- If every test is true, a string `"Perfect"`.
- If some test is true, the number of true tests (`1` or `2`).
- If every test is false, a string `"Indivisible"`.
For more details of the challenge, [Click here][https://edabit.com/challenge/NWR5BK4BYqDkumNiB]
## ✏️My Solution:
```
def digital_division(n):
	res = 0
	flag=0
	product = 1
	for i in str(n):
		if int(i)!=0:
			if n%int(i) != 0:
				flag=1
				break
	if flag == 0: res+=1
	if n%sum(int(j) for j in str(n)) == 0: res+=1
	if str(n).count("0") == 0:
		for i in str(n):
			product*=int(i)
		if n%product == 0: res+=1

	if res == 3: return "Perfect"
	elif res == 0: return "Indivisible"
	else: return res
```

[https://edabit.com/challenge/NWR5BK4BYqDkumNiB]: https://edabit.com/challenge/NWR5BK4BYqDkumNiB