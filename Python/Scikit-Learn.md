[[Python]]
```Python
from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score

# Laden des Iris-Datasets
iris = load_iris()
X_train, X_test, y_train, y_test = train_test_split(iris.data, iris.target, test_size=0.3)

# Trainieren eines Random Forest Classifiers
clf = RandomForestClassifier(n_estimators=100)
clf.fit(X_train, y_train)

# Vorhersagen treffen und Genauigkeit berechnen
y_pred = clf.predict(X_test)
print("Genauigkeit:", accuracy_score(y_test, y_pred))

```
