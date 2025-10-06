# Decision-tree
### 📄 `README.md`

```markdown
# 🧠 Decision Tree Classifier from Scratch (CART Algorithm)

This project implements a **Decision Tree Classifier** using the **Classification and Regression Trees (CART)** algorithm from scratch in Python — without using libraries like `scikit-learn`.

It uses the **Banknote Authentication Dataset** to predict whether a banknote is genuine or forged, based on image-based statistical features.

---

## 📌 Features

- Built completely from scratch using basic Python (no ML libraries)
- Uses **Gini Index** as the splitting criterion
- Supports:
  - Tree building with `max_depth` and `min_size` constraints
  - Cross-validation evaluation
  - Prediction on unseen data
- Fully modular and readable code
- Great for learning how decision trees work under the hood

---

## 📂 Dataset

**Filename:** `data_banknote_authentication.csv`  
**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/banknote+authentication)  
**Attributes:**

1. Variance of wavelet transformed image
2. Skewness of wavelet transformed image
3. Curtosis of wavelet transformed image
4. Entropy of image
5. Class label (0 = forged, 1 = genuine)

---

## 🧱 Project Structure

```

├── decision_tree.py       # Main script with all functions
├── data_banknote_authentication.csv
├── README.md

````

---

## 🚀 How to Run

1. **Clone the repository** (or download the files):

   ```bash
   git clone https://github.com/yourusername/decision-tree-from-scratch.git
   cd decision-tree-from-scratch
````

2. **Ensure Python 3 is installed**

3. **Run the script**:

   ```bash
   python decision_tree.py
   ```

   The script:

   * Loads the dataset
   * Converts strings to floats
   * Runs 5-fold cross-validation
   * Prints accuracy per fold and mean accuracy

---

## 📈 Sample Output

```
Scores: [98.91, 98.91, 100.0, 97.81, 99.27]
Mean Accuracy: 98.98%
```

---

## 🧠 Key Functions Explained

| Function                   | Purpose                                              |
| -------------------------- | ---------------------------------------------------- |
| `load_csv()`               | Load and parse CSV file                              |
| `str_column_to_float()`    | Convert string values to float                       |
| `cross_validation_split()` | Split data for k-fold evaluation                     |
| `get_split()`              | Find the best feature and threshold using Gini Index |
| `split()`                  | Recursively build the decision tree                  |
| `predict()`                | Make predictions using the tree                      |
| `evaluate_algorithm()`     | Evaluate model with cross-validation                 |
| `decision_tree()`          | Wrap training and prediction                         |

---

## 🛠️ Parameters to Tune

You can change these at the bottom of the script:

```python
n_folds = 5
max_depth = 5
min_size = 10
```

---

## ✅ Project Goals

* ✅ Understand decision tree internals
* ✅ Implement classification logic step-by-step
* ✅ Learn recursive programming and tree traversal
* ✅ Build a real-world ML model without libraries

---

## 📌 Future Enhancements

* [ ] Visualize the decision tree
* [ ] Add post-pruning to reduce overfitting
* [ ] Handle categorical features
* [ ] Convert to OOP (class-based model)
* [ ] Compare results with scikit-learn

---

## 👨‍💻 Author

**Tonnis Ondito**
GitHub: [@Maliph-Guye](https://github.com/Maliph-Guye)
Email: [onditotonnis@gmail.com](mailto:onditotonnis@gmail.com.com)

---

## 📝 License

This project is open-source and available under the [MIT License](LICENSE).

```

---

## 🧩 Next Steps

- Replace `"Your Name"` and GitHub links with your info
- Optionally, add screenshots or visualizations
- Save this file as `README.md` in the root of your project directory

Would you like a `requirements.txt` (if you add plotting), a `.py` script version of all code, or help with turning this into a Jupyter notebook?
```
