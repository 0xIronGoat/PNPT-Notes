# Importing Modules
Many modules are built in to python, but there's a lot of optional ones out there that can do some very useful things, e.g. `sys` which can perform functions related to your python installation or `os` which performs functions related to your operating system.

##### Modules must be imported before they can be used
```
import sys

print(sys.version) # Print your current version of python
sys.exit() # Exit python cleanly
```


##### You can also import specific *parts* of a module, rather than the entire module:
```
from datetime import datetime

print(datetime.now()) # Print current date and time
```


##### You can import modules with *aliases*:
```
from datetime import datetime as dt

print(dt.now()) # Print current date and time
```