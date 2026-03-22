# Artificial Intelligence Tools

A collection of six AI and machine learning algorithms implemented from scratch in Java as part of a university course. Each project demonstrates a fundamental technique - from supervised classification to unsupervised clustering and combinatorial optimization - without relying on external ML libraries.

## Projects

### Project 1 - k-Nearest Neighbors (k-NN)

A classic instance-based classifier that predicts a sample's class by majority vote among its *k* closest neighbors (Euclidean distance). Includes tie-breaking by random selection.

- **Dataset:** Iris (4 numeric features, 3 classes)
- **Usage:** `java nai.project1.Main <k> <training_file> <test_file>`
- **Interactive mode:** after evaluation, enter comma-separated feature values to classify new samples in real time

---

### Project 2 - Single-Layer Perceptron

A binary linear classifier that learns a decision boundary through iterative weight adjustment. Weights are normalized after each epoch to prevent overflow.

- **Dataset:** Iris (binary subset, 4 numeric features)
- **Usage:** `java nai.project2.Main <learning_rate> <training_file> <test_file>`
- **Interactive mode:** enter feature values for on-the-fly classification

---

### Project 3 - Language Detection (Multi-Class Perceptron)

A one-vs-all perceptron ensemble that identifies the language of a text sample. Each input is represented as a 26-element vector of letter frequency ratios (a–z).

- **Dataset:** text files organized in per-language directories
- **Usage:** `java nai.project3.Main <articles_directory>`
- **Interactive mode:** type or paste text to get a language prediction

---

### Project 4 - K-Means Clustering

An unsupervised clustering algorithm that partitions data into *k* groups by iteratively assigning points to the nearest centroid and recomputing centroids until convergence. Reports within-cluster variance (WCV) at each iteration.

- **Dataset:** Iris (labels ignored during clustering)
- **Usage:** `java nai.project4.Main <data_file> <k>`

---

### Project 5 - Naive Bayes Classifier

A probabilistic classifier based on Bayes' theorem with the naive independence assumption. Uses Laplace smoothing to handle unseen feature–outcome combinations.

- **Dataset:** weather/tennis datasets (categorical features)
- **Usage:** `java nai.project5.Main <training_file> <test_file>`
- **Interactive mode:** enter comma-separated feature values for classification

---

### Project 6 - 0/1 Knapsack Problem (Dynamic Programming)

Solves the classic knapsack optimization problem using recursive backtracking with branch-and-bound pruning. Finds the optimal subset of items that maximizes total value without exceeding the weight capacity.

- **Dataset:** `knapsack.txt` (capacity, weights, values)
- **Usage:** `java nai.project6.Main <data_file>`

---

## Project Structure

```
src/nai/
  project1/    # k-Nearest Neighbors
  project2/    # Single-Layer Perceptron
  project3/    # Language Detection (Multi-Class Perceptron)
  project4/    # K-Means Clustering
  project5/    # Naive Bayes Classifier
  project6/    # 0/1 Knapsack Problem
data/          # Training and test datasets
```

## Tech Stack

- **Language:** Java
- **Build:** Standalone (no external dependencies)
- **IDE:** VS Code (launch configurations included in `.vscode/`)
