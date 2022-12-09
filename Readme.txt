Dataset: https://www.kaggle.com/datasets/vic006/beginner

Model: https://hkustconnect-my.sharepoint.com/:u:/g/personal/khleebi_connect_ust_hk/EYjST-XbZs5GmEzGpQNpqJcBSygfUvOkJAyNSfZQskAIYg?e=ubqSd8


Structure:

Conv2D(input_shape=(64, 64, 3), filters=64, kernel_size=(3, 3), padding="same", activation="relu")
Conv2D(filters=64, kernel_size=(3, 3), padding="same", activation="relu")
Conv2D(filters=64, kernel_size=(3, 3), padding="same", activation="relu")
MaxPooling2D(pool_size=(2, 2), strides=(2, 2))

Conv2D(filters=128, kernel_size=(3, 3), padding="same", activation="relu")
Conv2D(filters=128, kernel_size=(3, 3), padding="same", activation="relu")
Conv2D(filters=128, kernel_size=(3, 3), padding="same", activation="relu")
MaxPooling2D(pool_size=(2, 2), strides=(2, 2))

Conv2D(filters=256, kernel_size=(3, 3), padding="same", activation="relu")
Conv2D(filters=256, kernel_size=(3, 3), padding="same", activation="relu")
Conv2D(filters=256, kernel_size=(3, 3), padding="same", activation="relu")
MaxPooling2D(pool_size=(2, 2), strides=(2, 2))

Flatten()
Dense(units=4096, activation="relu", kernel_regularizer="l2")
Dropout(0.5)
Dense(units=1024, activation="relu", kernel_regularizer="l2")
(Dropout(0.5)
Dense(units=30, activation="softmax", kernel_regularizer="l1")