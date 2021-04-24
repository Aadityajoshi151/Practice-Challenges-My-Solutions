## 📦Challenge:
Create a function that returns the victorious digits.
For more details of the challenge, [Click here][https://edabit.com/challenge/cGB2rkiLYC8jdWn8P]

## ✏️My Solution:
```
def vicdigit(num)
    num = list(str(num))
    ans = ""
    for i in range(0,len(num),2):
        try:
            if not num[i] == num[i+1]:
                ans+=max(num[i],num[i+1])
        except:
            ans+=num[i]
    return int(ans)
```

[https://edabit.com/challenge/cGB2rkiLYC8jdWn8P]: https://edabit.com/challenge/cGB2rkiLYC8jdWn8P