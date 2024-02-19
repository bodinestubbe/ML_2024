# ML_2024

## Exploratory Data Analysis

# Loading from dotenv

1. Make sure you have the package `dotenv` installed, `pip install python-dotenv`

2. Make sure you have a .env file inside the folder ML_2024 with the following contents, adjusted for your own computer. Example for my file:

```
path_to_repo=/Users/casperruegg/Documents/python_projects/ML_2024
```

3. When importing the data to your own code, make sure to do it in this way
   
```
import os
from dotenv import load_dotenv

load_dotenv()

#load variable from .env file
ROOT_DIRECTORY = os.getenv("path_to_repo")

data = ROOT_DIRECTORY + '/data'
```

