# Lists
Lists are data structures, groups of elements  
Each object in a list is called an item  
Lists are denoted by square brackets, `[]`  
**Mutable** - can be altered  

```
movies = ["Lord of the Rings", "Star Wars", "Interstellar", "The Shawshank Redemption"]

print(movies[1]) # "Star Wars"
print(movies[0]) # "Lord of the Rings"
```

**Note:** Lists always start at index/position `0`

##### Printing multiple items from a list:
```
print(movies[1:3]) # ['Star Wars', 'Interstellar']
print(movies[1:4]) # ['Star Wars', 'Interstellar', 'The Shawshank Redemption']
print(movies[1:]) # ['Star Wars', 'Interstellar', 'The Shawshank Redemption']
print(movies[:2]) # ['Lord of the Rings', 'Star Wars']
```

- First number is the starting index/position
- Leave the first number blank to start at beginning of list
- Second number is the end index/position - **not inclusive**! i.e. it will stop printing items at the position *before* the number you put here
- You can leave the second number blank to continue printing items to the end of the list

##### Print last item in the list:
```
print(movies[-1]) # "The Shawshank Redemption"
```

##### Print length of a list:
```
print(len(movies)) # 4
```

##### Append item to end a list:
```
movies.append("Ashens and the Polybius Heist")
print(movies) # ['Lord of the Rings', 'Star Wars', 'Interstellar', 'The Shawshank Redemption', 'Ashens and the Polybius Heist']
```

##### Delete item from end of a list:
```
movies.pop()
print(movies) # ['Lord of the Rings', 'Star Wars', 'Interstellar', 'The Shawshank Redemption']
```

##### Delete item from specific position in a list:
```
movies.pop(0)
print(movies) # ['Star Wars', 'Interstellar', 'The Shawshank Redemption']
```