## 📦Challenge:
At a lemonade stand, each lemonade costs $5. Customers are standing in a queue to buy from you, and order one at a time.

Each customer will only buy one lemonade and pay with either a $5, $10, or $20 bill. You must provide the correct change to each customer so that the net transaction is that the customer pays $5.

Return True if and only if you can provide every customer with correct change.
For more details of the challenge, [Click here][https://edabit.com/challenge/voxWDZ9NSv8CXifec]
## ✏️My Initial Solution:
```
def lemonade(bills):
	return True if bills.count(5)>=bills.count(10)+bills.count(20) else False
```
*After submitting my answer, when I looked at other solutions, I saw EVERYONE was using 'for' loops for this. I was very happy that I solved it with just 1 line of code. Then I realized that my solution was right but my approach was wrong. Since customers are coming one-by-one, the `.count()` method cannot be used here. It would be practically wrong. Use of 'for' loop is the correct way here. I tried to update my answer on the site but I did not happen for some reason.*

## ✏️My Improved Solution:
```
def lemonade(bills):
    change = []
    for i in bills:
        try:
            if i == 5: change.append(5)
            elif i == 10:
                change.append(10)
                change.remove(5)
            else:
                change.append(20)
                change.remove(10)
                change.remove(5)
        except ValueError:
            return False
    return True
```
[https://edabit.com/challenge/voxWDZ9NSv8CXifec]: https://edabit.com/challenge/voxWDZ9NSv8CXifec