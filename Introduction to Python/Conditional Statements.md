# Conditional Statements
```
def drink(money):
	if money >= 2:
		return "You bought a drink!"
	else:
		return "You couldn't afford a drink!"

print(drink(3)) # "You bought a drink!"
print(drink(1)) # "You couldn't afford a drink!"


def alcohol(age, money):
	if (age >= 18) and (money >= 5):
		return "You bought an alcohol!"
	elif (age >= 18) and (money < 5):
		return "You can't afford an alcohol!"
	elif (age < 18) and (money >= 5):
		return "You're too young to buy an alcohol!"
	else:
		return "You are too you and too poor to buy an alcohol!"

print(alcohol(18, 5)) # "You bought an alcohol!"
print(alcohol(18, 3)) # "You can't afford an alcohol!"
print(alcohol(16, 5)) # "You're too young to buy an alcohol!"
print(alcohol(14, 1)) # "You are too you and too poor to buy an alcohol!"

```
