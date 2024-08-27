[[Python]]
```Python
import pandas as pd

# Erstellen eines DataFrames
data = {
    'Name': ['Anna', 'Bob', 'Charlie'],
    'Alter': [23, 35, 45],
    'Stadt': ['Berlin', 'München', 'Hamburg']
}
df = pd.DataFrame(data)

# Daten analysieren
print(df.describe())  # Statistische Übersicht über numerische Daten
print(df[df['Alter'] > 30])  # Filtern der Daten nach Bedingung

```