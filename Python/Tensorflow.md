[[Machine Learning]]
[[Python]]
```Python
import tensorflow as tf

# Erstellen eines einfachen neuronalen Netzes
model = tf.keras.Sequential([
    tf.keras.layers.Dense(128, activation='relu', input_shape=(784,)),
    tf.keras.layers.Dense(10, activation='softmax')
])

# Kompilieren des Modells
model.compile(optimizer='adam',
              loss='sparse_categorical_crossentropy',
              metrics=['accuracy'])

# Training des Modells (mit einem Beispiel-Dataset wie MNIST)
# (Normalerweise würden hier Trainingsdaten verwendet werden)
# model.fit(train_images, train_labels, epochs=5)

print(model.summary())

```