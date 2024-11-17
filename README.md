# DSC210-final-project-topic10-SGD-CD

# 1. How to load datasets 
   We use classical ML datasets for this project: https://machinelearningmastery.com/standard-machine-learning-datasets/. <br />
   **FOR NOW** For testing out stage, we use 
   ```
   from sklearn.datasets import load_iris
   ```
   or
   ```
   data = pd.read_csv("data.txt", header = None)
   ```

# 2. Randomization of datasets
   We use permutation test to randomization the dataset.
   ```
   X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
   indices = np.random.permutation(len(X_train))
   ```
