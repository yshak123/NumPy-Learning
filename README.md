# 📦 NumPy Revision Notebook

A beginner-friendly NumPy revision notebook with **definitions**, **examples**, and **comments** for every concept — built for students learning Data Science and Machine Learning.

---

## 📁 Files

| File | Description |
|---|---|
| `Numpy_revision_commented.ipynb` | Main notebook with all topics, comments & examples |
| `numpy_cheat_sheet.jpg` | Visual cheat sheet for quick reference |

---

## 📚 Topics Covered

### 1️⃣ Array Creation
- `np.array()` — create from list
- `np.arange()` — range array
- `np.linspace()` — evenly spaced values
- `np.zeros()`, `np.ones()`, `np.full()` — initialized arrays
- `np.empty()` — uninitialized array
- `np.identity()`, `np.eye()` — identity matrix

### 2️⃣ Array Attributes
- `.ndim`, `.shape`, `.size`, `.dtype`, `.itemsize`, `.nbytes`, `.T`

### 3️⃣ Array Manipulation
- `astype()`, `repeat()`, `transpose()`, `flip()`, `delete()`, `unique()`
- `concatenate()`, `stack()`, `vstack()`, `hstack()`
- `split()`, `hsplit()`

### 4️⃣ Reshaping
- `reshape()`, `flatten()`, `ravel()`
- Using `-1` to auto-calculate dimensions

### 5️⃣ Broadcasting
- Scalar broadcasting
- Row and column vector broadcasting
- Shape compatibility rules

### 6️⃣ Indexing & Slicing
- 1D, 2D, 3D indexing
- Slicing with `[start:stop]`
- **Boolean indexing** — `arr[arr > 50]`
- **Fancy indexing** — `arr[[0, 2, 4]]`

### 7️⃣ The `axis` Parameter
- `axis=0` → column-wise (down rows)
- `axis=1` → row-wise (across columns)
- Applied to `sum`, `mean`, `max`, `min`

### 8️⃣ Mathematical Functions
- `np.abs()`, `np.exp()`, `np.log()`, `np.log2()`, `np.log10()`
- `np.power()`, `np.sqrt()`
- `np.floor()`, `np.ceil()`, `np.round()`, `np.clip()`

### 9️⃣ Statistical Functions
- `np.mean()`, `np.median()`, `np.std()`, `np.var()`
- `np.sum()`, `np.prod()`, `np.min()`, `np.max()`

### 🔟 Sorting & Searching
- `np.sort()`, `np.argsort()`
- `np.argmax()`, `np.argmin()`
- `np.where()`

### 1️⃣1️⃣ Logical Operations
- `np.all()`, `np.any()`
- `np.logical_and()`, `np.logical_or()`, `np.logical_not()`

### 1️⃣2️⃣ Random Number Generation
- `np.random.randint()` — random integers
- `np.random.rand()` — uniform floats [0, 1)
- `np.random.randn()` — normal distribution
- `np.random.choice()` — random pick from array

### 1️⃣3️⃣ Linear Algebra
- `np.dot()` / `@` — matrix multiplication
- Element-wise vs matrix multiplication

### 1️⃣4️⃣ Copy vs View ⚠️
- Why slicing returns a **view** (not a copy)
- How to safely use `.copy()`
- `np.shares_memory()` to check

### 1️⃣5️⃣ NaN Handling
- `np.isnan()`, `np.nan_to_num()`
- `np.nansum()`, `np.nanmean()`, `np.nanmax()`, `np.nanmin()`

### 🎁 Bonus One-Liners
- Z-score normalization
- Min-Max normalization
- NaN detection and replacement

---

## 🚀 How to Run

### Option 1 — Jupyter Notebook (Local)
```bash
# Install dependencies
pip install numpy jupyter

# Launch notebook
jupyter notebook Numpy_revision_commented.ipynb
```

### Option 2 — Google Colab (No install needed)
1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Click **File → Upload Notebook**
3. Upload `Numpy_revision_commented.ipynb`
4. Click **Runtime → Run All**

### Option 3 — VS Code
1. Install the **Jupyter** extension in VS Code
2. Open `Numpy_revision_commented.ipynb`
3. Select a Python kernel and run cells

---

## 🛠️ Requirements

```
Python >= 3.8
numpy >= 1.21
jupyter (optional, for notebook interface)
```

Install with:
```bash
pip install numpy jupyter
```

---

## 💡 Tips for Beginners

- Always check `.shape` and `.dtype` after creating or transforming arrays
- Remember: **slicing gives a view**, not a copy — use `.copy()` to be safe
- Use `axis=0` for column-wise, `axis=1` for row-wise operations
- `np.where(condition)` is your best friend for filtering data
- Combine NumPy with **Pandas** for powerful data analysis 🐼

---

## 📌 Quick Reference

```python
import numpy as np

np.array([1,2,3])          # create array
np.arange(0, 10, 2)        # [0, 2, 4, 6, 8]
np.linspace(0, 1, 5)       # [0, 0.25, 0.5, 0.75, 1.0]
arr.reshape(3, 4)           # change shape
arr[arr > 50]               # boolean filter
np.sum(arr, axis=0)         # column-wise sum
np.dot(a, b)  or  a @ b    # matrix multiply
np.isnan(arr)               # detect NaN
np.nanmean(arr)             # mean ignoring NaN
arr.copy()                  # safe independent copy
```

---

## 📖 Learning Resources

| Resource | Link |
|---|---|
| NumPy Official Docs | [numpy.org/doc](https://numpy.org/doc/stable/) |

---

## 🤝 Contributing

Feel free to open an issue or pull request if you find any mistakes or want to add more examples!

---

⭐ **Star this repo if it helped you!**
