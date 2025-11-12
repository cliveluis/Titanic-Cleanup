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


   PassengerId  Survived  Pclass  ...     Fare Cabin  Embarked
0            1         0       3  ...   7.2500   NaN         S
1            2         1       1  ...  71.2833   C85         C
2            3         1       3  ...   7.9250   NaN         S
3            4         1       1  ...  53.1000  C123         S
4            5         0       3  ...   8.0500   NaN         S

[5 rows x 12 columns]

print(f"Survival rate: {train['Survived'].mean():.2%}")


Survival rate: 38.38%


