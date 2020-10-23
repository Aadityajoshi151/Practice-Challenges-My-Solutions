## 📦Challenge:
Create a function that takes in two words as input and returns a list of three elements, in the following order:
1. Shared letters between two words
1. Letters unique to word 1
1. Letters unique to word 2

Each element should have unique letters, and have each letter be alphabetically sorted.
For more details of the challenge, [Click here][https://edabit.com/challenge/GaJkMnuHLuPmXZK7h]
## ✏️My Solution:
```
def letters(word1, word2):
  word1 = sorted(word1)
  word2 = sorted(word2)
  shared,u1,u2= [],[],[]
  for i in word1:
    if i in word2:
      if i not in shared:
        shared.append(i)
  for i in word1:
    if i not in shared:
      if i not in u1:
        u1.append(i)
  for i in word2:
    if i not in shared:
      if i not in u2:
        u2.append(i)
  return ["".join(i for i in shared),"".join(i for i in u1),"".join(i for i in u2)]
```
*I completely forgot about "sets" otherwise this would have been solved in just a few lines of code 😥*

[https://edabit.com/challenge/GaJkMnuHLuPmXZK7h]: https://edabit.com/challenge/GaJkMnuHLuPmXZK7h