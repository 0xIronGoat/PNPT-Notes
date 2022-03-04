# Functions
Chunks of code that can be defined and then called multiple times later on.
Means you don't have to write the same cade out multiple times, you can just call the function.

Function definition and call:
```
def who_am_i():
	name = "IronGoat"
	age = 33
	print("My name is " + name + " and I am " str(age) + " years old.")

who_am_i()
```

**Note:** Python is very particular about indentation. Code intended to be part of a function must be indented. Notice the function call at the end is then *not* indented, as it is not part of the function.

Parameters:
```
# One parameter
def add_one_hundred(num):
	print(num + 100)

add_one_hundred(70) # Will print 170

# Two parameters
def add_two_nums(num1, num2):
	print(num1 + num2)

add_two_nums(20, 45) # Will print 65
```

Return statement:
```
def multiply(num1, num2):
	return(num1 * num2)

multiply(10, 10) # This will not print any output, as function does not print
print(multiply(10, 10)) # This will print the returned value


def square_root(num):
	return(num ** 0.5)

print(square_root(64)) # Will print 8.0
```