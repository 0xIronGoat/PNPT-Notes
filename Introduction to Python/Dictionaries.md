A dictionary is a set of "key:value pairs"
Denoted by `{}`

##### Drink is a *key*, and price is the value
```
drinks = {"White Russian": 7, "Old Fashioned": 10, "Lemon Drop": 8}
print(drinks)
```

##### You can assign lists to the values
```
employees = {"Finance": ["Bob", "Linda", "Tina"], "IT": ["Gene", "Louise", "Teddy"], "HR": ["Jimmy Jr.", "Mort"]}
print(employees)
```

##### You can add a new key:value pair in multiple ways
```
employees["Legal"] = ["Mr. Frond"]
print(employees)

employees.update({"Sales": ["Andie", "Ollie"]})
print(employees)
```

##### You can update existing entries
```
drinks["White Russian"] = 8
print(drinks)
```

##### You can grab specific items from the dictionary
```
print(drinks.get("White Russian")) # Prints the key's value, i.e. 8
```