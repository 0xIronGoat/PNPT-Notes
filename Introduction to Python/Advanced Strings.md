# Advanced Strings
##### Print specific characters from a string
```
name = "IronGoat"
print(name[0]) # "I"
print(name[-1]) # "t"

sentence = "This is a sentence."
print(sentence[:4]) # "This"
print(sentence[-9:-1]) # "sentence."
```

##### Split and print based on a delimiter (default = space)
```
print(sentence.split()) # ['This', 'is', 'a', 'sentence.']
```
##### Split sentence by spaces, then join back with a space (' ') delimiter, and print again
```
sentence_split = sentence.split()
sentence_join = ' '.join(sentence_split)
print(sentence_join) # "This is a sentence."
```
##### To put quotes inside a string, use the other type of quote, e.g. single quotes inside double quotes, or vice-versa
```
quote = "He said, 'give me all your money!'"
print(quote)
```
##### Or you could use escape characters to tell python to ignore the quote character
```
quote = "He said, \"give me all your money!\""
print(quote)
```

##### Stripping space from string:
```
too_much_space = "               Hello!            "
print(too_much_space.strip()) # "Hello!"
```

##### Boolean checks
```
print("A" in "Apple") # True
print("a" in "Apple") # False

# Remove case-sensetivity
letter = "A"
word = "Apple"
print(letter.lower() in word.lower()) # True
```

##### Format
```
movie = "Interstellar"
print("My favourite movie is {}.".format(movie)) # "My favourite movie is Interstellar"

# You can use multiple variables with format
name = "IronGoat"
print("My name is {} and {} is my favourite movie on the citadel!".format(name, movie)) # My name is IronGoat and Interstellar is my favourite movie on the citadel!

```


##### The same can also be achieved with f-string print statement
```
name = "IronGoat"
movie = "Interstellar"
print(f"My name is {name} and {movie} is my favourite movie on the citadel!")
```

Heath didn't cover this last one in his video but I think it's the neatest way to format this.