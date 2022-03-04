# Variables and Methods
Assign and print a string variable:
```
quote="There are more things in Heaven and Earth, Horatio, than are dreamt of in your philosophy."
print(quote)
```

Methods:
```
print(quote.upper()) # Print quote in upper case
print(quote.lower()) # Print quote in lower case
print(quote.title()) # Print quote in title case

print(len(quote)) # Print length (in characters) of quote
```

Variable types:
```
name = "IronGoat" # string
age = 33 # integer
gpa = 3.7 # float

# convert float value to integer, i.e. trunates number but does NOT round it
print(int(gpa)) 

# Convert int value to string so that it can be printed as part of a string concatenation
print("My name is " + name + " and I am " str(age) + " years old.")

# Add 1 to age
age +=1
print(age)

# Add 1 to age via variable birthday
birthday = 1
age += birthday
print(age)
```