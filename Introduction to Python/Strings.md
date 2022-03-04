# Strings
Shebang, good idea to include at the top of every script, points to your python binary so you can execute a script with `./script.py` rather than having to be explicit with `python3 script.py`:
```
#!/bin/python3
```

  
Printing text can use single or double quotes, newlines can be printed with regular expression `\n`:
```
print("Hello, world!")
print('\n')
print('Hello, world!')
```

  
Strings can be on multiple lines:
```
print("""This string runs 
multiple lines!""")
```

  
Concatenation:
```
print("This string is " + "awesome!")
```
