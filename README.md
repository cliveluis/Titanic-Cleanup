# Titanic EDA – Clive Luis

Quick data load and preview of the Titanic dataset using **pandas**.

## What I Did
- Loaded `train.csv` from the Titanic competition  
- Previewed the first 5 rows with `train.head()`  
- Calculated the **overall survival rate**

## Code & Output
```python
import pandas as pd

# Load data
train = pd.read_csv('/kaggle/input/titanic/train.csv')

# Preview
print(train.head())
