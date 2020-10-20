## 📦Challenge:
Create a function that takes two strings and determines if an anagram of the first string is in the second string. Anagrams of "bag" are "bag", "bga", "abg", "agb", "gab", "gba". Since none of those anagrams are in "grab", the answer is false. A "g", "a", and "b" are in the string "grab", but they're split up by the "r".
For more details of the challenge, [Click here][https://edabit.com/challenge/LF6LyPmjcuLnSjgiL]
## ✏️My Solution:
```
from itertools import permutations
def ana_str_str(needle, haystack):
    count=0
	for i in list(permutations(needle)):
		count += haystack.count("".join(j for j in i))
        if count > 0: break
	if count > 0: return True
	else: return False
```

[https://edabit.com/challenge/LF6LyPmjcuLnSjgiL]: https://edabit.com/challenge/LF6LyPmjcuLnSjgiL