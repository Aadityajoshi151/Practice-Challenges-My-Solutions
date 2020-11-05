## 📦Challenge:
Create a function that takes the side n of the game screen and returns the number of times the snake can eat before it runs out of space in the game screen.

For more details of the challenge, [Click here][https://edabit.com/challenge/Y5Ji2HDnQTX7MxeHt]
## ✏️My Solution:
```
def snakefill(n):
	snake = 1
	ans = 0
	while(True):
		snake = snake*2
		if snake <= n*n: ans+=1
		else: break
	return ans
```

[https://edabit.com/challenge/Y5Ji2HDnQTX7MxeHt]: https://edabit.com/challenge/Y5Ji2HDnQTX7MxeHt